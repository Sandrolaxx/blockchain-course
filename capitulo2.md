# Funcionamento do Blockchain: mecanismo, consenso e incentivos

Até o momento, conceituamos o blockchain, explicando o que é, o que se propõe a resolve e quais os benefícios esperados. Do ponto de vista tecnológico, a grande revolução promovida pela tenologia é a de como atingimos um consenso em uma rede decentralizada de participantes.

Porém, existem vários algoritmos para atingir este consenso, cada um com suas vantagens e desvantagens, o conteúdo deste capítulo se baseia nesse tema e de como tecnicamente o *blockchain* funciona.

---

## Redes Públicas x Privadas

Antes de continuarmos quanto aos algorítimos de consenso, temos de compreender que a uma *blockchain* pode estar sendo executada em uma rede pública ou privada.

**Rede Pública**: Como nome já bem diz, são redes mais democráticas e que possibilitam a qualquer um participar da rede a qualquer momento. Elas são descentralizadas e ninguém possui o controle total sobre a rede. Um membro pode deixar de ser um participante com a mesma facilidade em que entrou, sem pedir permissão a ninguém, basta deixar de rodar o software ou desligar o equipamento.

Contudo, devida a alta concorrência, atuar como validado de transações de um *blockchain*(papel vulgarmente conhecido como minerador) geralmente envolve um grande investimento, logo em redes públicas, é comum ser estabelecido um incentivo ou recompensa aos participantes, geralmente o ativo que a *blockchain* se propõe a validar. Assim sendo, mineradores da rede Bitcoin recebem bitcoins como recompensa, participantes da rede Ethereum recebem ethers e assim por diante.

**Rede Privada**: São redes fechadas e os membros devem ser convidados a participar, nessa categoria de rede o controle é de uma empresa ou de um consórcio de empresas, que escolhem a dedo seus participantes, possuem algoritmos de consenso mais simples e não tem nenhum incentivo ou recompensa aos validadores da rede, encorajados a realizar esse papel mediante outros modelos de negócios, sendo geralmente encarado como qualquer outra despesa de infraestrutura da empresa.

---

## O Problema dos Generais Bizantinos

Para ilustrar o problema de um consenso descentralizado, podemos pegar o artigo publicado por Lamport, Shostak e Pease(1982) que elaboraram o seguinte problema, imagine vários generais bizantinos com seus exércitos, estes que realizaram um cerco em volta de um reino, e eles têm de decidir por um plano de ação comum, se vão atacar ou recuar, cada general tem autonomia em sua decisão, os generais só podem se comunicar através de mensageiros.

Considere também que alguns desses generais foram subornados e se tornaram traidores, assim sendo suas decisões não irão conforme as dos generais leais, um general traidor pode decidir recuar quando o melhor plano de ação seria atacar.

Os generais bizantinos precisam de um algoritmo de consenso que:

1. Todos os generais decidam pelo mesmo plano de ação, eles farão o que for decidido, enquanto os traidores farão o que quiserem.
2. Um pequeno número de traidores não influencie a decisão dos generais leais, fazendo-os tomar a pior decisão.

<br>

>Desenho do Problema dos Generais Bizantinos
![Desenho do Problema dos Generais Bizantinos](/images/generaisBizantinos.png)

<br>

Nesse caso se todos os generais trocarem mensagens entre si, eles poderiam optar pelo plano de ação mais recebido, desconsiderando a opção "votada" em minoria.

Em um livro-razão distribuído, quaisquer entradas(as mensagens) para o livro-razão(o ataque acordado) devem ser confiáveis. As redes digitais geralmente possuem milhares a milhões de membros ou nós(os generais) que estão dispersos globalmente e não há um comando centralizado(nenhuma governança central), e é impossível se conhecer e confiar em todos os membros. 

Então, como você pode confiar nos outros membros da rede e garantir que as entradas para o registro distribuído sejam precisas e, além disso, garantir que este possua as informações corretas? O *Blockchain* resolve esse problema e, no caso do nosso general bizantino, garante que ele possa enviar mensagens confiáveis e liderar um ataque bem-sucedido e coordenado(GHOSH,2016).

<br>

>Problema dos Generais em uma Rede Blockchain
![Problema dos Generais em uma Rede Blockchain](/images/generaisBizantinosBlockchain.png)

<br>


---

## Descentralização e o Ataque de 51%

O grande risco de um *blockchain* é que vários membros mal-intencionados da rede, tenha majoritariamente a maioria dos nós da rede, ou seja, 51% dela, assim tendo o controle da rede, de modo a centralizar as decisões e também comandá-las, e caso queiram, por exemplo, reorganizar blocos já validados, assim desfazendo eles e manipular as regras da rede a sua própria escolha.

---

## Como Atigir o Consenso em Uma Rede Descentralizada

Conforme abordado anteriormente, além de garantir que os dados registrados neste livro-razão são confiáveis, cada membro da rede deve possuir uma **cópia idêntica e completa** desse livro-razão. Por se tratar de um livro-razão que é escrito a todo instante, ele é dividido em blocos que contém as transações, operações ou dados que devem ser registrados.

Sempre que novas informações precisam ser registradas, um novo bloco deve ser criado, preenchido, validado e posicionado no final do livro-razão, incrementando este grande documento. Estes blocos são encadeados de tal maneira que a assinatura usada para validar o bloco anterior é necessária para validar o novo bloco, criando a famosa "cadeia de blocos" que batiza a tecnologia.

É esse encadeamento que torna a blockchain imutável, já que a alteração ou remoção de um dado já registrado necessitaria da revalidação do bloco em que o dado está e todos os blocos gerados anterior e posteriormente.

No entanto, vamos abordar a seguinte questão: Se as cópias do blockchain são idênticas, como decidir quais transações serão registradas aos novos blocos? Através de algoritmos de consenso, é claro! A cada novo bloco é eleito um membro que ganha o direito de registrar os dados no bloco, cabendo aos demais a função de validá-lo.

Vários são os algoritmos de consenso aplicados para este fim, cada um com suas vantagens e desvantagens. Veremos em detalhes os dois mais utilizados, o Proof of Work(POW) e Proof of Steak(POS), e daremos uma visão geral sobre alguns outros não tão utilizados.

---

## Proof of Work(POW) Aplicado no Consenso de Nakamoto

A Prova de Trabalho(ou Proof of Work) é um protocolo criptográfico criado para prevenção de ataques cibernéticos de negação de serviço(Denial of Service) e Spam, proposto por Cynthia Dwork e Moni Naor em um artigo de 1993. O termo "Prova de Trabalho", entretanto, só foi cunhado seis anos depois, em um artigo de Markus Jakobson e Ari Juels.

Inspirado por BACK(2002), que explorou a Prova de Trabalho para ataques de negação de serviço em um mecanismo batizado de Hashback, Satoshi Nakamoto adaptou os conceitos de Prova de Trabalho que funcionasse como um algoritmo de consenso(NAKAMOTO, 2008), o que passou a ser conhecido posteriormente como consenso de Nakamoto(Nakamoto Consensus).

### Mecanismo

Nesta abordagem, a cada bloco um líder é eleito através de uma forma de "loteria". Falando especificamente da rede Bitcoin, um enigma criptográfico é proposto pelo protocolo e os membros que participam desta rede se propõem a decifrá-lo. Basicamente o enigma é a execução de uma função hash SHA-256 utilizando alguns dados específicos do bloco atual e um número aleatório, resultando em um hash que comece com um determinado número de zeros. Se o número de zeros em questão não for obtido, a função hash deve ser tentada utilizando outro número aleatório.

O enigma criptográfico é este: adivinhar o número aleatório(também conhecido como **nonce**) que, aliada as informações do bloco, deve resultar em um hash iniciado por um número de zeros. Para se ter uma ideia como a adivinhação deste número é algo trabalhoso, milhões de tentativas são feitas em um único segundo e este processo de descoberta leva em torno de dez minutos para acontecer.

Os participantes de rede competem entre si, apostando uma corrida de quem será o primeiro a adivinhar este número. O nó que conseguir fazer isso primeiro comunica imediatamente aos demais participantes qual é o número aleatório; estes, por sua vez, param de utilizar números aleatoriamente e usam o número informado para validar a vitória do reclamante. Confirmada a solução do enigma, os participantes da rede, em consenso, elegem este nó como líder.

O líder eleito tem o direito de determinar quais transações de Bitcoin não confirmadas irão compor o novo bloco; as transações realizadas e não confirmadas do Bitcoin formam uma fila que o membro líder deve consultar. Em novembro de 2019, o tamanho exato do bloco é de apenas 1MB, espaço capaz de armazenar cerca de três mil transações por vez. Todas as demais transações não escolhidas para confirmação no novo bloco permanecem na fila de espera e serão confirmadas nos blocos seguintes. Escolhidas as transações, o vencedor propaga o bloco formado para os demais participantes, e estes armazenam o bloco final da corrente e se preparam para a próxima corrida.