# Aplicações Blockchain

Embora a aplicação como moeda e sistema financeiro sem intermediários seja a aplicação mais famosa da tecnologia de blockchain, várias outras possibilidades e aplicações podem ser vislumbradas. Ainda que tenha algumas desvantagens tecnológicas, a tecnologia traz várias vantagens, como:

* **Múltiplas cópias de segurança**: Redundância de informações é algo fundamental para evitar perdas de dados e nada tem mais backups do que algo controlado por um blockchain, afinal, cada um dos mineradores e até mesmo outros membros da rede (como o caso dos fullnodes do bitcoin) possuem uma cópia completa, atualizada e integral de todos os blocos e, portanto, todas as informações registradas por ele. Assim sendo, para a informação se perder, todos os nós teriam que ser comprometidos de alguma forma e, sendo assim, quanto mais membros o blockchain tiver, mais segura a informação estará.

* **Registros virtualmente inalteráveis**: o hash que valida um bloco é formado pelas informações registradas em um bloco e hash do bloco anterior, que foi gerado pelos dados dele e seu antecessor, e por aí vai. Assim sendo, as informações em um blockchain são incrementais e acumulativas, armazenadas de forma a não ser alteradas ou apagadas. Embora seja tecnicamente possível alterar ou apagar informações, o esforço exigiria um consenso de toda a rede de mineração para recalcular todos os hash do bloco alterado em diante, o que exigiria muito poder computacional e, portanto, muito investimento financeiro. Além disso, exigiria o consenso de todos os participantes independentes que, em uma rede descentralizada composta por milhares de nós como no caso do bitcoin, é praticamente impossível.

* **Resiliência do sistema**: por se tratar de uma rede P2P (peer-to-peer) e, portanto, sem servidores centrais, ela se mostra extremamente resiliente; um excelente exemplo é o BitTorrent, que trabalha com o mesmo tipo de rede descentralizada. Apesar de ser uma rede de transferência de dados legítima, boa parte dos conteúdos compartilhados detém direitos autorais,  como músicas, séries de TV ou filmes. Por mais de uma década gravadores e estúdios tentam, em vão, proibir estes compartilhamentos, que simplesmente não podem ser contidos; enquanto uma rede P2P possuir pelo menos dois participantes, ela continuará funcionando. O mesmo acontece com o blockchain que, enquanto houver ao menos dois participantes, os blocos continuarão sendo minerados e gerados.

* **Eliminação de intermediários**: por permitir a troca de informações (ou valores) de maneira direta, seu funcionamento elimina a necessidade de intermediários, também conhecido como “terceiro de confiança”; o papel de garantir a legitimidade e validade das informações é feito pelos mineradores, que fazem o papel de “testemunhas” da troca que aconteceu ponto a ponto. A ironia é que os mineradores sequer precisam confiar uns nos outros, basta que todos se submetam as regras estabelecidas pelo sistema que já está em funcionamento. Tais regras incentivam o comportamento honesto, é extremamente mais rentável seguir as regras do que tentar subvertê-las por alguma razão.

Estas características podem ser aproveitadas para dezenas de aplicações diferentes e a seguir falaremos de algumas delas.

---

## Autenticidade dos Documentos

Garantir a autenticidade de documentos é algo custoso, especialmente no Brasil, e ser caro não garante que o processo é à prova de falhas ou fraudes, pois sempre que houver um fator humano que possa ser corrompido e subverter o sistema, a fraude será possível.

A startup brasileira OriginalMy surgiu com uma proposta: registrar documentos em um Blockchain, beneficiando-se de, pelo menos, duas características importantes: o fato de que o registro do documento não possa ser alterado ou removido e a transparência que um blockchain público provê, permitindo a verificação deste registro sem burocracias.

!["Site da OriginalMy.com"](/images/aplicacoesBlockchain/originalMy.png)
<br>| - Site da OriginalMy.com(Fonte: ORIGINALMY(2020))

Documentos oficiais, ideias, patentes, letras de música ou livros podem ser registrados em um blockchain para comprovação de autoria posteriormente, ou seja, ele desempenha um dos papéis de um cartório de registro.

Entretanto, a tecnologia surge sem pedir licença, ela sempre chega antes de eventuais legislações. Garantindo um respaldo judicial, a startup possui um serviço adicional de registro notarial em um cartório tradicional, vislumbrando um futuro em que, talvez, isso não seja mais necessário.

Caso um sistema notarial de algum país fosse implementado integralmente em um único blockchain, além de mitigar fraudes por adulteração ou remoção de informações, todos os documentos poderiam ser verificados e confrontados, evitando a fraude do “vidente que registra sua previsão em cartório”: algumas pessoas fazem dezenas de previsões aleatórias como “prever” celebridades mortas em acidentes aéreos, por exemplo. Ao registrar tais previsões em dezenas de cartórios diferentes (cada previsão em um cartório diferente), quando o previsto se torna um fato, basta apresentar a previsão que “acertou” o acontecimento, desprezando todas as demais.

Fraude semelhante aconteceu na Copa do Mundo de 2014, quando uma conta de Twitter chamada “@fraudefifa” quis provar que a FIFA manipulava os resultados da competição. Curiosa, no entanto, foi a maneira pela qual a conta decidiu “provar” sua tese, realizando postagens com todas as possibilidades de confrontos e vencedores, dias antes das partidas. Quando dois times realmente jogavam e um destes ganhava, bastava remover do Twitter todas as postagens desfavoráveis. Alguém desavisado que se deparasse com as postagens ao final da competição concluiria que realmente a organização manipulava os resultados.

!["O caso de @fraudefifa"](/images/aplicacoesBlockchain/fraudeFifa.png)
<br>| - O caso de @fraudefifa(Fonte: Google Imagens(2020))

Se o Twitter funcionasse baseado em um blockchain, as postagens jamais seriam apagadas e tal fraude não seria possível.

Existem outras iniciativas de autenticação de documentos na Internet, como é o caso do site LexisNexis, que também registra os documentos de maneira a comprovar sua autoria futura.

!["O site de autenticação de documentos lexisnexis.com"](/images/aplicacoesBlockchain/lexisNexis.png)
<br>| - O site de autenticação de documentos lexisnexis.com(Fonte: FIAP(2020))

De acordo com a Legal Architect Camila Rioja Arantes no programa Legal Talks da OriginalMy, já existem ganhos de causas na justiça brasileira da qual as provas estavam registradas em Blockchain (LEGAL TALKS, 2019).

---

## Protegendo direitos autorais e fotográficos

Garantir direitos autorais para seus respectivos autores é um desafio e tanto desde o surgimento da Internet: a facilidade para compartilhamento de dados possibilitou o livre trânsito de textos, fotos e vídeos, muitos deles de forma que seus criadores não fossem remunerados por suas obras.

A situação se torna ainda mais crônica quando falamos em fotografias. A fotografia digital popularizou o compartilhamento de fotos em um patamar jamais atingindo pela humanidade, no entanto, várias destas fotografias que são compartilhadas e utilizadas por vezes de maneira profissional são realizadas por fotógrafos que vivem desta tão importante profissão.

Falando em fotografia digital, a gigante Kodak decidiu não investir na tecnologia em razão da grande receita que a empresa adquiria na revelação de filmes fotográficos tradicionais. No entanto, o restante do mercado disponibilizou a tecnologia que foi adotada massivamente, o que fez a tão tradicional empresa declarar falência em 2012.

A empresa de 140 anos busca se reerguer, procurando um novo “Kodak moment” e parece ter achado uma oportunidade para inovação com criptoativos e o blockchain, propondo o uso destas tecnologias para garantir direitos autorais para fotógrafos.

A ideia é criar uma plataforma de gerenciamento de direitos de imagem da qual os fotógrafos possam registrar seus trabalhos em um blockchain, que impedirá que tal registro seja alterado ou apagado. Desta maneira, o registro da foto em um blockchain poderia comprovar um eventual plágio fotográfico, permitindo identificar o autor da obra com facilidade.

A solução que foi batizada de KodakOne também possibilitará um marketplace para licenciamento o uso da imagem, comprovando o direito de uso da imagem e também garantindo que os royalties cheguem às mãos certas. Para tal, ambas as partes utilizarão um criptoativo chamado de KodakCoin.

A empresa também promete fazer uso de Big Data, Inteligência Artificial e Web Crawling para vasculhar a web verificando o uso devido ou não destas imagens.

!["A plataforma de direitos autorais fotográficos da Kodak"](/images/aplicacoesBlockchain/kodakOne.png)
<br>| - A plataforma de direitos autorais fotográficos da Kodak(Fonte: KODAKONE(2020))

Embora ainda seja apenas uma proposta (e não uma realidade), segundo Randewich (2018), da Reuters, o valor das ações da empresa (Eastman Kodak Co, identificada na Dow Jones como KODK.N) mais do que dobraram quando o anúncio da KodakOne/KodakCoin foi realizado. Resta agora que a centenária empresa entregue o prometido e inove uma vez mais.

Enquanto a Kodak não se move, outras iniciativas começam a surgir. O site Binded.com é uma iniciativa para proteger os direitos fotográficos utilizando Blockchain de maneira simples e rápida.

!["A Plataforma Binded.com"](/images/aplicacoesBlockchain/binded.png)
<br>| - A Plataforma Binded.com(Fonte: FIAP(2020))

---

## Registros Imobiliários

Os custos da intermediação da compra e venda de imóveis são elevadíssimos, qualquer um que fez a compra ou venda de um deles no Brasil pode comprovar esta afirmação. Entretanto, dado ao alto investimento da transação, a responsabilidade do intermediador do processo é altíssima, uma vez que o risco de fraude cresce com o valor envolvido.

Existem muitos países que possuem um sistema de registro imobiliário muito frágil e a vida de milhares de famílias é arruinada por fraudes imobiliárias, que podem ir desde a falsificação de registros, imóveis vendidos para múltiplos compradores e até funcionários corruptos que fraudam registros ao fazê-los de forma retroativa. A Costa Rica é um dos países da América Central que mais sofrem com fraudes imobiliárias, embora não seja o único.

Ao falarmos dos criptoativos como o Bitcoin, lembramos que o blockchain impede que sejam forjados, não possam ser gastos duas vezes pela mesma pessoa e suas transferências são irreversíveis e fáceis de serem verificadas e auditadas. Por que isso não pode ser feito com registros imobiliários? 
Observe uma escritura ou registro de um imóvel que tenha tido vários proprietários diferentes. Ele já é um “blockchain” por si só, pois cada uma das transações é registrar de forma cronológica e incremental. Nenhuma das informações deve ser apagada.

Um blockchain único utilizado por todas as partes que realizem registros imobiliários em um país tornaria este processo muito mais seguro e verificável do que é hoje e os custos para tal poderiam ser drasticamente diminuídos.

A empresa Ubitquity criou o primeiro blockchain com esta finalidade, a de realizar registros imobiliários de maneira segura.

!["Ubitquity, o primeiro blockchain para registros imobiliários"](/images/aplicacoesBlockchain/ubitquity.png)
<br>| - Ubitquity, o primeiro blockchain para registros imobiliários(Fonte: UBITQUITY(2020))

Segundo Keirns (2017), as cidades de Pelotas e Morro Redondo no estado do Rio Grande do Sul estão servindo de piloto para registros imobiliários utilizando blockchain. O fundador da Ubitquity informa que o primeiro registro imobiliário usando a plataforma foi realizado por um médico residente em Pelotas, no 30 de março de 2017.

Outros pilotos têm sido realizados por outras startups em outros países, como a startup ChromaWay na Suécia. Esperamos que os pilotos sejam bem-sucedidos e que os benefícios desta tecnologia transformem positivamente a vida das pessoas em um dos seus momentos mais importantes: a aquisição de um imóvel, com todas as promessas e sonhos que este momento representa.

---

## Alternativa ao Seguro tradicional

Produtos disponibilizados por seguradoras costumam ser caros e pouco inclusivos, por diversas razões. Entre elas, o grande número de assaltos, furtos, acidentes e fraudes envolvendo os bens assegurados, tornando tais produtos indisponíveis para algumas pessoas.

Um conceito que vem ganhando terreno é o da proteção compartilhada: grupos de pessoas são criados para assegurar seus bens, quando um evento que compromete este bem acontece, o membro recorre ao seu grupo de ajuda mútua, que decide pelo ressarcimento (ou não) de seu membro.

Entretanto, administrar o funcionamento de um grupo de ajuda mútua não é tarefa simples. Quais são as regras, como os eventos serão registrados e votados? Onde fica ou com quem fica o dinheiro deste fundo de emergência?

A startup brasileira Mutual.Life é uma insurtech que propõe gerenciar os problemas que surgem na implementação de um grupo de ajuda mútua. Para tal, emprega a tecnologia de blockchain e inteligência artificial para garantir a segurança os valores e transparência dos processos envolvidos.

!["A startup brasileira de grupos de ajuda mútua Mutual.Life"](/images/aplicacoesBlockchain/mutualLife.png)
<br>| - A startup brasileira de grupos de ajuda mútua Mutual.Life(Fonte: MUTUAL.LIFE(2020))

De acordo com Fabricio Vargas Matos, cofundador e CTO da Mutual.Life, a empresa promove o chamado “seguro peer-to-peer”, uma vez que o membro do grupo atua como seguradora e assegurado ao mesmo tempo. Assim como acontece com criptoativos, a falta de regulação pode ser um obstáculo em busca de respaldo jurídico aos membros e, segundo Matos (2017), a Superintendência de Seguros Privados − SUSEP (órgão regulador do setor de seguros no Brasil) promete estudar o “seguro peer-to-peer” em uma agenda de curto prazo, prometendo regular apenas o que for necessário e se necessário, uma vez que o excesso de regulamentação geralmente representa um obstáculo à inovação.

---

## Maior segurança na cadeia logística

Uma das grandes aplicações do blockchain é para a cadeia logística de suprimentos. Entre outros riscos, há a possibilidade do bem ser falsificado ou extraviado. Quais as garantias de que o suprimento chegou a uma determinada unidade de distribuição ou que alguns passos do itinerário tenham sido removidos para facilitar o extravio ou falsificação?

A empresa Blockverify faz uso do Blockchain para registrar a movimentação de produtos de alto valor (como bolsas de grife, diamantes, entre outros produtos) em um blockchain, desta forma, o itinerário dos bens não pode ser alterado ou mesmo apagado. Além disso, a empresa se utiliza de IoT, utilizando RFid para registrar os itens unicamente, de forma a evitar falsificações. As tags também permitem registrar a movimentação do item automaticamente, tornando o processo logístico mais eficiente e rápido, mitigando as possíveis fraudes no processo.

!["Blockverify, blockchain para segurança em cadeia logística"](/images/aplicacoesBlockchain/blockverify.png)
<br>| - Blockverify, blockchain para segurança em cadeia logística(Fonte: BLOCKVERIFY(2020))

---

## Carrefour e a primeira cadeia de alimentos em Blockchain

Em 2018, pela primeira vez, na França, o Carrefour usou a tecnologia blockchain com uma de suas linhas icônicas de produtos animais: o frango Carrefour Quality Line Auvergne, do qual um milhão é vendido todos os anos, um marco importante para seu plano de transformação chamado Carrefour 2022.

A tecnologia blockchain já é utilizada para frangos de linha livre do Carrefour Quality Line Auvergne e será utilizado em mais oito linhas de produtos de origem animal e vegetal, como ovos, queijo, leite, laranja, tomate, salmão e bife moído. Um sistema inovador projetado garante aos consumidores uma completa rastreabilidade do produto (CARREFOUR, 2018).

Pode ser usado no setor de alimentos para que cada uma das partes ao longo da cadeia de fornecimento (produtores, processadores e distribuidores) possa fornecer informações de rastreabilidade sobre seu papel específico e para cada lote (datas, locais, prédios agrícolas, canais de distribuição), tratamentos potenciais, etc.

O rótulo de cada produto contará com um QR Code que os consumidores poderão escanear usando seus smartphones. Isso fornecerá informações sobre o produto e a jornada que ele tomou − desde onde foi criado até quando foi colocado nas prateleiras. Por exemplo: para o frango de linha livre do Carrefour Quality Line Auvergne, os consumidores poderão descobrir onde e como cada animal foi criado, o nome do agricultor, que alimento foi usado (se as aves foram ou não alimentadas com cereais franceses e soja, produtos livres de transgênicos, etc.), quais tratamentos foram usados (antibióticos-free, etc.), quaisquer rótulos de qualidade, onde foram abatidas etc. (CARREFOUR, 2018).

!["Carrefour Quality Line Auvergne"](/images/aplicacoesBlockchain/carrefour.png)
<br>| - Carrefour Quality Line Auvergne(Fonte: CARREFOUR(2020))

---

## Aplicações em Smart Contracts

Graças a esta importante tecnologia, novas aplicações se tornaram possíveis. Veremos a seguir alguns dos exemplos mais relevantes usando contratos inteligentes.

---

## OpenBazaar, o Ml sem o ML

Uma das aplicações em funcionamento que elimina intermediários é o OpenBazaar, uma plataforma de comércio eletrônico P2P, ligando compradores e vendedores diretamente. Por não haver intermediários, não há taxas ou restrições para seu uso.

!["Logo OpenBazaar"](/images/aplicacoesBlockchain/openbazar.png)
<br>| - Logo OpenBazaar(Fonte: OPENBAZAAR(2020))

Por funcionar em uma rede descentralizada, as informações dos anúncios e das transações realizadas não ficam em servidores centrais ou sites, funcionando em uma rede similar à rede Onion, do navegador Tor. Para acessar o marketplace, existe um navegador web capaz de acessar os anúncios e, para comodidade, possui uma carteira de criptoativos embutida, para realizar os pagamentos em Bitcoin, Bitcoin Cash ou Zcash (o vendedor escolher em qual criptoativo que receber).

!["Logo OpenBazaar"](/images/aplicacoesBlockchain/produtosOpenbazar.png)
<br>| - Logo OpenBazaar(Fonte: OPENBAZAAR(2020))

Quando acontece uma venda, é estabelecido um contrato inteligente entre comprador e vendedor para a garantia das partes envolvidas. O sistema permite o rankeamento de seus membros e qualificar vendedores após as compras, como em qualquer e-commerce que estejamos acostumados a comprar. O OpenBazaar não é uma empresa, é uma comunidade de software livre promovendo a inovação na forma que contratamos produtos pela Internet.

---

## Arcade.city, o uber sem o uber

O Uber é um grande exemplo de uma nova economia, baseada em Sharing Economy. Além disso, é uma startup Data-driven, ou “guiada por dados”, afinal, seu maior valor é se utilizar de tecnologias como Big Data e Inteligência Artificial para gerar valor. Se há alguma dúvida, saiba que é uma empresa que não tem bens físicos significativos ou uma frota de carros, no entanto, segundo Melo (2016), com apenas 7 anos de existência seu valor de mercado superava a das gigantes e centenárias Ford e GM. 

Entretanto, a parte da “empresa sem uma frota de carros” está prestes a mudar. Segundo GIBBS (2017) para o jornal The Guardian, o Uber planejava comprar 24 mil veículos autônomos da Volvo ao final de 2017 e em meados de 2018 a empresa já possuía mais de uma centena de carros em testes nas ruas de cidades nos Estados Unidos e Canadá (JOHNSON & FITZSIMMONS, 2018).

!["Ford Fusion autônomo da Uber em testes nas ruas da Pittsburgh"](/images/aplicacoesBlockchain/uber.png)
<br>| - Ford Fusion autônomo da Uber em testes nas ruas da Pittsburgh(Fonte: JOHNSON e FITZSIMMONS(2018))

Sendo assim, podemos concluir que, cedo ou tarde, a empresa vai retirar o motorista da equação, embora este seja hoje uma parte importante de seu modelo de negócio. Pode levar algumas décadas, especialmente em países como o Brasil, mas acontecerá.

Contratos inteligentes permitem a eliminação de intermediários e um grupo de motoristas em Austin, Texas, resolveu fazer o contrário: tirar o Uber da equação.

O Arcade.City é a primeira iniciativa bem-sucedida de uma rede de viagens P2P, ou seja, motoristas e passageiros são conectados ponto a ponto. A iniciativa em Austin já está em funcionamento há dois anos, prestando o serviço de deslocamento seguro sem incidentes (DAVID, 2017). Em 2017, a cidade contava com mais de 150 motoristas ligados à rede de viagens (WISTROM, 2017).

!["Aplicativo de Smart Mobility Arcade City"](/images/aplicacoesBlockchain/arcadeCity.png)
<br>| - Aplicativo de Smart Mobility Arcade City(Fonte: ARCADE.CITY(2020))

Algumas experiências em outras cidades e países, como é o caso do Rio de Janeiro, já foram realizadas. O serviço realizou um ICO de seu Arcade Token recentemente, com o intuito de custear o desenvolvimento de um aplicativo mobile que possa ser utilizado em qualquer país e cumpra as regras que foram estabelecidas no whitepaper.

---

## Musicoin, direitos autorais fonográficos

A indústria musical sofreu várias revoluções ao longo das décadas: desde o fonógrafo que gravou a primeira voz humana criado por Thomas Edson, passando pelo walkman da Sony, os CDs, o iTunes e finalmente no modelo vigente, os streamings, do qual temos como referência o Spotify e, no caso do audiovisual, a Netflix. Entretanto, estas novas gigantes por vezes acabam ditando “suas regras para o mercado” e, assim, vários artistas acabaram declarando guerra ao Spotify e ao Apple Music (como a Taylor Swift no passado), queixando-se do baixo valor de repasse destes grandes serviços.

Outro fator a ser levantado são os números apresentados pelos serviços, afinal, quando o Spotify diz ao artista que sua música foi executada X milhões de vezes e, por esta razão ele vai receber Y, pergunta-se até onde estes números correspondem à realidade, afinal, são estes mesmos serviços que realizam estas apurações. Se eu não confirmar no intermediário, nada feito.

Se o blockchain e os smart contracts têm o poder de eliminar intermediários, seria possível pensar em um modelo de streaming de áudio sem o Spotify? É aí que entra o Musicoin.

!["Logo do Musicoin"](/images/aplicacoesBlockchain/musicoin.png)
<br>| - Logo do Musicoin(Fonte: MUSICOIN(2020))

O Musicoin propõe um modelo de remuneração ao artista baseado em um contrato PPP (pay-per-play, ou pagamento por execução), ou seja, toda vez que uma música for executada um valor será enviado para a remuneração dos artistas, o contrato autogerenciável já faz a divisão financeira automaticamente. No exemplo da Figura “Funcionamento do Musicoin”, temos o guitarrista que recebe 1/4 do valor, o baterista recebendo outro 1/4 e o cantor e compositor da música, os 2/4 restantes.

!["Funcionamento do Musicoin"](/images/aplicacoesBlockchain/musicoin2.png)
<br>| - Funcionamento do Musicoin(Fonte: MUSICOIN(2020))

Cada música teria o seu próprio contrato com uma distribuição diferente, ou seja, em outra música do mesmo “álbum” temos outra pessoa como compositor da letra recebendo 10%, um produtor recebendo 15% e assim por diante.

Os ouvintes não precisam necessariamente pagar por execução, embora os artistas sejam remunerados desta maneira. Em seu modelo de negócio, existe um criptoativo que é minerado, conhecido como Musicoin (MUSIC), e 15% da recompensa pela mineração vai para um fundo chamado de Universal Basic Income (UBI). Quando ouvimos uma música gratuitamente no serviço de streaming do Musicoin é a partir deste fundo que o artista é remunerado. Além disso, ouvintes podem comprar Musicoins (ou $MUSIC) e dar tips (gorjetas) para seus artistas favoritos, que são remunerados nestes dois casos pelos contratos PPP.

---

## Smart Governance, votação 2.0

    “Em essência, um blockchain é compartilhado, programável, criptograficamenteseguro e tornando-se, portanto, um livro-razão confiável que nenhum usuáriocontrola e que pode ser inspecionado por qualquer pessoa” (SCHWAB apud KO,2018, tradução minha)

Há sempre suspeitas de fraude em qualquer eleição realizada em qualquer nação do mundo; há muita coisa em jogo e seus vencedores têm acesso a altos valores e muito, muito poder. Assim sendo, sistemas de votação sempre levantarão suspeitas, especialmente de seus perdedores.

Existem várias propostas do uso de smart contracts para sistemas de votação inteligentes, afinal, suas propriedades de imutabilidade sem que haja controle por nenhuma das partes tornam as eleições uma aplicação perfeita para a tecnologia.

!["Votações inteligentes usando Smart Contracts"](/images/aplicacoesBlockchain/smartContracts.png)
<br>| - Votações inteligentes usando Smart Contracts(Fonte: TAYEB(2016))

McCorry e colaboradores (2017) relatam terem implementado o conceito na rede Ethereum, chamando sua implementação de Open Vote Network:

    Apresentamos a primeira implementação de uma abordagem descentralizada e protocolo de voto pela internet com máxima privacidade dos eleitores usando o Blockchain. A Open Vote Network (Rede de Votação Aberta) é adequada para as eleições de diretoria e está escrito como um contrato inteligente para a Ethereum. Ao contrário de protocolos de e-votação Blockchain propostos anteriormente, esta é a primeira implementação que não depende de qualquer autoridade confiável para calcular o registro ou proteger a privacidade do eleitor. Em vez disso, a Open Vote Network (Rede de Voto Aberto) é um protocolo auto-organizado, e cada eleitor está no controle da privacidade de seu próprio voto de tal forma que só pode ser violado por uma colusão completa envolvendo todos os outros eleitores. A execução do protocolo é aplicada usando o mecanismo que também protege o blockchain da rede Ethereum. Nós testamos a implementação na rede oficial de testes da Ethereum para demonstrar sua viabilidade. (MCCORRY et al, 2017, tradução minha).

Além de garantir a privacidade, o contrato traz transparência ao processo de
apuração pois, ao verificar as condições para as quais os votos foram apurados, é
possível garantir que 1 pessoa = 1 voto. Ao utilizar um blockchain como infraestrutura
para que o sistema de votação seja realizado, reduzem-se drasticamente quaisquer
fraudes que possam hoje ser realizadas em sistemas eleitorais tradicionais.   

---

## DAPP

Utilizamos aplicativos de smartphones o tempo todo, para as mais diferentes necessidades. A criação de contratos inteligentes trouxe consigo uma nova proposta de arquitetura para aplicações, chamada de DAPP.

DAPP significa decentralized application, ou aplicações descentralizadas. Em DAPP, as aplicações possuem parte de sua programação em frontend (instalados nos smartphones, como geralmente o são), mas a programação mais pesada, conhecida como backend, roda em um blockchain em uma rede descentralizada P2P. Desta forma, as DAPPs se tornam verdadeiras aplicações compartilhadas não sendo possível, nem aos próprios desenvolvedores, modificar condições e regras já estabelecidas.

!["Arquitetura de DAPP, uma aplicação descentralizada"](/images/aplicacoesBlockchain/dapp.png)
<br>| - Arquitetura de DAPP, uma aplicação descentralizada(Fonte: TAYEB(2016))

Embora seja algo recente, o site State of the Dapps (https://www.stateofthedapps.com/) já traz mais de mil e seiscentas aplicações descentralizadas.

---

## DAO e as Smart Nations

Imagine o seguinte cenário: em um congresso internacional, você conhece outras duas pessoas fantásticas, surge uma grande afinidade e, juntos, vocês têm uma ideia para uma solução que vai revolucionar o mundo. Vocês resolvem empreender juntos, mas existe um grande entrave: enquanto você reside no Brasil, seus futuros sócios moram na Alemanha e Índia, respectivamente. Estão todos muito interessados em empreender juntos, comprometidos com a ideia e apaixonados, no entanto, cada um está muito bem estabelecido em seu país de origem e vocês não estão interessados em mudar de país.

Qual a solução neste caso? Abrir três empresas (que na prática é apenas uma), uma em cada país? Em um eventual processo judicial, qual o foro escolhido? Como criar uma estrutura que garanta respaldo para cada uma das partes?

Uma das alternativas é criar uma DAO (Decentralized autonomous organization ou Organização Autônoma Descentralizada), em que as regras e os processos da empresa sejam codificados em contratos inteligentes.

!["Proposta de Arquitetura de uma DAO"](/images/aplicacoesBlockchain/dao.png)
<br>| - Proposta de Arquitetura de uma DAO(Fonte: BLOCKCHAINHUB(s.d))

E o que seria uma nação, senão um conjunto de leis, deveres e direitos que seus cidadãos dentro de suas fronteiras precisam seguir? Se pensarmos em como a Internet tornou nossa comunicação tão veloz e nossas fronteiras geopolíticas praticamente irrelevantes em várias atividades modernas, como consumir entretenimento, fazer compras e até mesmo negócios, talvez o nosso conceito de nação precise ser revisto.

O conceito de DAO pode ser expandido para as Smart Nations, ou nações inteligentes. Algumas pessoas – especialmente libertários – começam a se organizar em nações virtuais, ou seja, teríamos as nações físicas (com suas fronteiras geopolíticas) e verdadeiras nações “lógicas”, em que as pessoas escolhem se organizar de maneira diferente, escolhendo assim o conjunto de regras que deseja seguir.

---

## Conclusão

Os blockchains e smart contracts são tecnologias em ascensão. Enquanto os ativos digitais são usados por uma parcela muito pequena da população mundial, a adoção do blockchain é inicial em outros campos e ainda faltam exemplos de grandes cases de uso da tecnologia.

No entanto, trata-se de algo que sequer completou dez anos de existência. A cada dia que se passa, novas iniciativas são anunciadas e muitas delas prometem revolucionar os mercados nos quais estão inseridas. Não deixe de acompanhar esta tecnologia que será uma das forças mais transformadoras da próxima década.

---

## Referências

ANTONOPOULOS, Andreas. Mastering Bitcoin: Unlocking Digital Cryptocurrencies. Sebastopol: O’Reilly Media, 2016.

BLOCKVERIFY. Blockverify Website. 2018. Disponível em: <http://www.blockverify.io/>. Acesso em: 22 jul. 2020.

CARREFOUR. Carrefour launches Europe's first food blockchain. 2018. Disponível em: <http://www.carrefour.com/current-news/carrefour-launches-europes-first-food-blockchain>. Acesso em: 22 jul. 2020.

EICHMANN, Kerstin. Machine Economy — a decentralized future that is enabled by autonomous machine-to-Machine transactions! 2018. Disponível em: <https://medium.com/innogy-innovation-hub/machine-economy-a-decentralized-future-that-is-enabled-by-autonomous-machine-to-machine-e497b90f13c1>. Acesso em: 22 jul. 2020.

KEIRNS, Garrett. Blockchain Land Registry Tech Gets Test in Brazil. 2017. Disponível em: <https://www.coindesk.com/blockchain-land-registry-tech-gets-test-brazil/>. Acesso 22 jul. 2020.

KODAKONE. KodakOne Website. 2018. Disponível em: <https://kodakone.com/>. Acesso em: 22 jul. 2020.

LEGAL TALKS. LegalTalk #:6 Camila Rioja | Novas tendências do mercado jurídico. 2019. Disponível em: <https://www.youtube.com/watch?v=qCeMLTK6ncM>. Acesso em: 22 jul. 2020.

MATOS, Fabrício Vargas. A regulação é realmente um gargalo para asinsurtechs? 2017. Disponível em: <https://mutual.life/br/blog/a-regulacao-e-realmente-um-gargalo-para-as-insurtechs>. Acesso em: 22 jul. 2020.

MUTUAL.LIFE. Mutual.Life WebSite. 2018. Disponível em: <https://mutual.life/>. Acesso em: 22 jul. 2020.

ORIGINALMY.COM. OriginalMy.com Website. 2018. Disponível em: <https://originalmy.com/>. Acesso em: 22 jul. 2020. 

POPPER, Nathaniel. Digital Gold: Bitcoin and the Inside Story of the Misfits and
Millionaires Trying to Reinvent Money. Nova York: Harper Paperbacks, 2016.

RANDEWICH, Noel. Eastman Kodak unveils cryptocurrency, stock doubles. 2018. Disponível em: <https://www.reuters.com/article/us-eastman-kodak-stocks/eastman-kodak-unveils-cryptocurrency-stock-doubles-idUSKBN1EY2AD>. Acesso em: 22 jul. 2020.

UBITQUITY. Ubitquity Website. 2018. Disponível em: <https://www.ubitquity.io>. Acesso 22 jul. 2020.