# Como a Internet Funciona

Nota: Sendo criada nos Estados Unidos por volta de 1969 (em meio a Guerra Fria), a Internet, chamada na época de Arpanet, tinha como função interligar laboratórios de pesquisa durante a guerra, caso os meios de comunicação tradicionais fossem destruídos em ataques russos às bases militares.

# Representação de Dados

- Ao contrário do que muitos pensam, o **computador não é um dispositivo super inteligente**, capaz de realizar tudo e pensar por si próprio (pelo menos não ainda), antes disso, o mesmo representa uma **máquina capaz de analizar sinais e fazer contas simples de maneira super rápida**. Resumindo bastante, o computador compreende somente duas coisas: **Zeros** e **Uns**.

- Na prática, o que circula dentro de um computador não são vários **Zeros** e **Uns.** Por se tratar de um **equipamento eletrônico**, o computador funciona por meio de **sinais** (**ondas**). Ou seja, o computador lê ****sinais elétricos na sua forma mais simples: com corrente (1) ou sem corrente (0). Estes sinais são representados como **Ondas Quadradas**, também chamados de **Ondas Digitais**:

![DigitalWaveform.png](Como%20a%20Internet%20Funciona%20bfc81b15694343dabfe46d106344a199/DigitalWaveform.png)

- Na computação, estes valores de **Zeros** e **Uns** são chamados de **Digitos Binários** (**Binary Digits**), ou de forma simplificada: **Bits**. Estes **Bits** são agrupados em **conjuntos de 8**, que também recebem um nome especial: **Bytes**, que por sua vez, são agrupados em **conjuntos de 1024**, e assim por diante:
    
    
    - **1 byte (B)** = 8 bits
    - **1 kilobyte (KB)** = 1024 bytes
    - **1 megabyte (MB)** = 1024 kilobytes
    - **1 gigabyte (GB)** = 1024 megabytes
    - **1 terabyte (TB)** = 1024 gigabytes
    - **1 petabyte (PB)** = 1024 terabytes
    - **1 exabyte (EB)** = 1024 petabytes
    - **1 zettabyte (ZB)** = 1024 exabytes
    - **1 yottabyte (YB)** = 1024 zettabytes

<aside>
🚫 **Bits** e **Bytes** (assim como seus múltiplos) são **unidades de medida que contam quantidades de informação**. Tomando por exemplo o múltiplo **‘Mega’**, um Megabit (Mb) é mais usado para medir **velocidades de transmissão**, em quanto um Megabyte (MB), assim como **Gigabyte** e **Terabyte**, são mais relacionados à **capacidade de armazenamento**.

</aside>

---

# Conversão dos Sinais

- Como foi visto anteriormente, o computador funciona por meio de **Ondas Digitais/Quadradas**, sinais que são diferentes das **Ondas Analógicas/Senoidais** (entendidas pelos sistemas analógicos como linhas telefônicas). Essa diferença entre os tipos de sinais **dificulta a comunicação** entre **Cliente** e **Servidor**, por conta disso, é necessário que ocorra uma “conversão”, mais conhecida como **Modulação**.

![sinal-analogico-vs-digital.jpg](Como%20a%20Internet%20Funciona%20bfc81b15694343dabfe46d106344a199/sinal-analogico-vs-digital.jpg)

- Essa **“converção”** de sinais ocorre por intermédio de um aparelho conhecido como **Modem**, que possui esse nome pois realiza a Modulação dos sinais que saem do computador e a Demodulação dos sinais que chegam ao mesmo.

<aside>
🚫 Aprofundando um pouco mais o estudo de **redes de comunicação**, veremos que a função **Modem** desses aparelhos é apenas uma das características do produto. Na verdade, este dispositivo é um **Gateway**, que irá se ligar aos **Roteadores** do provedor de acesso.

</aside>

---

# Ligação entre Clientes e Servidores

- Imagine que você tenta **acessar um site por meio de um computador**, nesse cenário, seu computador representa um **Cliente**, pois o mesmo **solicita um serviço** (que no caso é o acesso à um site), ao descobrir onde está o site, a máquina que está hospedando ele será o **Servidor**, que irá **fornecer os arquivos que compõem o site**. O caminho que vai criar uma ligação entre o **Servidor** e o **Cliente** será decidido pelos **Roteadores da Internet**.

- Por questões de segurança, existem alguns processos entre a **Requisição** (**Request**) ****de um serviço e sua **Resposta** (**Response**). Antes de mais nada, é necessário entendermos um conceito de suma importância, no que diz respeito à identificação de cada ponto conectado à rede.

![cliente e server.png](Como%20a%20Internet%20Funciona%20bfc81b15694343dabfe46d106344a199/cliente_e_server.png)

- A Internet funciona baseada em um **conjunto de protocolos** chamado **TCP/IP**: ***T**ransmission **C**ontrol **P**rotocol* e ***I**nternet **P**rotocol *****(**Protocolo de Controle de Transmissão** e **Protocolo de Internet**). Um protocolo garante que **todas as comunicações seguirão um mesmo padrão**, permitindo que dispositivos diferentes, com tecnologias completamente distintas, **possam se comunicar**.

 

- Uma das funções do **TCP/IP**, mais especificamente do **IP**, é **identificar cada ponto que está conectado à rede**, quando alguém **“se conecta”** à **Internet**, este recebe uma **identificação única**. Essa identificação é chamada **Endereço IP**. Pense assim: o **Endereço IP** é como o **número de telefone atribuído ao seu smartphone**. **TCP** é toda a **tecnologia que faz o telefone tocar** e **permite conversar com alguém em outro telefone**.

<aside>
🚫 **IPv4** e **IPv6** representam o **Protocolo de Internet Versão 4** e o **Protocolo de Internet Versão 6**, respectivamente. o **IPv6** é a **nova versão do protocolo de Internet**, que é muito melhor que o **IPv4** em termos de complexidade e eficiência (os **IPv6** utilizam **128 bits** ao todo, o que representa **4x mais bits que seu antecessor**).

</aside>

---

# Acesso aos Servidores

- Uma vez sabendo como os pontos são identificados, vamos propor o seguinte cenário: você se encontra no **Ponto A**, tentando acessar um site que está guardado no servidor (representado pelo **Ponto D**). Vale ressaltar que tanto você quanto o **Ponto D** possuem **Endereços IPs**. Agora imagine que para acessar um site, você precisasse decorar seu **Endereço IP**, certamente isso dificultaria todo o processo, certo?

![Top 10 exemplos.png](Como%20a%20Internet%20Funciona%20bfc81b15694343dabfe46d106344a199/Top_10_exemplos.png)

- É a fim de resolver esse tipo de problema que existem os **Servidores DNS**: ***D**omain **N**ame **S**ystem* (**Sistema de Nome de Domínio**), representado no diagrama pelo **Ponto C**. Em termos práticos, os **Servidores DNS** fazem a ligação entre um **Domínio** e um **número de IP**, que nada mais é do que a **identificação do servidor para o qual o domínio está apontado**. Para facilitar ainda mais, um **Servidor DNS** é o sistema que traduz o ***“site.com.br”*** para um **Endereço de IP**, por exemplo, **151.101.129.121**. Isso ocorre quando o domínio é digitado nos navegadores.

- Vamos agora retornar ao cenário proposto anteriormente, e entender **passo-a-passo** do que ocorre nesse acesso:
    
    
    1. Você se encontra no **Ponto A** (conectado à **Internet**), e, no seu navegador, digita o **endereço do site** que deseja acessar (ex: www.facebook.com).
    2. A arquitetura da **Internet** (**Ponto B**) irá localizar o **Servidor DNS** que possui o registro do **IP** referente ao domínio que você digitou.
    3. O **Servidor DNS**, que representa o **Ponto C**, irá retornar o **Endereço IP** atual do site que foi requisitado (ex: no dia em que escrevi esse material, o IP do www.facebook.com era **157.240.22.35**).
    4. Uma vez que seu navegador possui o **Endereço IP** do site que deseja acessar, o mesmo manda uma mensagem de requisição **HTTP** para o servidor (**Ponto D**), pedindo que envie uma cópia do site ao cliente (**Ponto A**).
    5. Caso a requisição seja aceita, o servidor (**Ponto D**) começará a **enviar os arquivos** do site para o seu navegador, por meio de uma série de pequenos pedaços chamados **pacotes de dados**. Com isso, o navegador **monta os pequenos pedaços em um site completo** e o exibe a você.

<aside>
🚫 As **Rotas** representam outro assunto importante para o funcionamento da **Internet**. Para enviar um sinal de um **Ponto A** para um **Ponto B**, podemos ter várias rotas. Quem irá definir a melhor rota são os **Roteadores** que compõem a rede.

</aside>

---

# Hospedagem de Sites

- Quando um site é desenvolvido de forma local (utilizando o **Localhost**), a única forma de acessá-lo é por meio de uma **URL especia**l (ex: localhost:00000). O problema prático desse tipo de desenvolvimento de site é a **incapacidade de compartilhamento** do mesmo, tendo em vista que **apenas clientes conectados à mesma rede de Internet** têm acesso ao que foi desenvolvido.

- A fim de resolver esse problema, algumas empresas fornecem serviços de **Hospedagem**, que na prática, permitem que você publique um site na **Internet** e o deixe acessível a todos. Essas **Provedoras de Hospedagem** armazenam os dados do seu site em seus servidores, e os enviam para os navegadores de seus usuários quando eles digitam sua **URL** na barra de endereço.

---

# URL e Domínio

- Vimos anteriormente que todo site é identificado por meio de seu **Endereço IP**, porém, a fim de simplificar o acesso, a grande maioria dos sites utilizam um **Domínio**. Um **Domínio** trata-se de um nome único (**não existem dois Domínios de mesmo nome**), usado para conectar o site à sua hospedagem. Vale ressaltar que, para ter direito a um nome de **Domínio**, é necessário pagar pelo mesmo (normalmente por meio de assinaturas anuais).

![anatomia url.png](Como%20a%20Internet%20Funciona%20bfc81b15694343dabfe46d106344a199/anatomia_url.png)

- A imagem acima representa uma **URL**: ***U**niform **R**esource **L**ocator* (**Localizador Uniforme de Recursos**), que nada mais é do um **endereço virtual de uma página ou website**. Cada uma dos elementos que compõem uma **URL** representam **funções** e **significados específicos**, veremos a seguir uma simples definição de cada elemento:
    
    
    - **Protocolo (`https://`):** O **Protocolo** informa ao navegador como se **comunicar com o servidor** de um site, a fim de **enviar** e **recuperar** informações. Os protocolos podem variar, geralmente, entre **HTTP** e **HTTPS**, dependendo do nível de segurança (o protocolo **HTTPS** representa uma versão mais segura do protocolo **HTTP**).
    
    ---
    
    - **Subdomínio (`blog`):** O **Subdomínio** é comumente usado para **separar logicamente um site em seções**. O “**www”** costuma ser o **subdomínio principal** de um servidor web, porém é perfeitamente possível que um mesmo site possua **vários subdomínios.** Tomando o Google como exemplo:
        - www.google.com: Dá acesso ao site principal do Google.
        - images.google.com: Dá acesso ao Google Images.
        - maps.google.com: Dá acesso ao Google Maps.
    
    ---
    
    - **Domínio (`hubspot.com`):** O **Domínio** é um identificador único de um site, que geralmente leva o cliente para a **página inicial**, caso nada seja adicionado ao final. Naturalmente, um nome de **domínio** é composto de **duas partes**: o **nome do site em questão** e o **TLD**.
    
    ---
    
    - **TLD (`.com`):** O **TLD: *T**op-**L**evel **D**omain* (Domínio de Nível Superior) representa parte essencial ****do **Domínio**, na prática, serve para **facilitar e organizar a categorização de páginas na web** com base nas informações associadas aos sites. Os **TLDs** podem ser divididos em dois principais grupos:
        - **gTLD:** Representam **TLDs genéricos**, sem indicação de país (ex: .com, .net, .gov, .org).
        - **ccTLD:** Representam **TLDs com código de país** (country code), projetados para indicar uma localização geográfica ou país específico (ex: .br, .tk, .jp, .cn)
        
        Vale destacar que vários sites podem compartilhar o mesmo nome, mas terem **TLDs** diferentes (ex: meusite.com é diferente de meusite.edu).
        
    
    ---
    
    - **Subdiretório (`/marketing`):** O **Subdiretório** apesar de opcional, ajuda a indicar as pastas que devem ser percorridas para que se enconte um **arquivo específico** dentro do site.
    
    <aside>
    🚫 Saber escolher bons **Domínios**, tal qual bons **Serviços de** **Hospedagem**, traz diversas vantagens tanto para o **desenvolvedo**r quanto para o **cliente**, tais como: **credibilidade perante o usuário**, **maior segurança**, além de oferecer certa dose de **profissionalismo**.
    
    </aside>