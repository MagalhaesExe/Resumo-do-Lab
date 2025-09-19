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
