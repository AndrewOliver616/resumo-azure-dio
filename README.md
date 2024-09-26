# resumo-azure-dio
Repositório de resumo de aprendizado do curso de Azure Microsoft na DIO

Neste curso, até o momento, vimos os fundamentos da computação em nuvem e fomos apresentados aos principais recursos da plataforma.

O conceito de computação em nuvem em fornecer serviço de computação pela internet, habilitando inovações mais rápidas, recursos flexíveis e economia de escala.
Vimos os principais tipos de Nuvem: Privada, Pública e Híbrida. Foi abordado os conceitos de CapEx e OpEx explorando os típos de despesas na computação em nuvem.
AZ-900: Introdução e conceito (Benefícios da Nuvem AZURE)

Alta disponibilidade, Escalabilidade, Elasticidade, Confiabilidade, Previsibilidade, Governança e Gerenciabilidade.
Tipos de serviço em Nuvem.

IaaS - Infraestrutura como serviço
PaaS - Plataforma como serviço
SaaS - Software como serviço

Modelos de responsabilidade Compartilhada.

Arquitetura e Serviços do Azure
- Componentes de Arquitetura
  *Regiões e Zonas de Disponibilidade
  Pares de região: Regiões Soberanas do Azure, Governo dos EUA e China* (*VIA 21)
  *Assinaturas e Grupos de Serviço

Recursos do Azure
  Grupos de Recursos
  Assinaturas do Azure (Limite de cobrança e Limite do Controle de Acesso)
    Grupos de Gerenciamento - Podem incluir várias assinaturas, as assinaturas herdam as condições aplicadas ao grupo de gerenciamento.
Computação e Rede
  Serviços de Computação e Máquinas Virtuais
  VMs - Emulação de software de computadores físicos
  Conjunto de dimensionamento de VMs - Balanceamento de carga para dimencionar os recursos automaticamente.
  Área de trabalho remota -Virtualização da área de trabalho e aplicativo executado em nuvem.
  Serviços de contêiner do Azure - Ambiente leve e virtualizado que nçao exige o gerenciamento do sistema operacional #PaaS
  Azure Functions - Oferta de PaaS que dá suporte a operaçao de computação sem servidor.
  Serviço de aplicativo do Azure: Plataforma gerenciada para criar, implantar, e dimensionar aplicativos web e APIs rapidamente.

Serviços de Rede
  Permite que os serviços/recursos do Azure se comuniquem um com o outro e com a internet.
    Sub-redes virtuais
  Gateway de VPN - Tráfego criptografado
  Express Route - Conexão privada facilitada por um provedor de conectividade
  DNS do Azure - serviço de hospedagem de domínios DNS (Sistema de Nomes de Domínio) na infraestrutura da Microsoft Azure. Ele permite que gerencie registros DNS usando as mesmas credenciais, APIs, ferramentas e faturamento que os outros serviços do Azure12.

Armazenamento AZURE
  Contas de armazenamento Storage Account
    *Nome globalmente exclusivo (não apenas na sua conta, entre todas as contas existente no mundo inteiro, de qualquer usuário). Utilizar de 3 a 24 caracteres.
    Fornecer acesso a internet em todo o mundo
  Determinar serviços de armazenamento e as opções de redundância - LRS | ZRS | GRS | GZRS
  LRS - Redundância Local [11 noves] - Datacenter Local
  ZRS - Redundância de Zona [12 noves] - Três Zonas de Disponibilidade na região primária
  GRS - Redundância Geográfica [16 noves] - Datacenter único no primário e na região secundária.
  GZRS - Redundância de Zona Geográfica [16 noves] - Três zonas de disponibilidade na região primária e um único datacenter na região secundária.

Serviços de Armazenamento do Azure
  Blob do Azure - Otimizado para armazenamento de quantidades massiavas NÃO ESTRUTURADAS. blob.core.windos.net
  Disco do Azure - Disco para máquinas virtuais, aplicativos e outros serviços. dfs.core.windos.net
  Fila do Azure - Armazenamento de mensagens (armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64kb) queue.core.windos.net
  Arquivos do Azure - Compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando protocolo de bloco de mensagens do servidor. file.core.windos.net
  Tabela do Azure - Opção de chave de atributo para o armazenamento de dados estruturados NÃO RELACIONAIS com um design sem esquema. table.core.windos.net

Contas de Acesso de Armazenamento
  Frequente: Dados acessados com frequência
  Esporádico: Acessados com pouca frequência, dados armazenados por pelo menos 30 dias
  Frio: Dados acessados com pouca frequência, armazenados por pelo menos 90 dias
  Arquivo morto: Dados raramente acessados, armazenados por pelo menos 180 dias
  *NOTA: Quanto ,ais tempo sem consulta, mais cara será a requisição, quanto mais acessado, mais barata será cada requisição.
Migração para AZURE
  Plataforma de migração unificada
  Intervalo de ferramentas integradas e autônomas
  Avaliação e Migração

   Azure Data Box: Armazena até 80 TBs de dados
    *Recuperação de desastres, conformidade ou necessidade regulatória, locais remotos com conectividade limitada.
  AzCopy: Utilitário de linha de comando
    *Copiar Blobs, sicronização em uma direção.
  Gerenciador de armazenamento: Interface gráfica do usuário.
    *Compátivel com Windows, MacOS e Linux
  Sincronização de Arquivos: Sincroniza arquivo locais de forma bidirecional
    *A camada de nuvem mantém os arquivos acessos com frequência no local, enquanto libera espaço.

   Microsoft Entra ID
    Serviço de gerenciamento de identidades e acesso baseado em nuvem do Microsoft Azure!
    *Autenticação (os funcionários entram para acessar os recursos).
    *Logon único (SSO)
    *Gerenciamento de aplicativos.
    *Negócios para Negócios (B2B).
    *Gerenciamento de dispositivos.
Autenticação
 * Identifica a pessoa ou serviço buscando acesso a um recurso.
 * Solicita credenciais de acesso legítimo
 * Base para criar principios de identidade e controle de acesso seguros

   
Autorização
 *Determina o nível de acesso de uma pessoa ou serviço autenticado
 *Define quais dados eles podem acessar e o que podem fazer com eles.
 
Autenticação Multifator
 *Fornece segurança adicional para s identidades exigindo dois ou mais elementos para autenticação completa.
 
Acesso Condicional
   * É utilizado para reunir sinais , tomar decisões e impor políticas organizacionais.
 #Associação de usuário ao grupo, local do IP, dispositivo, aplicativo e detecção risco.

Controle de acesso baseado em função
 *Confiança Zero: é uma abordagem de segurança que parte do pressuposto de que nenhuma entidade, seja interna ou externa à rede, deve ser automaticamente confiável. Em vez disso, todas as tentativas de acesso devem ser verificadas e autenticadas continuamente.

Proteção Completa
 *Uma abordagem em camada para proteger sistemas de computador.
 *Fornece vários níveis de proteção.
 *Ataques contra uma camada são isolados das camadas subsequentes.

Microsoft Defender para nuvem
 * é um serviço de monitoramento que fornece proteção contra ameaças nos datacenters do Azure e locais.
 * Fornece recomendações de segurança.
 * Detectar e bloquear malware
 * Analisar e identificar ataques potenciais.
 * Controle de acessos just-in-time para portas.

   #NOTA: Contas de usuários excluídas podem ser restauradas até 30 dias da data da exclusão.


Otimizando Custo no Azure

 Calculadora de Custo Total de Propriedade - TCO
 Calculadora do Azure

*Auxílio nas estimativas de economia em obter os serviços de nuvem do Azure.

Definir as cargas de trabalho

Servidores

Bancos de Dados

Armazenamento

Rede

Cobertura do software Assurance (Benefício Híbrido) - Benefício híbrido tende a diminuir o custo de aquisição dos serviços. Reserva e horas ativas também influenciam o no custo total.

Cost Management + Billing e Marcas (Tags)
Análises de recursos por marcas para identificar os focos de gastos da assinatura e buscar alternativas através de estratégias. Além disso é possível criar um linha de corte para os custos de determinado recursos, seja com alertas, seja com redução/suspensão do uso por determinados períodos.

Tags: Research Group - Não são pré-requisitos, dupla chave e valor com apontamento de centro de custo, a Tag não é herdável
