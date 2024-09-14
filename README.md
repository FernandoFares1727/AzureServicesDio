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

Resumo Final
Os SLAs no Azure são fundamentais para garantir níveis de serviço adequados para diferentes cenários. À medida que as necessidades de disponibilidade e resiliência aumentam, as opções de configuração, como Availability Sets e Availability Zones, permitem que as empresas ajustem suas VMs e outros recursos da nuvem para garantir SLAs mais altos. Azure oferece flexibilidade com IaaS, PaaS e SaaS, permitindo que os clientes configurem e escolham serviços com diferentes SLAs de acordo com suas necessidades de negócio e criticidade dos aplicativos.
