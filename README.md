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
