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

![Desenho do Problema dos Generais Bizantinos](https://on.fiap.com.br/pluginfile.php/1/local_conteudoshtml/conteudo/9187/assets/private/on-image-problema-generais-bizantinos.svg)

Nesse caso se todos os generais trocarem mensagens entre si, eles poderiam optar pelo plano de ação mais recebido, desconsiderando a opção "votada" em minoria.

Em um livro-razão distribuído, quaisquer entradas(as mensagens) para o livro-razão(o ataque acordado) devem ser confiáveis. As redes digitais geralmente possuem milhares a milhões de membros ou nós(os generais) que estão dispersos globalmente e não há um comando centralizado(nenhuma governança central), e é impossível se conhecer e confiar em todos os membros. 

Então, como você pode confiar nos outros membros da rede e garantir que as entradas para o registro distribuído sejam precisas e, além disso, garantir que este possua as informações corretas? O *Blockchain* resolve esse problema e, no caso do nosso general bizantino, garante que ele possa enviar mensagens confiáveis e liderar um ataque bem-sucedido e coordenado(GHOSH,2016).

---

## Descentralização e o Ataque de 51%

O grande risco de um *blockchain* é que vários membros mal-intencionados da rede, tenha majoritariamente a maioria dos nós da rede, ou seja, 51% dela, assim tendo o controle da rede, de modo a centralizar as decisões e também comandá-las, e caso queiram, por exemplo, reorganizar blocos já validados, assim desfazendo eles e manipular as regras da rede a sua própria escolha.