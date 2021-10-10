# Smart Contracts

A tecnologia do blockchain tem trazido consigo uma variedade de outras propostas de aplicação, evoluindo nas mais diferentes direções, e a mais promissora dentre elas é chamada de smart contract.

---

## O que são Smart Contracts

Os Smart Contracts (ou contratos inteligentes) podem ser definidos como o próximo passo evolucionário na prevenção de fraudes (GULKER, 2017). De acordo com Raskin (2017), o contrato inteligente é um acordo entre as partes cuja execução é automática, sendo essa automação realizada por um código de computador que traduz um discurso legal em um programa executável.

Assim sendo, o algoritmo verifica com suas estruturas condicionais se determinadas condições foram satisfeitas e, caso tenham sido, ele automaticamente executa os termos estipulados no contrato. Os Smart Contracts permitem que as partes interessadas se comprometam previamente com os termos a serem executados sem, no entanto, determinar uma autoridade central (um sistema judicial) para fazer valer sua execução (GULKER, 2017).

!["Smart Contracts"](/images/smartContracts/smartContracts.png)
<br>| - Logo IPFS(Fonte: FIAP(2019))

Portanto, podemos criar contratos, que outrora eram feitos no papel, de forma digital e, melhor do que isso, com ações automatizadas. Para tal, é necessário traduzir em linguagem de programação as condições e ações a serem realizadas, tornando os contratos autoexecutáveis. Existem várias propostas de como se implementar essa tecnologia, a mais promissora e que está sendo desenvolvida há anos é a dos contratos inteligentes na plataforma Ethereum.

Uma vez confeccionado o contrato em uma linguagem de programação utilizando uma linguagem conhecida como solidity, o contrato é publicado em um blockchain da plataforma Ethereum. Esse procedimento traz uma propriedade importante: uma vez publicado, ele não pode ser alterado ou modificado (herdando tal característica dos blockchain), ou seja, para que as condições sejam modificadas, o contrato atual precisa ser destruído (rescindido) ou abandonado, e um novo deve tomar o seu lugar. Dessa maneira, há garantias de que o contrato será executado exatamente com as condições que foram previamente estabelecidas, de forma compulsória.

---

## Aplicações em Smart Contracts

Graças a essa importante tecnologia, novas aplicações se tornaram possíveis. Veremos a seguir alguns dos exemplos mais proeminentes de contratos inteligentes.

---

## OpenBazzar, o ML sem o ML

Uma das aplicações em funcionamento desde 2014 que eliminam intermediários é o OpenBazaar, uma plataforma de comércio eletrônico ponto a ponto (P2P), ligando compradores e vendedores diretamente. Por não haver intermediários, não há taxas ou restrições para seu uso.

---

## Arcade.city, o uber sem o uber

Contratos inteligentes permitem a eliminação de intermediários, e um grupo de motoristas em Austin, no Texas, resolveu fazer o contrário: tirar o Uber da equação.

O Arcade.City é a primeira iniciativa bem-sucedida de uma rede de viagens P2P, ou seja, motoristas e passageiros são conectados ponto a ponto. A iniciativa em Austin já está em funcionamento há alguns anos, prestando o serviço de deslocamento seguro sem incidentes (DAVID, 2017). Em 2017, a cidade contava com mais de 150 motoristas ligados à rede de viagens (WISTROM, 2017).

---

## Smart Governance, votação 2.0

Há sempre suspeitas de fraude em qualquer eleição realizada em qualquer nação do mundo; há muita coisa em jogo, e os vencedores têm acesso a altos valores e muito, muito poder. Assim sendo, sistemas de votação sempre levantarão suspeitas, especialmente dos perdedores. “Sempre”, será?

Existem várias propostas para o uso de smart contracts em sistemas de votação inteligentes, afinal, suas propriedades de imutabilidade sem que haja controle por nenhuma das partes tornam as eleições uma aplicação perfeita para a tecnologia.

Além de garantir a privacidade, o contrato traz transparência ao processo de apuração, pois, ao verificar as condições em que os votos foram apurados, é possível garantir que 1 pessoa = 1 voto. Ao utilizar um blockchain como infraestrutura para que o sistema de votação seja realizado, reduz-se drasticamente quaisquer fraudes que possam hoje ser realizadas em sistemas eleitorais tradicionais.

---

## O Smart Contract mais promissor é da plataforma Ethereum

A Ethereum Foundation vem agitando o mundo da blockchain desde o início do projeto no final de 2013 e início de 2014. Existem várias propostas do que seria a evolução do Bitcoin, e o projeto apresenta uma das mais interessantes possibilidades de “Bitcoin 2.0”. O Ethereum é um projeto de blockchain com uma criptomoeda, Ether, semelhante ao Bitcoin, mas, diferentemente do Bitcoin, cujas operações se restringem a adições (na carteira destino) e subtrações (na carteira de origem), a plataforma Ethereum tem o recurso adicional de uma linguagem de máquina virtual (quase) completa de Turing e capacidade de processamento incorporada à implementação do nó (MOLECKE, 2017). O Ethereum é a resposta para a pergunta: “e se o dinheiro fosse programável? ”

---

## Solidity, a linguagem usada na plataforma Ethereum

Para possibilitar a implementação de Smart Contract, a plataforma Ethereum optou pela criação de uma linguagem de programação orientada a objetos e em alto nível para esse fim. Influenciada por C++, Python e JavaScript, surgiu a linguagem Solidity, atualmente na versão 0.7.0 (SOLIDITY, 2020).

Trata-se de uma linguagem fortemente tipada (são aquelas em que declaramosobrigatoriamente os tipos de variáveis), permite tipos complexoscustomizados esuporta bibliotecas e herança (SOLIDITY, 2020).

Assim como a linguagem Java, o Solidity é uma linguagem compilada e interpretada ao mesmo tempo: o código-fonte escrito na linguagem é armazenado em arquivos .sol e são submetidos a um compilador chamado Solidity Compiler (solc) e se transformam em bytecode; esse contrato compilado é publicado na plataforma Ethereum, que possui um interpretador conhecido como Ethereum Virtual Machine (EVM), que é responsável por interpretar este bytecode. A diferença em relação à linguagem tradicional como o Java é que essa EVM é descentralizada, e o processamento do contrato acontece em milhares de nós que compõem uma rede Ethereum atualmente.

!["Funcionamento Solidity"](/images/smartContracts/funcionamentoSolidity.png)
<br>| - Funcionamento Solidity(Fonte: Coindesk(2019))

Com o Solidity, você pode criar contratos para usos como votação, financiamento coletivo, leilões cegos e carteiras com várias assinaturas.

## Exemplo prático

Vamos a alguns exemplos práticos, para consolidar a ideia dos contratos inteligentes de maneira mais tácita. Para começarmos nossas primeiras implementações em contratos inteligentes na plataforma Ethereum, não será necessário computador potente ou complicadas instalações de software, bastará um modesto desktop/laptop com um navegador Google Chrome.

## Instalação da carteira digital Metamask

Vamos começar com a abordagem mais simples, para a qual é necessária a instalação de um plugin no Google Chrome, e esse, em questão, é o Metamask, que embute uma carteira virtual de Ethers (e tokens ERC-20 e ERC-721, dois tipos de criptos que podem ser criados na rede Ethereum), permitindo transferir valores e interagir com as dApps, os Decentralized applications, que nada mais são do que contratos inteligentes com uma interface amigável. Com o Google Chrome, acesse metamask.io e clique no link “Get chrome extension”:

!["Donwload Carteira MetaMask"](/images/smartContracts/lab01.png)
<br>| - Donwload Carteira MetaMask(Fonte: FIAP(2020))

Ao ser direcionado para a Chrome Web Store, clique em “Usar no Chrome” e posteriormente “Adicionar extensão”.

!["Instalação MetaMask no Google Chrome"](/images/smartContracts/lab02.png)
<br>| - Instalação MetaMask no Google Chrome(Fonte: FIAP(2020))

MetaMask instalado, clique no botão “Primeiros passos”.

!["Primeiros Passos instalação MetaMask"](/images/smartContracts/lab03.png)
<br>| - Primeiros Passos instalação MetaMask(Fonte: FIAP(2020))

Como estamos criando uma carteira pela primeira vez, clique no botão “Crie uma Carteira”. Posteriormente, a carteira criada fornece doze palavras no idioma inglês que, na sequência, podem restaurar a carteira em qualquer desktop (ou mesmo apps no smartphone). Daí a opção “Importar Carteira”.

!["Começo da criação da carteira no Metamask"](/images/smartContracts/lab04.png)
<br>| - Começo da criação da carteira no MetaMask(Fonte: FIAP(2020))

O plugin solicita o envio de dados para melhoria das próximas versões do Metamask. Clique no botão que julgar mais adequado e seguimos adiante.

!["Permissão de envio de dados no MetaMask"](/images/smartContracts/lab05.png)
<br>| - Permissão de envio de dados no MetaMask(Fonte: FIAP(2020))

Na sequência, informe a senha que será utilizada para assinar as transações, aceite o termo de uso e clique no botão “Criar”.

!["Criação da senha de transações do MetaMask"](/images/smartContracts/lab06.png)
<br>| - Criação da senha de transações do MetaMask(Fonte: FIAP(2020))

A frase secreta de backup composta por doze palavras no idioma inglês (conhecido como mnemônico). Clique para revelar e anote as doze palavras, ou clique em “Lembrar mais tarde”.

!["Frase secreta de backup no Metamask"](/images/smartContracts/lab07.png)
<br>| - Frase secreta de backup no Metamask(Fonte: FIAP(2020))

Pronto! A carteira no Metamask foi finalmente criada.

---

## Rede de testes e faucet no Metamask

Para implementar um contrato inteligente em uma rede de testes da plataforma Ethereum (e não gastar nenhum centavo para isso), é preciso apontar a carteira digital para uma rede de testes, como a rede Ropsten. Selecione a rede de testes na caixa de seleção na parte superior da carteira.

!["Mudança da rede Ethereum no MetaMask"](/images/smartContracts/lab08.png)
<br>| - Mudança da rede Ethereum no MetaMask(Fonte: FIAP(2020))

Será necessária uma quantia em ethers para pagar os custos da publicação do contrato na rede além de processamentos e armazenamentos de dados no contrato. Felizmente, é possível pedir ethers de teste para a rede (chamados de faucets). Para isso, clique no botão “Depósito”, presente na carteira.

!["Opção de Depósito na carteira MetaMask"](/images/smartContracts/lab09.png)
<br>| - Opção de Depósito na carteira MetaMask(Fonte: FIAP(2020))

Na sequência, clique em “Obter Ether” na “Torneira de Testes”.

!["Opção do Torneira de Testes no MetaMask"](/images/smartContracts/lab10.png)
<br>| - Opção do Torneira de Testes no MetaMask(Fonte: FIAP(2020))

Clique no botão “request 1 ether from faucet”. O dApp solicita permissão para a interação com a carteira, portanto, na tela que surge clique no botão “Conectar-se”.

!["Solicitando um ether para o faucet"](/images/smartContracts/lab11.png)
<br>| - Solicitando um ether para o faucet(Fonte: FIAP(2020))

Deve aparece um hash identificando unicamente a transação em “transactions”. Caso apareça um erro e, em poucos minutos, não aparecer 1 ether na carteira, recarregue a página e repita a operação clicando em “request 1 ether from faucet”.

!["Carteira MetaMask com uma quantia em ethers"](/images/smartContracts/lab12.png)
<br>| - Carteira MetaMask com uma quantia em ethers(Fonte: FIAP(2020))

Contudo, talvez a faucet ou “torneira” do metamask dê erro dizendo que há muitas requisições para ele – infelizmente, há algum tempo ele sofre de congestionamento. Se for o caso, tente este outro endereço: <https://faucet.ropsten.be/>.

!["Outro faucet para solicitar ethers"](/images/smartContracts/lab13.png)
<br>| - Outro faucet para solicitar ethers(Fonte: FIAP(2020))

---

## Publicação de um Smart Contract no Remix

Para implementar um contrato inteligente, a maneira mais fácil é utilizar um ambiente de desenvolvimento totalmente web-based disponibilizado pelo projeto Ethereum, o Remix. Para tal, no mesmo Google Chrome por meio do qual a carteira Metamask foi instalada, acesse <https://remix.ethereum.org/>.

!["Tela inicial do Remix"](/images/smartContracts/lab14.png)
<br>| - Tela inicial do Remix(Fonte: FIAP(2020))

Repare que, em sua barra lateral esquerda, apenas dois botões de abas aparecem. Para habilitar os demais botões do ambiente, clique no botão “Solitidy” presente na seção “Environments”.

Em File Explorers, temos uma estrutura de arquivos com códigos-fonte disponíveis. Por padrão, os arquivos ballot.sol e ballot_test.sol já estão disponíveis e se referem a um exemplo de contrato de votação inteligente, portanto, dê uma olhada posteriormente, quando o Solidity se tornar um pouco mais familiar para você.

Clique no botão “+”, presente ao lado da palavra “browser”, e peça para criar um arquivo chamado “SimpleStorage.sol”. Este exemplo, presente na documentação oficial do Solidity, é uma espécie de exemplo do tipo “Alô mundo”, que pode ser um excelente primeiro contato com a tecnologia.

!["Criando um contrato no Remix"](/images/smartContracts/lab15.png)
<br>| - Criando um contrato no Remix(Fonte: FIAP(2020))

Eis o código-fonte em Solidity conforme a documentação oficial. Vamos explicar as nuances desta linguagem, linha a linha.

```java
pragma solidity >=0.4.0 <0.7.0;

contract SimpleStorage {
    uint storedData;
    
    function set(uint x) public {
        storedData = x;
    }

    function get() public view returns (uint) {
        return storedData;
    }
}
```

A instrução **pragma solidity** é obrigatória e serve para informar com qual(is) versão(ões) do compilador solidity o código-fonte é compatível. Repare que, por estar na versão 0.7.0 (abaixo de 1), a linguagem é considerada extremamente instável, com instruções novas surgindo e outras sumindo o tempo todo. Neste caso específico, o código seria compatível com versões maiores ou iguais a 0.4.0 e menores do que 0.7.0. É possível estabelecer uma versão exata, logo, **pragma solidity** 0.5.0 significa que o código-fonte exige ser compilado em um compilador versão 0.5.0.

A instrução **contract** seguida pelo nome do contrato (**SimpleStorage**) não é muito diferente de qualquer linguagem orientada a objeto, ou seja, **contract** é equivalente ao **class**, e o objeto é a instância desse contrato, que será gerada no momento da publicação na plataforma Ethereum. As instruções presentes dentro do bloco iniciado pelo símbolo { e encerrado pelo } fazem parte do contrato em questão.

Na quarta linha, temos **uint** **storedData** , uma declaração de atributo, em um padrão bem conhecido das linguagens orientadas a objeto: o tipo de dado seguido pelo identificador do atributo. É nesses atributos que as informações do contrato são armazenadas (por isso, o nome sugestivo de storedData) e ficam visíveis por todas as operações do contrato. O tipo de dado uint é uma abreviação para **unsigned integer** ou número inteiro sem sinal, assim sendo, **storedData** aceita armazenar um número do conjunto dos números naturais. No Quadro “Tipos de dados disponíveis no Solidity”, são apresentados os tipos de dados disponíveis na linguagem.

|       Tipo de dado   |      Descrição      | 
|----------------------|---------------------|
| bool                 |  O clássico tipo de dado booleano, aceitando apenas dois estados, true ou false. | 
| int / uint           |    A linguagem conta com diversos tipos de dados para guardar números inteiros com ou sem sinal, dos mais diferentes tamanhos. Os tipos de dados int8, int16, int32, int64, int128, int256 guardam números inteiros com a quantidade de bits especificada no tipo de dado, logo, int64 usa 64 bits para guardar números no intervalo de -9.223.372.036.854.775.808 até 9.223.372.036.854.775.807. Com a letra “u” na frente, a variável guarda apenas números positivos e seu intervalor dobra, sendo assim, enquanto int16 trabalha no intervalo - 32.768 até 32.767, uint16 guarda números de 0 até 65.535 com a mesma quantidade de bits (16, nestes casos). A ausência do número de bits remete à maior versão disponível, logo, int e uint são abreviações de int256 e uint256, respectivamente.   | 
| fixed / ufixed      | Destinado para números fracionados (ou com ponto flutuante). Devem ser usadas as palavras-chave ufixedMxN ou fixedMxN, cujo M representa quantos bits são usados para a variável e o N, quantos casas decimais estão disponíveis para parte fracionada. Assim como no tipo de dado inteiro, M deve ser um número divisível por 8 dentro do intervalo 8 e 256 (bits). N, por sua vez, pode ser um número entre 0 a 80, incluindo ambos. | 
| address             | Como no caso inteiro, os tipos de dados precedidos pela letra “u” armazenam apenas números positivos, dobrando o intervalo de número positivos armazenados pelas versões sem o “u”. ufixed and fixed são abreviações dos tipos ufixed128x18 and fixed128x18, respectivamente. Atenção: estes tipos de dados ainda não estão implementados, embora apareçam na documentação oficial.| 
| bytes               | Utilizados para uma sequência de bytes de tamanho fixo, ideal para alfanuméricos. Estão disponíveis bytes1 até bytes32 e bytes é uma abreviação de bytes1. | 
| String              | Armazena alfanuméricos de tamanho variável no padrão UTF-8. | 
| Enum                | A forma mais simples de criar uma lista de valores pré-definidos no Solidity, segue exemplo de declaração: <br/>contract Produto { <br/>enum EstadoOpcoes { Novo, Seminovo, Usado } <br/>EstadoOpcoes estado = EstadoOpcoes.Novo;<br/> } | 

Voltando ao nosso código-fonte do contrato SimpleStorage, este possui dois métodos (ou operações) chamados de set e get, sendo set responsável por armazenar um número em storedData e get em exibí-lo. Repare que ambos possuem a palavra public, que define a visibilidade das funções, que podem ser chamadas livremente. O quadro “Tipos de visibilidade disponíveis no Solidity” apresenta este e outros tipos de visibilidade.

| Tipo de Visibilidade |      Descrição      | 
|----------------------|---------------------|
| public               |Um atributo ou método marcado como public pode ser acessado livremente, seja pelo próprio contrato, seus herdeiros (interno) ou outros contratos e dApps (externo).|
| private              |Para atributos e métodos que serão acessados exclusivamente pelo contrato que as possui.|
| internal | Para atributos e métodos que serão acessados apenas internamente (seja pelo contrato que as possui ou por seus filhos, que as herdam). |
| external | Este tipo de visibilidade é exclusivo para métodos e, por essa razão, não está disponível para atributos. As funções definidas como external são consideradas parte da interface do contrato e serão chamadas externamente em transações e não podem ser chamadas internamente (ou seja, em um função external f, a chamada f() não funciona, mas this.f() sim).|

Enquanto o método **set()** recebe um parâmetro x do tipo uint e faz uma persistência de dados armazenando o número em storedData, **get()** é um método apenas de visualização e, por essa razão, recebe a palavra reservada **view** indicando isso. O comando **returns** seguido pelo tipo de dado indica o que a função está retornando.

!["Escrevendo o contrato no Remix em Solidity"](/images/smartContracts/lab16.png)
<br>| - Escrevendo o contrato no Remix em Solidity(Fonte: FIAP(2020))

Antes de mais nada, o contrato precisa ser compilado no compilador Solidity solc. No Remix, clique no segundo botão no menu esquerdo (com o logo do Solidity, um “S”) e selecione a versão do compilador (optamos por utilizar a versão 0.5.16, embora existam versões mais novas!).

!["Mudando a versão do compilador Solidity no Remix"](/images/smartContracts/lab17.png)
<br>| - Mudando a versão do compilador Solidity no Remix(Fonte: FIAP(2020))

Clique no botão “Compile SimpleStorage.sol” e o bytecode estará pronto.

!["Contrato compilado no Remix"](/images/smartContracts/lab18.png)
<br>| - Contrato compilado no Remix(Fonte: FIAP(2020))

No terceiro botão do menu esquerdo (com o logo da plataforma Ethereum), realize a publicação do contrato e, para tal, selecione a opção “Injected Web3” no campo “Environment”.

!["Mudando o ambiente no Remix"](/images/smartContracts/lab19.png)
<br>| - Mudando o ambiente no Remix(Fonte: FIAP(2020))

Ao fazer isso, o Remix solicitará permissão para interagir com sua carteira mantida pelo Metamask. Clique em “Conectar-se” para conceder essa permissão.

!["Integração da carteira do Metamask com o Remix"](/images/smartContracts/lab20.png)
<br>| - Integração da carteira do Metamask com o Remix(Fonte: FIAP(2020))

Repare que a carteira do Metamask agora aparece no campo “Account”, com seu saldo (por aqui, 2 ethers). Clique no botão “Deploy”, e novamente a carteira do Metamask será acionada, agora em uma transação de “Implantação de Contrato”. Note que uma pequena taxa de rede é cobrada. No exemplo, por aqui, 0 000289 ETH (também conhecido como 289 Szabos ou 289000 GWei). Essa taxa de rede é calculada dinamicamente pelo Metamask, logo, provavelmente você notará uma diferença em sua execução. Note também que a taxa pode ser definida pelo usuário por meio do link “EDIT”. Clique no botão “Confirmar”.

!["Publicando o contrato na rede Ropsten por meio do Remix"](/images/smartContracts/lab21.png)
<br>| - Publicando o contrato na rede Ropsten por meio do Remix(Fonte: FIAP(2020))

O contrato foi publicado na rede Ropsten. Por aqui, o saldo da carteira do Metamask se tornou 1.9997 ETH, assim, a taxa para a publicação do contrato foi realmente paga. Ao ser publicado, uma instância do contrato SimpleStorage se torna ativa e um endereço o identifica unicamente nesta rede (em nosso caso, 0xA67348e15B18CB6155075eF248A8BB0fA1502Dda).

Experimente utilizar o contrato agora, primeiro, passando um número positivo qualquer por meio do método set() e, posteriormente, visualize-o usando o método get(). Os botões tornam-se disponíveis no Remix, conforme a Figura “Testando o contrato publicado na rede Ropsten no Remix”.

!["Testando o contrato publicado na rede Ropsten no Remix (1)"](/images/smartContracts/lab22.png)
<br>| - Testando o contrato publicado na rede Ropsten no Remix (1)(Fonte: FIAP(2020))

Note que, ao utilizar o método set() informando um número (em nosso caso, o “150”), a carteira Metamask é novamente chamada e uma taxa será cobrada para rodar o método. Isso acontece porque o método set() faz uma mudança de estado no contrato, mudando um valor (no caso, storedData) que está armazenado nele. Sendo assim, sempre que houver uma mudança de valor ou um grande processamento envolvido, quem chama este método terá que pagar um gas, ou seja, um “combustível” para fazer rodar esse contrato. A analogia pode ser feita com um carro mesmo: para fazê-lo rodar, é necessário gastar parte do combustível que está em seu tanque.

!["Testando o contrato publicado na rede Ropsten no Remix (2)"](/images/smartContracts/lab23.png)
<br>| - Testando o contrato publicado na rede Ropsten no Remix (2)(Fonte: FIAP(2020))

É possível calcular este “gas”? Sim, cada instrução, tamanho de variável a ser armazenada, tudo acaba influindo; para ilustrar, na figura “Tabela para cálculo de Gas no Ethereum” Gavin Wood relaciona em sua EIP-150 o custo em gás de cada tipo de instrução.

!["Tabela para cálculo de Gas no Ethereum"](/images/smartContracts/lab24.png)
<br>| - Tabela para cálculo de Gas no Ethereum(Fonte: FIAP(2020))

A chamada de um método que envolva cálculos ou alteração de variáveis, como é o caso do set(), vai custar, no mínimo, 21000 gas que, segundo Wood (s.d.) é o preço pago para cada transação. O número em gas que representa o custo de rodar um determinado método do contrato deve ser multiplicado pelo preço do gas, o chamado gas price. Segundo Rosic (2018), o preço médio do gas gira em torno de 20 Gwei (ou 0,00000002 ETH), mas este método pode subir ou descer: se a rede está muito congestionada, o valor médio do gas pode subir para 30, 40 Gwei. Note que é possível determinar o gas price que você está disposto a pagar: se você tem pressa e quer ter certeza de que uma determinada transação do contrato vai rodar com prioridade, basta comprar o combustível pelo preço mais caro. Se o gas price médio naquele momento for 20 Gwei, pagar 25 ou 30 já será mais do que suficiente para que os mineradores do Ethereum deem preferência para suas transações. Para finalizar, se o método de um Smart Contract precisa de 30.000 gas para rodar, e o gas price médio é 0,00000002 ETH, basta multiplicar um pelo outro e chegamos ao custo de rodar aquele método (neste exemplo, 30.000 gas x 0,00000002 ETH = 0,0006 ETH).

Na demonstração, é possível observar que o gas price da rede Ropsten é sensivelmente menor; Mesmo a rede principal, após algumas restruturações oriundas da atualização do software de mineração da plataforma Ethereum (atualmente na versão Istanbul) resultou em um impacto no gas price médio que, segundo Etherscan (2020) está em torno de 10 Gwei.

Por outro lado, por ser um método apenas de visualização (está até mesmo
marcado com a palavra reservada view) o método get() não gera custo, olhar para o contrato é “de graça”. O Remix destaca os métodos de forma diferente em sua interface, ao pintar os botões de chamada em cores diferentes (o set() é laranja enquanto o get() é azul). Bem, clique no botão de chamada do método get() e experimente acessar o dado armazenado no contrato.

!["Testando o contrato publicado na rede Ropsten no Remix (3)"](/images/smartContracts/lab25.png)
<br>| - Testando o contrato publicado na rede Ropsten no Remix (3)(Fonte: FIAP(2020))

Vamos, agora, escrever um contrato um pouco mais elaborado, de forma a
apresentar outros conceitos importantes do Solidity. O exemplo a seguir é um clássico jogo de azar do tipo “Bolão”: criaremos um método para entrar no bolão (pagando um valor, é claro) e, depois de juntar uma quantia interessante, uma figura que chamaremos aqui de gerente “fecha as apostas”, solicitando ao contrato sortear um dos apostadores aleatoriamente, entregando toda a bolada. Eis o código.

```java
pragma solidity 0.5.16;

contract Bolao {
    address private gerente;
    address[] private jogadores;
    address payable private vencedor;
    
    constructor() public {
        gerente = msg.sender;
    }

function entrar() public payable {
    require(msg.value == .1 ether);
    jogadores.push(msg.sender);
}

function descobrirGanhador() public restricted {
    uint index = randomico() % jogadores.length;
    vencedor = address(uint160(jogadores[index]));
    vencedor.transfer(address(this).balance);
    jogadores = new address[](0);
    vencedor = address(uint160(0x0));
}

modifier restricted() {
    require(msg.sender == gerente);
    _;
}

function getSaldo() public view returns (uint) {
    return uint(address(this).balance);
}

function randomico() private view returns (uint) {
    return uint(keccak256(abi.encodePacked(block.difficulty, jogadores)));
```

Neste contrato, são declarados três atributos: um para guardar o endereço da carteira do gerente, um para guardar endereços dos jogadores que fazem apostas e um para guardar o endereço da carteira do vencedor (e realizar a transferência). Repare que o tipo de dado para jogadores é **address[]**, com colchetes, simbolizando uma estrutura conhecida como array, que permite o armazenamento de múltiplos endereços de carteira (por isso jogadores, no plural). O atributo vencedor é do tipo novo, **address payable**, para que a transferência do saldo do bolão seja possível.

O método **construct()**, como o nome sugere, é utilizado no momento da construção e instanciação do contrato, ou seja, é executado uma única vez no momento do seu deploy. O termo **msg.sender** sempre trará o endereço da carteira que chamou o método, ou seja, o remetente da transação. Nesse caso, fica estabelecido que quem publicar o contrato, é seu gerente (nada mais justo.

O “coração” do contrato é o método **entrar()**; observe que ele é do tipo **payable**, ou seja, além dos gastos com o **gas**, um valor deve ser mandado nessa transação (o valor em **wei**, **a décima-oitava casa do ether**, pode ser observado em **msg value**). Para estabelecer certa justiça nas apostas, uma função require() é utilizada para verificar se o valor enviado é de 0,1 ETHER, nem mais, nem menos. Dessa forma, entrar possui um ticket de valor fixo. A remoção dessa linha permitiria enviar absolutamente qualquer valor para o bolão.

O método **descobrirGanhador()** é exclusivo do gerente (observe que ao declarar o método temos a palavra **restricted**, e a regra de restrição é implementada a seguir, por uma estrutura chamada **modifier**, que verifica se **msg.sender == gerente**). O procedimento é usar um método randomico(), implementado mais ao final do contrato, que sorteia o número baseado no número de jogadores, chamando uma função de transferência (transfer()), transferindo todo o saldo do contrato **(address(this).balance)**. Os demais procedimentos “zeram” os atributos de jogadores e vencedor para a “brincadeira” começar novamente.

Para testar o contrato, alguns cuidados devem ser tomados: em primeiro lugar, é necessário criar mais carteiras no Metamask, para que tenhamos múltiplos papéis neste contrato. Para tal, basta clicar no ícone redondo na raposa presente no canto superior direito do Google Chrome, e selecionar “Criar Conta”.

!["Criando novas carteiras no MetaMask"](/images/smartContracts/lab26.png)
<br>| - Criando novas carteiras no MetaMask(Fonte: FIAP(2020))

É aconselhável fazer o procedimento duas vezes, assim, é possível separar bem os papéis: a primeira carteira publica o contrato e fica como gerente, e as contas dois e três são os jogadores. É necessário transferir um valor para essas novas carteiras. Para ter acesso ao endereço da carteira nova, selecione a nova carteira no ícone redondo e clique em cima do endereço que aparece de forma reduzida. Pronto, o endereço da carteira foi copiado para a área de transferência.

!["Criando novas carteiras no Metamask (1)"](/images/smartContracts/lab27.png)
<br>| - Criando novas carteiras no Metamask (1)(Fonte: FIAP(2020))

!["Criando novas carteiras no Metamask (2)"](/images/smartContracts/lab28.png)
<br>| - Criando novas carteiras no Metamask (2)(Fonte: FIAP(2020))

Depois de publicado o contrato pela primeira carteira, selecione a segunda carteira no Metamask e, antes de clicar no botão “entrar” (em vermelho, já que é um método payable), coloque o valor a ser enviado pela transação, 0.1, e a grandeza em ethers (o padrão é wei). Somente aí o botão de entrar pode ser clicado e, após a devida confirmação, este se torna um apostador.

!["Entrando no bolão"](/images/smartContracts/lab29.png)
<br>| - Entrando no bolão(Fonte: FIAP(2020))

O botão getSaldo exibe a quantia que o contrato está custodiando (não estranhe o valor, ele será informado em wei!). Note que, clicar no botão de entrar informando um valor diferente de 0,1 ETH ou clicar no botão “descobrirGanhador” com uma carteira que não seja do gerente resultará em erros, o que significa que as regras de restrição do contrato estão sendo devidamente seguidas.

---

## Outras opções de ambiente de desenvolvimento solidity

O desenvolvimento de Smart Contracts em Remix, embora viável, não é a solução mais robusta para grandes projetos. Trata-se de um contato inicial sem a necessidade de grandes instalações e estruturas, mas pode deixar a desejar conforme os projetos se tornarem mais ambiciosos.

Uma das possibilidades é um framework conhecido como **Truffle**. Além do
compilador **Solidity Compiler**, vários scripts de automação, bibliotecas e outras facilidades são disponibilizadas por ele.

!["Website do framework Truffle"](/images/smartContracts/lab30.png)
<br>| - Website do framework Truffle(Fonte: FIAP(2020))

Para instalá-lo, é necessária a instalação prévia do Nodejs (www.nodejs.org). Somente aí, o npm (node package manager) se torna disponível na linha de comando do Windows (em algumas distribuições Linux, contudo, o npm é uma instalação à parte) e o comando mostrado na Figura “Website do framework Truffle” pode ser usado para instalar o framework.

Realizar todos os testes em redes como a Ropsten, Rinkeby e Kovan podem se tornar um processo lento e sem o controle necessário. Uma boa opção é instalar o Ganache, o chamado “blockchain em um clique”. Fácil de instalar e rodar, permite subir uma plataforma Ethereum local, mais rápida e com fartos recursos em Ether (nada de ficar pedindo na torneira de fauctes).

!["Ganache a blockchain Ethereum em um click"](/images/smartContracts/lab31.png)
<br>| - Ganache a blockchain Ethereum em um click(Fonte: FIAP(2020))

!["Ganache em funcionamento"](/images/smartContracts/lab32.png)
<br>| - Ganache em funcionamento(Fonte: FIAP(2020))

Como pode ser visto nas abas da Figura “Ganache em funcionamento” é possível visualizar informações dos contratos publicados, verificar cada transação da plataforma, entre outros.

O Metamask possui uma opção para configurar uma rede personalizada, conforme pode ser visto na figura “Configurando o Metamask para uma rede personalizada”.

!["Configurando o Metamask para uma rede personalizada"](/images/smartContracts/lab33.png)
<br>| - Configurando o Metamask para uma rede personalizada(Fonte: FIAP(2020))

---

## Conclusão

A tecnologia dos **Smart Contracts** abre uma gama gigantesca de possibilidades de automação e negócio, e este capítulo não tinha a pretensão de formar desenvolvedores de contratos inteligentes em Solidity, mas de ser um pontapé inicial, respondendo às perguntas mais básicas desse procedimento técnico. Esperamos que este capítulo tenha aguçado seu interesse pelo assunto e que seja uma das alternativas de especialização no futuro.

## Referências

ARCADE.CITY. Arcade City WebSite. 2018. Disponível em: <http://arcade.city/>. Acesso em: 11 jun. 2018.

BLOCKCHAIN “Smart Contracts” Will Revolutionize Voting in Elections. 2018. Disponível em: <https://medium.com/@spireProtocol/blockchain-smart-contracts-will-revolutionize-voting-in-elections-acb5abc7beb6>. Acesso em: 17 set. 2020.

BLOCKCHAIN: Honduras 1-France 0? 2015. Disponível em: <https://blockchainfrance.net/2015/09/16/le-honduras-adopte-la-blockchain/>. Acesso em: 11 dez. 2019.

CHANDRAN, R. Modernizing land records in Honduras can help stem violence, says analyst. 2017. Disponível em: <https://www.reuters.com/article/us-honduras-landrights-tech/modernizing-land-records-in-honduras-can-help-stem-violence-says-analyst-idUSKBN1AR151>. Acesso em: 11 dez. 2019.

COINDESK. Ethereum 101. 2019. Disponível em: <https://www.coindesk.com/learn/ethereum-101/what-is-ethereum>. Acesso em: 9 jan. 2020.

DAVID, C. Começou agora a venda e a distribuição para a comunidade do Arcade Token ($ARCD). 2017. Disponível em: <https://blog.arcade.city/come%C3%A7ou-agora-a-venda-e-a-distribui%C3%A7%C3%A3o-para-a-comunidade-do-arcade-token-arcd-eadd9b8f2430>. Acesso em: 17 set. 2020.

EICHMANN, K. Machine Economy – a decentralized future that is enabled by autonomous machine-to-Machine transactions! 2018. Disponível em: <https://medium.com/innogy-innovation-hub/machine-economy-a-decentralized-future-that-is-enabled-by-autonomous-machine-to-machine-e497b90f13c1>. Acesso em: 10 jun. 2018.

EIGHT, E. Spotify CEO Daniel Ek Talks Convincing Taylor Swift to Re-Join Service. 2018. Disponível em: <https://www.rollingstone.com/music/news/spotify-ceo-talks-convincing-taylor-swift-to-re-join-service-w518672>. Acesso em: 17 set. 2020.

GIBBS, S. Uber plans to buy 24,000 autonomous Volvo SUVs in race for driverless future. 2017. Disponível em: <https://www.theguardian.com/technology/2017/nov/20/uber-volvo-suv-self-driving-future-business-ride-hailing-lyft-waymo>. Acesso em: 11 jun. 2018.

GULKER, M. Are Smart Contracts the Future of Fraud Prevention? 2017. Disponível em: <https://www.aier.org/article/are-smart-contracts-future-fraud-prevention>. Acesso em: 17 set. 2020.

JOHNSON, L.; FITZSIMMONS, M. Uber self-driving cars: everything you need to know. 2018. Disponível em: <https://www.techradar.com/news/uber-self-driving-cars>. Acesso em: 17 set. 2020.

KO, T. A guide to developing an Ethereum decentralized voting application. 2018. Disponível em: <https://medium.freecodecamp.org/developing-an-ethereum-decentralized-voting-application-a99de24992d9>. Acesso em: 17 set. 2020.

LEFF, A. Costa Rica: "For Sale," or just a scam? 2011. Disponível em:
<https://www.pri.org/stories/2010-11-23/costa-rica-sale-or-just-scam>. Acesso em: 11 dez. 2019.

MCCORRY, P.; et al. A Smart Contract for Boardroom Voting with Maximum Voter Privacy. 2017. Disponível em: <https://eprint.iacr.org/2017/110.pdf>. Acesso em: 17 set. 2020.

MCINTYRE, H. Why Did Taylor Swift Really Rejoin Spotify? Forbes, 2017. Disponível em: <https://www.forbes.com/sites/hughmcintyre/2017/06/27/why-did-taylor-swift-really-rejoin-spotify/#7fc83189373d>. Acesso em: 17 set. 2020.

MELO, L. Após aporte de US$ 2,1 bi, Uber já vale mais que Ford ou GM. 2016. Disponível em: <https://exame.com/negocios/com-aporte-de-us-2-1-bi-uber-ja-vale-mais-que-ford-ou-gm/#:~:text=Assim%2C%20o%20Uber%20valeria%20mais,%2C2%20bilh%C3%B5es%20de%20d%C3%B3lares).>. Acesso em: 17 set. 2020.

MOLECKE, R. How To Learn Solidity: The Ultimate Ethereum Coding Tutorial. 2017. Disponível em: <https://blockgeeks.com/guides/solidity/>. Acesso em: 9 jan. 2020.

OPENBAZAAR. OpenBazaar Website. 2018. <https://www.openbazaar.org>. Acesso em: 11 jun. 2018.

Disponível em: RASKIN, M. The Law and Legality of Smart Contracts. 2017. Disponível em: <https://www.georgetownlawtechreview.org/the-law-and-legality-of-smart-contracts/GLTR-04-2017/>. Acesso em: 17 set. 2020.

ROSIC, A. What is Ethereum Gas? [The Most Comprehensive Step-By-Step Guide Ever! 2018. Disponível em: <https://blockgeeks.com/guides/ethereum-gas/>. Acesso em: 13 jan. 2020.

SOLIDITY. Solidity v0.7.0. 2020. Disponível <https://solidity.readthedocs.io/en/v0.7.0/>. Acesso em: 17 ago. 2020.

SZABO, N. The Idea of Smart Contracts. 1997. Disponível em: <https://nakamotoinstitute.org/the-idea-of-smart-contracts/ >. Acesso em: 13 jan. 2020.

TAYEB, H. ‘A big step in the right direction’: Settlemint’s founder and CEO on blockchain e-voting. 2016. Disponível em: <https://www.tearsheet.co/funding/a-big-step-in-the-right-direction-settlemints-founder-and-ceo-on-blockchain-e-voting>. Acesso em: 17 set. 2020.

WISTROM, B. Scrutinized by Governments, Austin’s Arcade City Expands Uber Alternative Ride-Hailing Model. 2017. Disponível em:
<https://www.americaninno.com/austin/scrutinized-by-governments-austins-arcade-city-expands-uber-alternative-ride-hailing-model/>. Acesso em: 17 set. 2020.