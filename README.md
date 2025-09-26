# ☁️ Computação em Nuvem – Resumo

A **computação em nuvem (cloud computing)** é o modelo de uso de recursos de **TI** (armazenamento, processamento, redes, bancos de dados e softwares) fornecidos pela **internet**, em vez de depender apenas de servidores locais. Assim, usuários e empresas podem **alugar recursos sob demanda** de provedores como [AWS](https://aws.amazon.com/), [Microsoft Azure](https://azure.microsoft.com/) e [Google Cloud](https://cloud.google.com/).

---

## 🔑 Características
- 🌍 **Acesso remoto** de qualquer lugar com internet  
- 📈 **Elasticidade** para ampliar ou reduzir recursos conforme a demanda  
- 💳 **Pagamento sob demanda** (*pay-as-you-go*)  
- 🔒 **Gerenciamento simplificado**, já que o provedor cuida da infraestrutura  
- ⚡ **Escalabilidade** rápida, sem necessidade de aquisição de hardware físico  
- 📊 **Alta disponibilidade e tolerância a falhas** com replicação de dados e redundância  

---

## 🌐 Modelos de Implantação
- ☁️ **Nuvem Pública** → infraestrutura compartilhada (ex.: Gmail, Dropbox, AWS)  
- 🏢 **Nuvem Privada** → infraestrutura exclusiva de uma organização (ex.: bancos)  
- 🔗 **Nuvem Híbrida** → combinação de pública + privada, equilibrando custo e segurança  

---

## ⚙️ Modelos de Serviço

| **Serviço** | **O que oferece** | **Exemplos** | **Uso comum** |
|-------------|-----------------|-------------|---------------|
| 🖥️ **IaaS** (*Infrastructure as a Service*) | Máquinas virtuais, armazenamento, redes, servidores | AWS EC2, Azure VMs, Google Compute Engine | Hospedagem de sites, bancos de dados, ambientes de teste e desenvolvimento |
| 💻 **PaaS** (*Platform as a Service*) | Ambiente completo para desenvolver, testar e implantar aplicações | Heroku, Google App Engine, Azure App Service | Desenvolvimento ágil de aplicativos, APIs, microserviços |
| 📦 **SaaS** (*Software as a Service*) | Aplicativos prontos para uso via internet | Microsoft 365, Google Workspace, Salesforce | E-mail corporativo, colaboração, CRM, ferramentas de produtividade |
| 🗄️ **FaaS / Serverless** (*Function as a Service*) | Execução de funções sem se preocupar com servidores | AWS Lambda, Azure Functions | Automação de processos, execução de funções sob demanda |
| 🛠️ **DaaS** (*Desktop as a Service*) | Área de trabalho virtual acessível remotamente | Amazon WorkSpaces, Citrix DaaS | Trabalho remoto, ambientes seguros para colaboradores externos |

---

## 💰 CapEx x OpEx
- 💵 **CapEx (Capital Expenditure)** → investimento inicial alto em infraestrutura própria (ex.: compra de servidores)  
- 🔄 **OpEx (Operational Expenditure)** → custos operacionais recorrentes, comuns na nuvem (ex.: assinaturas SaaS)  
- ⚡ **Baseado em Consumo** → paga apenas pelo que usar (ex.: Azure VMs, AWS EC2)  

| **Modelo** | **Exemplo em TI** | **Vantagens** | **Desvantagens** |
|------------|------------------|---------------|------------------|
| **CapEx** | Comprar servidores e montar datacenter | Controle total, custo previsível a longo prazo | Alto investimento inicial, risco de ociosidade |
| **OpEx fixo** | Licença mensal SaaS (ex.: Microsoft 365) | Previsibilidade de custos | Paga mesmo sem uso intenso |
| **Consumo (pay-as-you-go)** | AWS EC2, Azure VMs | Flexibilidade, paga só pelo uso | Difícil prever custos em alta demanda |

---

## 🌟 Benefícios da Computação em Nuvem
- 🚀 **Agilidade e inovação** → permite testar e lançar novos serviços rapidamente  
- 💰 **Redução de custos** → elimina investimento em infraestrutura física e manutenção  
- 🔄 **Escalabilidade elástica** → ajusta recursos automaticamente conforme a demanda  
- 🔒 **Segurança aprimorada** → provedores investem em criptografia, backups e monitoramento  
- 🌍 **Acesso global** → usuários podem acessar serviços de qualquer lugar do mundo  
- 🛠️ **Atualizações automáticas** → softwares e plataformas são mantidos atualizados pelo provedor  
- 📊 **Análise de dados avançada** → integração com serviços de Big Data e IA  

# 🏗️ Componentes de Arquitetura do Azure

## 1. Regiões
- Conjuntos de datacenters implantados em uma área geográfica específica.  
- Mais de **60 regiões globais** cobrindo mais de 140 países.  
- Reduzem **latência**, preservam a **residência dos dados** e permitem **escalabilidade**.  

---

## 2. Zonas de Disponibilidade
- **Datacenters independentes** dentro de uma região, com energia, rede e refrigeração próprias.  
- Interligados por **rede de fibra óptica privada**.  
- Garantem **alta disponibilidade** e **tolerância a falhas**.  

---

## 3. Pares de Regiões
- Regiões sempre são **emparelhadas** (mínimo **300 milhas de distância**).  
- Permitem **replicação automática**, **recuperação priorizada** e **atualizações sequenciais**.  

---

## 4. Regiões Soberanas
- Exemplo: **Azure Government (EUA)**.  
- **Isoladas fisicamente** do Azure público.  
- Foco em **conformidade legal** e **segurança crítica**.  

---

## 5. Recursos do Azure
- Unidades fundamentais como **VMs, armazenamento, redes e serviços de aplicação**.  
- São os **blocos básicos** para criar soluções em nuvem.  

---

## 6. Grupos de Recursos
- **Contêineres lógicos** para organizar e gerenciar recursos.  
- Um recurso só pode estar em **um grupo por vez**, mas grupos podem conter recursos de várias regiões.  
- Facilitam **monitoramento, políticas e controle de acesso**.  

---

## 7. Assinaturas do Azure
- Delimitam **escopo de cobrança e permissões**.  
- Permitem **relatórios de faturamento separados** e **controle de acesso granular**.  
- Exemplo: uma assinatura para **produção** e outra para **testes**.  

---

## 8. Grupos de Gerenciamento
- Camada **acima das assinaturas**.  
- Permitem aplicar **políticas e segurança** em várias assinaturas ao mesmo tempo.  
- Muito usados por **grandes empresas e multinacionais**.  

---

## 📌 Estrutura Hierárquica do Azure
1. **Recursos** →  
2. **Grupos de Recursos** →  
3. **Assinaturas** →  
4. **Grupos de Gerenciamento**  

🔹 Essa hierarquia garante **organização, governança e escalabilidade** dentro do Azure.  

---

## O que é computação em rede

“Computação em rede” refere-se ao uso de vários dispositivos de computação interconectados por meio de redes (físicas ou sem fio) para permitir:

- troca de dados entre dispositivos;
- compartilhamento de recursos (impressoras, arquivos, servidores, etc.);
- execução de aplicações de forma distribuída;
- colaboração remota.
Em essência, trata-se de fenômenos onde não há apenas um único computador operando de forma isolada, mas um conjunto trabalhando de modo cooperativo sobre uma infraestrutura de rede.
---

## O que são Azure Virtual Machines

As Azure VMs são instâncias de servidores virtuais fornecidas pela Microsoft na nuvem, que permitem executar sistemas operacionais (Windows, Linux, etc.), aplicações, bancos de dados, serviços de backend etc., sem precisar manter hardware físico próprio.
Você escolhe “o tamanho” da VM (vCPU, RAM, armazenamento, etc.), o sistema operacional, e paga pelo uso desses recursos.

---

## O que é um Conjunto de Disponibilidade (Availability Set)

Um *Availability Set* (conjunto de disponibilidade) é um agrupamento lógico de VMs dentro de um mesmo datacenter do Azure que tem como objetivo reduzir o risco de que falhas ou manutenções afetem todas as VMs de uma aplicação ao mesmo tempo. 
Ele é usado para garantir alta disponibilidade de aplicações, atendendo ao SLA de **99,95%** para VMs (desde que haja duas ou mais instâncias dentro do conjunto de disponibilidade).

---

## Como funciona: domínios de falha e domínios de atualização

Dois conceitos centrais no Availability Set:

| Conceito | O que significa | Por que importa |
| --- | --- | --- |
| **Domínio de Falha** (*Fault Domain*, FD) | Refere-se a um conjunto físico de hardware que compartilha infraestrutura comum: racks, alimentação elétrica, switches de rede. Se desse hardware vier a falhar, todas as VMs que estiverem no mesmo domínio de falha poderão ser afetadas. | Distribuir as VMs em diferentes domínios de falha ajuda a evitar que uma falha de hardware ou de energia derrube todas as VMs de uma aplicação ao mesmo tempo. |
| **Domínio de Atualização** (*Update Domain*, UD) | Refere-se a conjuntos de VMs que podem ser reiniciados ou atualizados pelo Azure ao mesmo tempo durante manutenções planejadas. Cada domínio de atualização define quais VMs vão “parar” juntas em uma manutenção. | Ao repartir VMs em diferentes domínios de atualização, o Azure garante que nem todas serão afetadas por uma manutenção de uma só vez. Só um update domain é reiniciado por vez.|

---

## Azure Virtual Desktop (AVD)

**O que é**

- Serviço de virtualização de desktops e apps rodando na nuvem Azure. Permite que usuários acessem ambientes Windows (desktop completo) ou aplicações específicas remotamente, de qualquer dispositivo.
- Oferece opções de desktop com sessão única ou multi-sessão.

**Principais funcionalidades**

- Publicação de aplicativos ou desktops (RemoteApp / full desktop).
- Imagens personalizadas, pools de hosts, workspaces gerenciados.
- Otimizações para Microsoft 365, suporte para Windows 10/11 multi-sessão, o que reduz custos de licenciamento/infraestrutura.
- Autoscaling, para ajustar capacidade conforme demanda.

**Vantagens**

- Facilita trabalho remoto e mobilidade, com segurança centralizada.
- Menor gerenciamento de hardware local.
- Economias quando se utiliza sessão multi-usuário, ou se aproveita licenças existentes.
- Experiência de usuário mais padronizada.

**Quando usar**

- Organizações que precisam prover desktops remotos para funcionários – home office, suporte remoto, terceirizados.
- Aplicações legadas que exigem ambiente Windows específico.
- Casos em que segurança, controle e conformidade são rígidos (pois os ativos ficam no Azure).

**Limitações / Considerações**

- Há custo contínuo com VMs, armazenamento, rede. Apesar de autoscaling, dimensionamento incorreto pode gerar desperdício.
- Dependência de conectividade de rede e latência, especialmente para usuários remotos distantes.
- Gerenciamento de perfis, aplicativos, compatibilidade etc precisa ser bem planejado.

---

## Containers no Azure

**O que são / exemplos de serviços**

- Contêineres são unidades leves de empacotamento de aplicações (app + dependências), que compartilham o kernel do sistema, mas rodam isoladas umas das outras. 
- Azure oferece vários serviços de containers, como:
    
    • **Azure Kubernetes Service (AKS)** — orquestração de containers em escala. 
    
    • **Azure Container Instances (ACI)** — rodar containers rapidamente, sem precisar gerenciar VMs ou clusters. 
    
    • **Azure Container Apps** — abordagem serverless para containers, microserviços, apps modernos.
  
    • Outros: Web App for Containers, OpenShift no Azure, registro de imagens (Container Registry) etc. 
    

**Principais vantagens**

- Leveza: containers iniciam rápido, consomem menos recursos comparados a VMs, já que não carregam sistema operacional completo. 
- Escalabilidade ágil: podem aumentar ou reduzir instâncias de forma dinâmica, útil para demandas variáveis ou picos.
- Portabilidade: imagens containerizadas permitem mover aplicações entre ambientes com mais facilidade (desenvolvimento, teste, produção).
- Menor overhead operacional: menos gerência de OS guest, menos patches de sistema operacional inteiro (dependendo do serviço usado) etc.

**Quando usar**

- Aplicações microserviços ou arquiteturas modernas.
- Workloads que precisam responder rapidamente a variações de carga.
- Processamento de dados em lote, tarefas curtas/efêmeras ou funções event-driven (triggered).
- Para acelerar entrega de aplicações, promover automação CI/CD, atualizações frequentes.

**Desafios / limitações**

- Segurança: embora haja bastante isolamento, containers compartilham kernel; vulnerabilidades no kernel podem afetar múltiplos containers.
- Estado persistente: containers são ideais para aplicações stateless; para estado persistente (dados, bancos), é preciso usar volumes, armazenamento externo, etc.
- Complexidade adicional se usar orquestração (ex: Kubernetes) — exige conhecimento, configuração de rede, monitoramento, logs, políticas de segurança.
- Custo de aprendizado e configuração inicial, se não houver experiência prévia.

---

## Azure Functions

**O que é**

Azure Functions é o serviço *serverless* do Azure para executar código acionado por eventos, sem que você precise gerenciar servidores ou infraestrutura subjacente. 
**Principais características**

- Tem suporte a várias linguagens (C#, JavaScript, Python, Java, PowerShell etc.). 
- Usa gatilhos (“triggers”) e vinculações (“bindings”) para reagir a eventos de Azure ou externos: por exemplo, triggers HTTP, de armazenamento (blob/queue), de timers, Service Bus, etc. 
- Modelos de hospedagem variáveis: plano de consumo (pay-per-use), plano premium, ou dentro de um App Service Plan, ou até com contêineres. 
- Escalabilidade automática: o serviço escala conforme a demanda (mais instâncias, execução paralela etc.), quando aplicável.

**Vantagens**

- Custos podem ser muito menores para workloads esporádicos ou picos: paga-se pelo que usa.
- Simplicidade operacional: menos infraestrutura para gerenciar, menos configuração de servidores, patch, etc. 
- Agilidade, ótimo para tarefas pequenas, automações, eventos, processamento em tempo real.

**Desvantagens / limitações**

- Pode haver “cold start” (latência inicial quando a função não está “ativa/quente”) dependendo do plano. Planos mais simples têm esse problema.
- Limites de tempo de execução para funções “normais” (não-duráveis) em alguns planos. Tarefas que demoram muito ou precisam de estado complexo podem exigir outras abordagens (por exemplo, *Durable Functions*). 
- Para cargas constantes e pesadas, ou aplicações que exigem muita customização ou controle sobre ambiente, pode sair mais caro ou ter menos flexibilidade se comparado a outras opções.

---

## Azure App Service (Serviços de Aplicativo do Azure)

- **Azure Virtual Network (VNet)**:
    - Conecta recursos do Azure entre si, à internet ou a redes locais.
    - Suporte a **endereços públicos e privados**.
    - Sub-redes e emparelhamento de redes privadas.
- **Gateway de VPN**:
    - Conecta redes locais ao Azure pela internet de forma segura e criptografada.
- **ExpressRoute**:
    - Conexão privada entre redes locais e o Azure via provedor.
    - Menor latência e maior confiabilidade que a VPN.
- **DNS do Azure**:
    - Gerenciamento de nomes de domínio internos e externos.
    - Usa rede Anycast global para confiabilidade.
    - Permite nomes de domínio privados customizados.

---

### **Contas de Armazenamento**

Uma conta de armazenamento é a porta de entrada para usar os serviços de armazenamento do Azure.

- Deve ter um **nome globalmente único** para evitar conflitos, pois é acessível via internet.
- Permite definir quais serviços de armazenamento estarão disponíveis e quais opções de redundância serão aplicadas.
- É nessa conta que se configuram permissões, acessos e políticas de segurança.

---

### **Redundância de Armazenamento**

A redundância é o mecanismo que garante a **alta disponibilidade e a durabilidade** dos dados, mesmo em caso de falhas de hardware ou desastres.

Alguns exemplos:

- **LRS (Locally Redundant Storage)**
    - Mantém cópias dentro do mesmo datacenter;
    - Datacenter individual na região primária.
- **ZRS (Zone-Redundant Storage)**
    - Três zonas de disponibilidade na região primária.
- **GRS (Geo-Redundant Storage)**
    - Replica os dados em outra região geográfica;
    - Datacenter único no primário e região secundária.
- **RA-GRS (Read-Access GRS)**: permite leitura mesmo quando a região principal está fora do ar.
    
    Essa escolha impacta diretamente no custo e na confiabilidade.
    
    | Tipo de Redundância | Replicação | Proteção contra falha regional? | Latência |
    | --- | --- | --- | --- |
    | **LRS** (Locally Redundant) | 3 cópias em **um** datacenter | ❌ Não | 🔵 Baixa |
    | **ZRS** (Zone-Redundant) | 3 cópias em **zonas da mesma região** | ❌ Não (só dentro da região) | 🔵 Baixa |
    | **GRS** (Geo-Redundant) | 6 cópias (3 na região primária + 3 em outra região) | ✅ Sim | 🟠 Maior para acesso secundário |
    | **RA-GRS** (Read-Access GRS) | Igual ao GRS, mas com leitura no secundário | ✅ Sim | 🟠 Maior |

---

### **Serviços de Armazenamento do Azure**

Cada serviço foi criado para um tipo específico de dado ou aplicação:

- **Blob Storage**: armazena grandes volumes de dados **não estruturados**, como vídeos, imagens, backups e arquivos de log. É ideal para conteúdo acessado via internet.
- **Disco do Azure**: fornece discos virtuais para máquinas virtuais, bancos de dados ou aplicativos que precisam de armazenamento permanente e rápido.
- **Fila (Queue)**: permite o envio e armazenamento de mensagens para comunicação entre sistemas, útil para aplicativos distribuídos que processam grandes volumes de mensagens.
- **Arquivos (File)**: cria um compartilhamento de arquivos de rede acessível por protocolo SMB, permitindo integração com sistemas Windows, Linux ou macOS.
- **Tabelas (Table)**: oferece armazenamento de dados estruturados no estilo NoSQL, ideal para aplicações que exigem escalabilidade sem estrutura fixa.

---

### **Camadas de Acesso**

O Azure permite escolher **camadas de acesso** que ajustam preço e desempenho conforme a frequência de uso dos dados:

- **Frequente (Hot)**: para dados acessados com frequência, com maior custo de armazenamento, mas menor custo de leitura.
- **Esporádico (Cool)**: para dados acessados ocasionalmente, com custo mais baixo para armazenar, mas mais caro para acessar.
- **Frio**: para dados acessados com pouca frequência e armazenado por pelo menos 90 dias.
- **Archive**: para dados raramente acessados (arquivos históricos, backups), com o menor custo de armazenamento, porém com maior tempo e custo de recuperação.

---

### **Migrações para o Azure**

Esse tópico aborda as ferramentas e estratégias para **mover dados de outros ambientes para o Azure**:

- **Plataforma de migração unificada**: reúne diferentes soluções de avaliação e migração em um só lugar.
- **Migrações para Azure**: serviços e ferramentas que ajudam a avaliar, planejar e executar a movimentação de grandes volumes de dados.

---

### **Azure Data Box**

O **Azure Data Box** é uma solução física para transferir grandes quantidades de dados (até 80 TB) para o Azure quando a conexão de internet é lenta ou inexistente.

- O cliente recebe uma caixa segura para copiar seus dados localmente.
- A caixa é então devolvida à Microsoft, que carrega os dados diretamente no Azure.
- Ideal para migrações de backup ou quando há necessidade de conformidade regulatória.

---

### **Opções de Gerenciamento de Arquivos**

Ferramentas que facilitam o controle, a movimentação e a sincronização de arquivos:

- **AzCopy**: utilitário de linha de comando para copiar dados de ou para uma conta de armazenamento. Funciona em uma única direção e é ideal para automações.
- **Gerenciador de Armazenamento do Azure**: ferramenta gráfica parecida com o Windows Explorer, disponível para Windows, Linux e macOS, que permite gerenciar arquivos de forma visual.
- **Sincronização de Arquivos do Azure**: mantém arquivos sincronizados entre servidores locais e o Azure. Permite que apenas os arquivos mais acessados fiquem localmente, economizando espaço.

---

## 🔑 **Identidade, Acesso e Segurança**

O Azure oferece um conjunto de serviços para garantir que apenas **usuários e dispositivos confiáveis** possam acessar recursos, além de permitir um **gerenciamento centralizado** de permissões.

### **Microsoft Entra ID**

- É a solução de **Identity and Access Management (IAM)** baseada em nuvem da Microsoft.
- Permite criar **usuários, grupos e políticas de segurança**, integrando-se a aplicativos SaaS (ex.: Office 365, Salesforce).
- Funcionalidades principais:
    - **Autenticação**: garante que apenas usuários legítimos acessem os recursos.
    - **Logon Único (SSO)**: um único login para acessar vários serviços (como Teams, Outlook e SharePoint).
    - **Gerenciamento de aplicativos**: controle de acesso a aplicativos internos ou externos.
    - **Gerenciamento de dispositivos**: registro e monitoramento de dispositivos que acessam a rede.
    - **Colaboração B2B**: convida parceiros e fornecedores externos para trabalhar com segurança em ambientes compartilhados.
- **Exemplo**: uma empresa pode integrar seu Active Directory local ao Entra ID para permitir autenticação híbrida entre o data center e a nuvem.

---

### **Microsoft Entra Domain Services**

- Fornece **serviços de domínio** (como ingressar máquinas em domínio, autenticação Kerberos/NTLM e políticas de grupo) **sem precisar de controladores de domínio físicos**.
- Ideal para **aplicações legadas** que não suportam autenticação moderna.
- **Exemplo**: migrar um sistema antigo que depende de LDAP para a nuvem sem reescrever o código.

---

### **Métodos de Autenticação**

1. **SSO (Single Sign-On)**
    - Usuários fazem login **uma única vez** e acessam múltiplos aplicativos sem inserir credenciais repetidamente.
    - Reduz risco de phishing, pois há menos logins.
2. **MFA (Multi-Factor Authentication)**
    - Requer **dois ou mais fatores**:
        - Algo que você **sabe** (senha, PIN).
        - Algo que você **possui** (token, celular, aplicativo Microsoft Authenticator).
        - Algo que você **é** (biometria como impressão digital ou reconhecimento facial).
    - **Exemplo**: login no portal do Azure pedindo senha + código no celular.
3. **Autenticação sem senha**
    - Usa métodos como **Windows Hello**, **chaves de segurança FIDO2** ou aplicativo Authenticator para evitar senhas.

---

### **Identidades Externas (B2B e B2C)**

- **B2B (Business to Business)**: permite colaboração com **parceiros externos** sem necessidade de criar contas internas.
- **B2C (Business to Consumer)**: permite que **clientes** façam login em aplicativos usando suas contas sociais (Google, Facebook, etc.).

---

### **Acesso Condicional**

- Cria **políticas automáticas** para determinar **quando e como** os usuários podem acessar recursos.
- Fatores considerados:
    - Localização geográfica (ex.: bloqueio de logins de países suspeitos).
    - Tipo de dispositivo (ex.: permitir apenas dispositivos corporativos).
    - Detecção de risco (ex.: bloquear login em caso de atividade incomum).
- **Exemplo**: exigir MFA apenas para logins fora da rede corporativa.

---

### **Controle de Acesso Baseado em Função (RBAC)**

- Permite **atribuir permissões específicas** para cada função ou grupo.
- Princípio de **menor privilégio**: usuários recebem **apenas o acesso necessário** para realizar suas tarefas.
- Funções comuns:
    - **Owner (Proprietário)**: controle total dos recursos.
    - **Contributor (Colaborador)**: cria e gerencia recursos, mas não gerencia permissões.
    - **Reader (Leitor)**: apenas leitura dos recursos.

---

### **Confiança Zero (Zero Trust)**

- **Princípio**: nunca confiar automaticamente em nenhum usuário, dispositivo ou rede, **mesmo que já esteja dentro da organização**.
- Cada requisição deve ser autenticada, autorizada e validada em tempo real.
- Componentes principais:
    - **Verificar explicitamente** cada acesso.
    - **Usar o menor privilégio possível**.
    - **Assumir violação** (monitorar continuamente).

---

### **Defesa em Profundidade**

- Modelo de **segurança em camadas** para proteger ambientes de TI.
- Camadas típicas:
    1. **Perímetro** (firewalls, proteção DDoS).
    2. **Rede** (segmentação, criptografia).
    3. **Computação** (patches, antivírus).
    4. **Aplicações** (validação de entrada, segurança de APIs).
    5. **Dados** (criptografia, backup).
- **Benefício**: mesmo que uma camada seja violada, as demais continuam protegendo.

---

### **Microsoft Defender para Nuvem**

- Serviço de **monitoramento de segurança** que protege recursos em **Azure, ambientes híbridos e multi-nuvem**.
- Principais recursos:
    - **Recomendações de segurança** para corrigir vulnerabilidades.
    - **Detecção e bloqueio de malware** em tempo real.
    - **Controle de acesso Just-in-Time (JIT)**: abre portas de rede apenas quando necessário.
    - Integração com **Azure Policy** para automatizar conformidade.
- **Exemplo**: detectar atividades suspeitas em uma VM e aplicar correções automáticas.

--- 

## Gerenciamento de Custos

O foco é como controlar, prever e otimizar custos e como organizar recursos para governança e cobrança no Azure. Conceitos-chave: **fatores que influenciam custo**, **Calculadora de Preços**, **Calculadora TCO**, **Azure Marketplace**, **Ferramentas de Gerenciamento de Custos (budgets, alertas, recomendações)** e **tags (marcas)**.

### Fatores que afetam os custos (explicação e impacto)

Principais fatores e por que importam:

- **Região (data center):** preços variam por região — latência, custos operacionais e disponibilidade de serviços mudam o valor.
- **Tipo e tamanho do recurso:** VMs (CPU/RAM), tipos de disco (HDD vs SSD), IOPS, e tipos de instância (spot/reserved) alteram o preço.
- **Uso/tempo de execução:** recursos cobrados por hora ou por segundo; escalonamento automático (autoscale) pode reduzir/elevar custos conforme demanda.
- **Tráfego de rede (egresso):** saída de dados da nuvem geralmente é cobrada; arquiteturas que transferem muitos dados aumentam custo.
- **Redundância e SLA:** optar por zonas de disponibilidade, regiões emparelhadas ou redundância geográfica aumenta custo.
- **Licenciamento e softwares adicionais:** licenças embarcadas (ex.: SQL Server) ou BYOL (bring your own license) mudam o custo.
- **Opções de compra:** preços sob demanda vs. **Reserved Instances** / **Savings Plans** / VMs Spot. Reservas reduzem custo se o uso for previsível.
- **Planos de suporte e contratos:** suporte pago (Standard/Professional Direct) agrega custo mensal/porcentagem.

**Implicação prática:** ao estimar custos, liste todas as decisões arquiteturais acima — cada escolha tem trade-offs entre preço, desempenho e disponibilidade.

### Azure Marketplace

O Azure Marketplace é um catálogo onde clientes encontram, testam, compram e provisionam soluções de fornecedores (imagens de VM, containers, SaaS, ferramentas de devops etc.). Uso típico:

- Encontrar imagens pré-configuradas (VM + software).
- Provisionar soluções de terceiros com faturamento consolidado.
- Permite acelerar projetos com padrões prontos (há milhares de ofertas).

Boas práticas: verificar modelo de cobrança do marketplace (licença inclusa ou separada), revisar SLAs do provedor e testar em ambiente de desenvolvimento antes de produção.

### Calculadora de Preços (Price Calculator)

O que faz: ajuda a **estimar** o custo de combinações de serviços antes do consumo real. Permite configurar opções por recurso (região, tamanho, camadas, horas, suporte, ofertas de dev/test).

Como usar (passos práticos):

1. Escolher serviços (ex.: Virtual Machines, Storage, Bandwidth).
2. Configurar região, tamanho/sku, e quantidades.
3. Ajustar horas previstas de uso (por ex., 24h x dias do mês).
4. Aplicar descontos previstos (reservas) ou promoções.
5. Exportar estimativa (CSV/PDF) para apresentar ao time financeiro.

Observação: **é uma estimativa** — custos reais dependem do uso real e de variações como transferência de dados e snapshots.

### Calculadora TCO (Total Cost of Ownership)

Propósito: comparar o custo atual de infraestrutura on-premises com o custo esperado se migrar para Azure — inclui servidores, licenças, manutenção, energia, espaço físico, pessoas.

O relatório TCO fornece estimativa de economia potencial e destaca áreas de economia (ex.: consolidação de servidores, redução de custo operacional).

Como interpretar: verifique premissas (nº de máquinas, CPU, RAM, utilização). TCO é útil para justificar migrações para a diretoria, mas depende muito da qualidade dos dados de entrada.

### Ferramenta de Gerenciamento de Custos do Azure (Cost Management + Billing)

Funcionalidades essenciais:

- **Análise de custos (Cost analysis):** visualizar gastos por período, por recurso, por tag, por grupo de recursos ou por assinatura.
- **Orçamentos (Budgets):** criar valores máximos e gatilhos (por ex., 80% do orçamento) e iniciar ações (emails, webhooks).
- **Alertas:** notificar equipes quando gastos atingem thresholds.
- **Recomendações de custo (Cost recommendations):** sugerem direitos de dimensionamento (rightsizing), compra de reservas, desligamento de recursos inativos.
- **Relatórios de cobrança & enriquecimento de dados:** exportar faturas, logs e integrar com BI/ERP.

Dica prática: combine **tags** com Cost Analysis para chargeback/showback por projeto ou centro de custo.

### Marcas (Tags) — organização e cobrança

O que são: pares **nome:valor** aplicados a recursos do Azure para categorizar (ex.: `env:prod`, `costCenter:CC123`, `owner:fulano`). Úteis para filtrar relatórios e agrupar custos.

Boas práticas:

- Defina uma **taxonomia** (nomenclatura padrão) antes de aplicar.
- Use tags para **ambiente**, **projeto**, **centro de custo**, **dono**.
- **Implemente Azure Policy** para obrigar tags na criação de recursos.
- Não coloque dados sensíveis (PII) nas tags.
- Limite número de tags relevantes e as padronize (ex.: `Environment` em vez de `env` misturado).

Observação: tags não são herdadas automaticamente por sub-resources — planeje aplicação via templates/automation.

### Relatórios, exportação e integração

- **Exports**: exporte faturas e uso em arquivos CSV/JSON para análises externas.
- **APIs**: integração programática permite automação de relatórios e integração com sistemas financeiros.
- **Enriquecimento de dados**: adicionar campos contextuais (tags, propriedades) para relatórios mais úteis.

### Recomendações operacionais e de governança

- **Defina escopos de cobrança** (cada subscription para ambiente / projeto).
- **Use management groups** para hierarquizar políticas e controles.
- **Políticas (Azure Policy)**: impor naming conventions, exigir tags, bloquear SKUs caros.
- **Automação**: shutdown programado de VMs de dev/test fora do horário para economizar.
- **Reservas e Savings Plans**: avaliar se o padrão de uso justifica compra antecipada.
- **Monitoramento contínuo**: dashboards de custo e alertas configurados com threshold razoáveis.

 ---

## Governança e Conformidade

### Visão geral — objetivo

Governança no Azure é o conjunto de políticas, processos e controles que garantem que os recursos na nuvem sejam criados, configurados e gerenciados conforme regras da organização (segurança, conformidade, custo, operações). Os principais instrumentos que você precisa conhecer:

- **Azure Policy** (impor padrões e avaliar conformidade).
- **Bloqueios de recurso** (proteger contra exclusão/modificação acidental).
- **Azure Blueprints** (pacotes repetíveis para implantar ambientes conformes).
- **Portal de Confiança do Serviço** (documentação e relatórios de conformidade).
- **Microsoft Purview** (governança e classificação de dados).

---

### Azure Policy — o que é e como usar

**O que é:** ferramenta para impor padrões em larga escala e avaliar conformidade de recursos (por exemplo: exigir tags, bloquear SKUs, exigir que recursos fiquem em determinadas regiões).

**Componentes:**

- **Policy definition**: regra individual (JSON) que descreve o que é permitido/proibido.
- **Initiative / Policy Set**: conjunto de policies agrupadas para facilitar atribuição.
- **Assignment**: aplicar uma policy/initiative a um escopo (subscription, resource group, management group, recurso).
- **Effects**: `Deny`, `Audit`, `Append`, `Modify`, `DeployIfNotExists`, `Disabled` (comportamentos que a policy pode executar/registrar).

**Casos práticos:** exigir `tag: costCenter`, negar criação de VMs em SKU X, auditar databases sem criptografia.

---

### Bloqueios de recurso (Resource Locks)

**O que fazem:** evitam exclusão ou alterações acidentais em recursos críticos. Aplicáveis ao nível de subscription, resource group ou recurso.

**Tipos:**

- **CanNotDelete** — recurso não pode ser deletado (mas pode ser modificado).
- **ReadOnly** — impede alterações (equivalente a “somente leitura”: não é possível excluir nem alterar).

---

### Azure Blueprints

**O que é:** mecanismo para empacotar e implantar de forma repetível um conjunto de artefatos necessários para um ambiente conformado. Pense em Blueprint como *template de governança + deploy*.

**Artefatos típicos:**

- Role assignments (RBAC)
- Policy assignments
- ARM templates (recursos a serem criados)
- Resource groups

**Vantagem:** versionamento de pacotes, aplicação consistente em múltiplas subscriptions, acelera provisionamento de ambientes conformes.

**Quando usar:** criar padrões para *environments* (dev/test/prod) com políticas, roles e recursos pré-configurados.

---

### Microsoft Purview (governança de dados)

**O que é:** solução para governança de dados corporativos — descoberta, classificação, catálogo e linhagem de dados em ambientes on-premises e multi-cloud.

**Funcionalidades chave:**

- Varredura/scan de fontes (storage, DBs, SaaS).
- **Classificação automática** de dados sensíveis (PII, números de cartão, etc.).
- **Data lineage** (quem/que transformou o dado ao longo do tempo).
- Catálogo unificado e glossário de negócios.

**Caso prático:** executar scan em um storage account e aplicar política de classificação para identificar arquivos que contenham números de CPF.

---

### Portal de Confiança do Serviço (Service Trust / Microsoft Trust Center)

**O que fornece:** documentação, relatórios de auditoria (SOC, ISO), guias de conformidade e informações sobre segurança e privacidade do Azure — útil para comprovar conformidade em auditorias e para due diligence.

**Uso prático:** baixar relatórios de auditoria, consultar escopos de conformidade por região e para serviços específicos

---

### Padrões e boas práticas de governança

- **Hierarquia:** use *management groups* → *subscriptions* → *resource groups* para organizar políticas e delegação.
- **RBAC** para controlar quem pode fazer o quê (funções built-in ou custom).
- **Policies** para controlar o quê pode ser criado/como configurado.
- **Tags** para chargeback/showback e relatórios de custo.
- **Locks** para proteger recursos críticos.
- **Blueprints** para implantar ambientes padronizados.
- **Automação**: desligamento automático de VMs de dev/test, scripts para aplicar tags, policy remediation.
- **Monitoramento & Cost Management**: dashboards e budgets para evitar surpresas.

**Regra prática simples:** RBAC = *quem*, Policy = *o que/como*, Locks = *impedir exclusão/modificação*, Blueprints = *empacotar e implantar padrão*.

---

### Comparativo rápido (útil para prova)

- **RBAC**: controla permissões (ex.: usuário pode criar VMs).
- **Azure Policy**: impõe regras em recursos (ex.: impedir criação de VMs em regiões não permitidas).
- **Resource Lock**: evita remoção/alteração acidental.
- **Blueprint**: modelo completo (resources + policies + roles) para implantar ambiente.
- **Management Group**: organiza subscriptions em tiers para aplicar políticas/controle centralizado.

---

### Hands-on sugeridos (passo a passo curto)

1. Criar uma **policy** que exige tag `project` e atribuí-la a uma subscription; testar criando recurso sem tag (deve ser `Deny`/`Audit`).
2. Criar um **resource group** e aplicar um **lock CanNotDelete**; tente excluir o RG (falhará) e remova o lock para permitir exclusão.
3. Criar um **blueprint** simples que defina um resource group + policy + role assignment e atribuí-lo a uma subscription.
4. No **Microsoft Purview**, configure um scan para um storage account (ou simule via demo) e analise categorias classificadas automaticamente.
5. Consultar o **Portal de Confiança** para localizar um relatório SOC ou ISO relacionado a um serviço Azure.
