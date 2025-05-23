# Bem vindo ao repositório de grades de programação de canais de TV brasileiros 🇧🇷

Utilizando-se na sua totalidade de recursos e soluções próprias eu coleto, organizo e crio arquivos XML com a grade de programação de canais abertos, pagos, streaming e FAST. E agora eu compartilho aqui para quem quiser ou precisar.
Serão duas atualizações por dia. Uma entre 11h30 e 12h00 e outra entre 23h30 e 00h00. Sempre no horário de Brasília.



Você vai encontrar 7 arquivos diferentes e aqui eu vou te explicar o que cada um tem para você escolher o melhor (ou usar todos também, por que não?):

### <b>band.xml</b>
Pra começar, trazemos as grades de programção de diversas Bands pelo Brasil. Aqui você vai achar: Band São Paulo, Band Aracaju, Band Bahia, Band Brasília, Band Mais (Campinas/Sorocaba), Band Ceará, Band Imperatriz, Band Maceió, Band Maranhão, Band Minas, Band Paraná, Band Paulista, Band Piauí, Band RN, Band RS, Band Rio, Band Tocantins, Band Triângulo e Band Vale 👀.

### <b>claro.xml</b>
Aqui você tem a grade de praticamente de todos os canais disponíveis no Claro TV+. Se você não achar, é porque a Claro não quis compartilhar 😔.

### <b>epg.xml</b>
Esse daqui é uma seleção feita por mim e pra mim (mas vai que te interessa). Tem em sua maioria canais esportivos, mas é uma seleção pegando o melhor de cada fonte 🥗.

### <b>globo-internacional.xml</b>
Vai que você não gosta da Globo do Brasil mesmo, então aqui tem a grade da Globo Internacional do EUA 🇺🇸.

### <b>globo.xml</b>
Nesse você acha todos os canais lineares e FAST disponíveis no Globoplay. Se tem lá, tem aqui 🌐!

### <b>maissbt.xml</b>
Você encontra a grade de programação de todos os canais FAST do +SBT 🚨.

### <b>vivoplay.xml</b>
Esse é perfeito pra você que é Fora Globo das ideias. A Vivo até tem os canais Globo, mas carrega quase nenhum dado de EPG. De resto, tem todo o resto ⛄.

## Como configurar no DVBViewer?

Para fazer a configuração você precisará de um programa chamado [XEPG](http://www.a123.dk/). Após instalar, você vai seguir os passos a seguir:

#### Entendendo o programa

![Janela principal do programa XEPG. O programa está com os campos e botões ordenados de 1 a 5 para facilitar o uso e configuração](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo1.png?raw=true)

O programa tenta ser intuitivo, quase tudo está ordenado e você deve seguir essa ordem.

##### 1) XMLTV EPG Job(s)
Essa é a lista de fontes de dados. Cada fonte que você adicionat ficará listada aqui. Logo abaixo você tem os botões para adicionar, editar e apagar um item selecionado dessa lista.

##### 2) Channel Pairing
Aqui é o botão que você vai apertar quando tudo tiver configurado. Apesar dele estar como o passo 2, será o terceiro passo desta configuração. 

##### 3) Options
É o local para configurar a conexão com o DVBViewer e com o DVBViewer Media Server, caso tenha ele. Na página do desenvolvedor há explicações de como configurar tudo direito aqui se for necessário.

##### 4) Test Import
Se tudo foi feito de modo certo, é aqui que você vai apertar para ver se os dados serão importados corretamente no DVBViewer.

##### 5) Automate
E depois de configurar tudo, aqui você configura para que tudo isso seja feito automaticamente. O passo-a-passo para isso estará na janela que se abrirá após apertar este botão.


#### Começando a configurar
Você vai clicar no botão <b>Add</b> para abrir a janela a seguir. Inicialmente apenas os dois primeiros campos serão usados.

![Janela oara inserção da URL do XML e local que ele está salvo](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo2.png?raw=true)

##### XMLTV TV Data File

![Página do globo-internacional.xml neste repositório](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo3.png?raw=true)

Para a primeira configuração de cada novo xml você precisa baixa-lo manualmente. Ao lado de <i>Raw</i> tem o botão para download, clique nele e salve em <b>C:\ProgramData\Xepg</b>. Depois clique no <b>...</b> (sim, é um botão com reticências) e selecione o arquivo que você acabou de baixar e salvar.

![Diretório C:\ProgramData\Xepg](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo5.png?raw=true)

##### Grabber executable/URL
Nesse campo você vai adicionar o link que leva ao XML que acabou de baixar. Na página dele, você vai clicar em <b>Raw</b> e pegar a URL.

![Página raw do globo-internacional.xml neste repositório](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo4.png?raw=true)

E assim deve ficar. Repare que o link que você pegou deve iniciar com <b>http://</b>, então cuide para garantir isso.
![Janela oara inserção da URL do XML e local que ele está salvo preenchida corretamente](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo6.png?raw=true)

Com tudo configurado, aperte <b>Ok</b>. 

#### Run Grabber(s)

![Janela principal do programa XEPG. O programa está com os campos e botões ordenados de 1 a 5 para facilitar o uso e configuração](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo1.png?raw=true)

Voltando para a janela principal, tem um botão que não comentei sobre e é o <b>Run Grabber(s)</b>. Ele é o responsavel por baixar os dados atualizados daqui do GitHub e atualizar o xml no seu computador. Sabendo disso, você vai clicar nele e, após a execução, deve receber um resultado muito parecido com este:

![Execução bem-sucedida após clicar em Run Grabber(s)](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo7.png?raw=true)

#### Channel Pairing

Aqui é onde você vai ligar os dados baixados com os canais salvos no DVBViewer.

![Execução bem-sucedida após clicar em Channel Pairing](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo8.png?raw=true)

Antes de abrir a lista para a seleção, você tem que ter uma mensagem parecida com essa da imagem acima

![Lista de canais do channel pairing](https://raw.githubusercontent.com/limaalef/BrazilTVEPG/main/howtoinstall/passo9.png?raw=true)

Na coluna da esquerda estão os canais disponiveis no XML e na coluna da direita estão os canais salvos no seu DVBViewer. Depois de selecionar as ligações ao seu modo, aperte <b>Ok</b> e em seguida aperte <b>Test Import</b>.

#### Test Import

Se tudo deu certo, os dados já devem aparecer no guia de programação do DVBViewer. Se não precisar mudar mais nada, você vai clicar em <b>Automate</b> e seguir os passos para automatizar a atualização dos dados.
