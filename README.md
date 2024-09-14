# AzureServicesDio
Descrição dos Laboratórios de Bootcamp Dio

O que é Computação em Nuvem

Computação em nuvem é um modelo de entrega de serviços de TI onde os recursos, como armazenamento, processamento e software, são disponibilizados através da internet. Em vez de manter infraestrutura local, as empresas podem alugar esses recursos de provedores de serviços em nuvem, que gerenciam toda a parte de hardware, redes e manutenção. Isso permite maior flexibilidade, escalabilidade e economia de custos.

Existem diferentes tipos de nuvens, categorizadas principalmente como nuvem pública, nuvem privada e nuvem híbrida:

Nuvem Pública: Oferecida por terceiros (como Microsoft Azure, AWS e Google Cloud), em que os recursos são compartilhados entre múltiplos clientes. É acessível publicamente e oferece uma solução econômica, especialmente para startups e empresas que não querem gerenciar infraestrutura física.

Nuvem Privada: Utilizada por uma única organização, seja hospedada no local (on-premises) ou por um provedor de terceiros. A nuvem privada oferece maior controle e segurança, sendo uma escolha comum para empresas que lidam com dados sensíveis ou precisam cumprir regulamentações específicas.

Nuvem Híbrida: Combina as nuvens pública e privada, permitindo que as empresas utilizem ambas de acordo com suas necessidades. Por exemplo, uma empresa pode manter seus dados mais críticos em uma nuvem privada e usar uma nuvem pública para aumentar a capacidade durante picos de demanda.

Modelos de Serviço: IaaS, PaaS e SaaS
IaaS (Infrastructure as a Service): Fornece recursos de infraestrutura, como servidores, armazenamento, e redes. O cliente tem controle sobre o sistema operacional, aplicativos e dados, enquanto o provedor gerencia o hardware. Um exemplo de IaaS no Azure é o Azure Virtual Machines, que permite criar e gerenciar máquinas virtuais na nuvem.

PaaS (Platform as a Service): Oferece uma plataforma que permite desenvolver, testar e gerenciar aplicativos sem se preocupar com a infraestrutura subjacente. O cliente foca no desenvolvimento e implantação de aplicativos, enquanto o provedor gerencia tudo, desde o sistema operacional até a rede. No Azure, o Azure App Service é um exemplo de PaaS, facilitando a criação e hospedagem de aplicativos web sem precisar gerenciar servidores.

SaaS (Software as a Service): Nesse modelo, o cliente acessa softwares prontos para uso, normalmente através de um navegador. Não há necessidade de gerenciar a infraestrutura ou desenvolver a aplicação; tudo é oferecido pelo provedor. O Microsoft 365 é um exemplo popular de SaaS no Azure, onde os usuários podem acessar aplicativos como Word, Excel e Outlook diretamente pela internet.

Como os Serviços se Encaixam no Azure
IaaS no Azure: A Microsoft Azure oferece uma variedade de serviços de infraestrutura, como máquinas virtuais, redes e balanceadores de carga. Isso permite que empresas aluguem recursos de computação e armazenamento conforme necessário, sem se preocupar com hardware físico.

PaaS no Azure: Com serviços como o Azure App Service e o Azure Functions, o Azure permite que desenvolvedores criem, implantem e gerenciem aplicativos sem a complexidade de gerenciar servidores. Isso acelera o processo de desenvolvimento e reduz custos com manutenção de infraestrutura.

SaaS no Azure: Serviços como Microsoft 365 e Dynamics 365 estão disponíveis diretamente na plataforma Azure, permitindo que os usuários acessem softwares empresariais completos de forma simples e sem precisar instalar ou manter nada localmente.

O Azure oferece uma plataforma versátil e escalável que cobre os três modelos de serviço (IaaS, PaaS, e SaaS) e as diferentes opções de nuvem (pública, privada e híbrida), atendendo a uma ampla gama de necessidades empresariais e tecnológicas.

O que é SLA (Service Level Agreement)
O SLA (Acordo de Nível de Serviço) é um contrato ou compromisso entre um provedor de serviços e o cliente que define o nível mínimo de serviço esperado. Em termos técnicos, o SLA descreve métricas como disponibilidade, tempo de resposta, suporte e resolução de problemas que o provedor garante oferecer ao cliente.

No contexto de computação em nuvem, o SLA geralmente se refere à disponibilidade (uptime) dos serviços, medido em termos percentuais ao longo de um período (normalmente mensal). Por exemplo, um SLA com 99,9% de disponibilidade significa que o serviço estará indisponível por no máximo 43 minutos em um mês (30 dias).

Os SLAs são importantes porque oferecem garantias de qualidade e desempenho dos serviços. Se o provedor não atingir os níveis de serviço estabelecidos, o cliente pode receber compensações, como créditos no uso do serviço.

Relação do SLA com os Tipos de Serviços do Azure
O Microsoft Azure oferece diferentes SLAs dependendo do tipo de serviço e da configuração utilizada. Aqui estão exemplos de SLAs para os principais tipos de serviços:

IaaS no Azure (Infrastructure as a Service):

Para máquinas virtuais (VMs), o SLA depende da configuração. Por exemplo:
SLA de 99,9%: Para uma única máquina virtual que utiliza armazenamento premium em discos gerenciados.
SLA de 99,95%: Para máquinas virtuais que estão distribuídas em conjuntos de disponibilidade (Availability Sets) dentro da mesma região.
SLA de 99,99%: Para máquinas virtuais que estão em zonas de disponibilidade (Availability Zones), onde os dados são replicados entre diferentes datacenters dentro da mesma região.
Isso significa que, dependendo de como você configura suas máquinas virtuais, você pode garantir um nível maior ou menor de disponibilidade, o que é crucial para cargas de trabalho críticas.

PaaS no Azure (Platform as a Service):

Serviços PaaS, como Azure App Service e Azure SQL Database, têm SLAs mais altos, como 99,95% ou até 99,99% de disponibilidade, pois o Azure gerencia toda a infraestrutura subjacente e a configuração da plataforma. O cliente se beneficia de maior resiliência e redundância sem precisar gerenciar a infraestrutura por trás dos aplicativos.
SaaS no Azure (Software as a Service):

Para soluções SaaS, como o Microsoft 365, a Microsoft oferece SLAs de 99,9% de disponibilidade, garantindo que as aplicações estarão acessíveis quase todo o tempo. Como esses serviços já vêm configurados e gerenciados pelo Azure, os usuários não precisam se preocupar com questões de disponibilidade, escalabilidade ou manutenção de hardware.
SLAs e Máquinas Virtuais no Azure
As Máquinas Virtuais (VMs) no Azure são um exemplo claro de como o SLA varia de acordo com as configurações escolhidas. A Microsoft oferece opções como Availability Sets e Availability Zones para aumentar a resiliência dos serviços e garantir maior disponibilidade.

Availability Sets: São usados para garantir que VMs em um conjunto sejam distribuídas em diferentes domínios de falha e atualização. Isso ajuda a minimizar o impacto de falhas de hardware ou de atualizações de manutenção. O SLA oferecido para VMs em Availability Sets é 99,95% de disponibilidade.

Availability Zones: Distribuem VMs entre diferentes datacenters dentro de uma mesma região. Como as zonas são fisicamente separadas, isso garante uma proteção ainda maior contra falhas de datacenters inteiros. O SLA para VMs distribuídas em Availability Zones é 99,99%.

Processo de Criação de uma Instância de Banco de Dados e Servidor no Azure
No Microsoft Azure, criar uma instância de banco de dados envolve a configuração de um banco de dados e seu servidor associado, que fornece o ambiente de execução necessário. Abaixo, descrevemos o processo geral para criar um banco de dados, usando como exemplo o Azure SQL Database, um dos serviços de banco de dados mais populares da plataforma. O processo pode ser aplicado de forma semelhante a outros tipos de bancos de dados no Azure, como MySQL, PostgreSQL e MariaDB.

1. Acesso ao Portal Azure
O primeiro passo é acessar o Portal do Azure (portal.azure.com) com suas credenciais.
A partir da página inicial do portal, você pode pesquisar por “SQL Database” ou acessar diretamente a seção de bancos de dados.
2. Criação do Servidor de Banco de Dados
Um servidor de banco de dados no Azure é o ambiente de hospedagem no qual o banco de dados será executado. Para criar um servidor, siga estes passos:
Clique em “Criar um recurso” e procure por "SQL Server" (para bancos de dados SQL Server) ou o banco de dados específico que você deseja (PostgreSQL, MySQL etc.).
Preencha as informações básicas:
Nome do Servidor: Escolha um nome único para o servidor de banco de dados.
Região: Escolha a região onde o servidor será hospedado. Isso impacta a latência e a proximidade dos usuários ao banco de dados.
Autenticação: Configure um nome de usuário e senha para administrar o servidor. O Azure também oferece suporte à autenticação integrada com o Azure Active Directory (AD).
Grupo de Recursos: Escolha um grupo de recursos existente ou crie um novo. Isso facilita a organização e o gerenciamento dos recursos no Azure.
Escolha o modelo de licença e a camada de desempenho do servidor, como a quantidade de vCPUs e memória, conforme suas necessidades de escalabilidade e carga de trabalho.
Clique em Revisar + Criar e, em seguida, Criar para provisionar o servidor. O processo de criação leva alguns minutos.
3. Criação do Banco de Dados
Com o servidor provisionado, o próximo passo é criar a instância do banco de dados que rodará nesse servidor:

No portal do Azure, procure por SQL Database ou o tipo de banco de dados que você deseja (por exemplo, Azure Database for MySQL ou PostgreSQL).
Clique em Criar Banco de Dados SQL.
Preencha as informações necessárias:
Nome do Banco de Dados: Escolha um nome significativo para o banco.
Servidor: Escolha o servidor que você acabou de criar.
Camada de Desempenho: Selecione a camada de desempenho com base nas suas necessidades de capacidade, como DTUs (Database Transaction Units) para o SQL Database ou vCores, que permitem maior controle sobre CPU e memória.
Backup e Redundância: Escolha as opções de backup (locais, georredundantes ou sem redundância). Essas opções influenciam a recuperação de desastres e a durabilidade dos dados.
Após configurar as opções de desempenho e backup, clique em Revisar + Criar e, depois, em Criar.
4. Configuração de Segurança e Regras de Firewall
Uma vez que o banco de dados e o servidor estão criados, é necessário configurar as políticas de segurança:

Regras de Firewall: Por padrão, o acesso ao servidor de banco de dados é bloqueado de fora da rede do Azure. Para habilitar conexões externas, configure as regras de firewall, permitindo o acesso de IPs específicos ou de toda a rede do Azure.
Autenticação: Use as credenciais de administrador configuradas durante a criação do servidor ou integre o Azure Active Directory (AD) para gerenciar a autenticação de forma centralizada.
5. Conexão ao Banco de Dados
Após a criação do banco de dados, você pode conectar-se a ele usando uma ferramenta de gerenciamento de banco de dados (como SQL Server Management Studio (SSMS) para SQL Server ou pgAdmin para PostgreSQL):

Para conectar, você precisará do nome do servidor, nome do banco de dados, usuário administrador e senha configurados anteriormente.
Use o endpoint do servidor (geralmente no formato servidor.database.windows.net) para estabelecer a conexão.
6. Monitoramento e Manutenção
O Azure oferece várias ferramentas integradas para monitoramento, otimização e manutenção de bancos de dados:

Azure Monitor: Permite acompanhar o desempenho e os recursos consumidos pelo banco de dados.
Query Performance Insight: No caso de SQL Database, oferece insights sobre consultas que podem estar degradando o desempenho.
Backup e Recuperação Automática: Configure backups automáticos para garantir a restauração de dados em caso de falhas ou perda de informações.
7. Escalabilidade
O Azure permite a escalabilidade horizontal (adicionando réplicas de leitura) e a escalabilidade vertical (aumentando a capacidade de computação e armazenamento). Isso pode ser feito sem interromper o serviço, garantindo que o banco de dados cresça conforme suas necessidades.

Resumo Final
O processo de criação de uma instância de banco de dados e um servidor no Azure envolve configurar o servidor para hospedar o banco de dados, selecionar as camadas de desempenho adequadas, configurar regras de segurança (como firewall), e monitorar o desempenho do banco. O Azure simplifica esse processo com uma interface intuitiva no portal e fornece opções para aumentar a resiliência, como backups automáticos, regras de firewall e escalabilidade sob demanda, garantindo alta disponibilidade e segurança dos dados.

Resumo Final
Os SLAs no Azure são fundamentais para garantir níveis de serviço adequados para diferentes cenários. À medida que as necessidades de disponibilidade e resiliência aumentam, as opções de configuração, como Availability Sets e Availability Zones, permitem que as empresas ajustem suas VMs e outros recursos da nuvem para garantir SLAs mais altos. Azure oferece flexibilidade com IaaS, PaaS e SaaS, permitindo que os clientes configurem e escolham serviços com diferentes SLAs de acordo com suas necessidades de negócio e criticidade dos aplicativos.
