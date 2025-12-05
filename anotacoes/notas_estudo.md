# **Notas de Estudo: Gerenciando Instâncias EC2 na AWS**

Estas notas reúnem pontos importantes, conceitos, insights e observações feitas durante o laboratório do curso **"Gerenciando Instâncias EC2 na AWS"**, parte do bootcamp **TQI – Modernização com GenAI**. Elas servem como guia de estudo, revisão rápida e apoio para futuras implementações.

---

## 🖥️ **1. Amazon EC2: Conceitos Fundamentais**

### 🔸 O que é EC2?
- Serviço de computação escalável da AWS.  
- Permite criar servidores virtuais (instâncias) sob demanda.  

### 🔸 Tipos de Instâncias
- General Purpose  
- Compute Optimized  
- Memory Optimized  
- Storage Optimized  
- Accelerated Computing  

Cada tipo atende um perfil de aplicação específico.

### 🔸 Ciclo de Vida de Instâncias
- **Pending → Running → Stopping/Stopped → Terminated**
- Estado influencia custos e uso de recursos.

---

## 📦 **2. AMIs: Amazon Machine Images**

### 🔸 O que é uma AMI?
Uma AMI contém:
- Sistema operacional  
- Drivers  
- Configurações e pacotes pré-instalados  
- Softwares opcionais  

### 🔸 Por que criar uma AMI?
- Replicar ambientes rapidamente  
- Facilitar escalabilidade horizontal  
- Criar backups completos de configuração  

### 🔸 Processo de Criação
1. Configurar a instância EC2 como desejado.  
2. Acessar o console e selecionar **Create Image**.  
3. Definir nome, descrição e volumes associados.  
4. AMI gerada disponível para lançar novas instâncias.  

### 🔸 Observações Importantes
- AMIs podem ser compartilhadas entre contas.  
- É possível copiar AMIs entre regiões.  
---

## 🗄️ **3. EBS: Elastic Block Store**

### 🔸 O que é EBS?
- Armazenamento em blocos para EC2.  
- Persistência mesmo após desligamento da instância.

### 🔸 Tipos de EBS
- gp3: Uso geral  
- io2/io1: Alto desempenho IOPS  
- st1: Otimizado para throughput  
- sc1: Baixo custo, baixa frequência de acesso  

### 🔸 Anexando e Desanexando Volumes
- Um volume pode ser anexado a uma instância por vez.  
- Ideal para expandir armazenamento ou substituir volumes.

---

## 📸 **4. Snapshots: Cópias Incrementais de Volumes**

### 🔸 Como Funcionam
- Copiam somente blocos alterados desde o snapshot anterior.  
- Armazenados no Amazon S3 de forma gerenciada.  
- Podem ser utilizados para recriar volumes ou gerar AMIs.

### 🔸 Ciclo de Backup
1. Criar snapshot manualmente ou por política automatizada.  
2. Armazenamento incremental reduz custos.  
3. Pode ser copiado entre regiões.

### 🔸 Casos de Uso
- Recuperação de desastres  
- Migração entre regiões  
- Versionamento de volumes  

---

## 🧩 **5. Security Groups e Regras de Acesso**

### 🔸 Características
- Atuam como firewall virtual.  
- Regras de entrada e saída baseadas em portas, protocolos e IPs.  

### 🔸 Boas Práticas
- Evitar portas abertas para 0.0.0.0/0 quando possível.  
- Criar regras específicas para cada ambiente (dev, hml, prod).  

---

## 🏗️ **6. Arquiteturas Criadas no Laboratório**

Nos exercícios foram criadas arquiteturas integrando EC2, S3, RDS, DynamoDB e Lambda.

Diagramas disponíveis no diretório `/images` do repositório.

---

## 📝 **7. Insights Pessoais**

- AMIs são extremamente úteis para padronização de ambientes.  
- Snapshots oferecem segurança e simplicidade no backup.  
- Criar diagramas ajuda a fixar conceitos e visualizar fluxo de dados.  
- O laboratório reforça como pequenos detalhes, como regras de SG e tamanho de volume, fazem grande diferença.

---

## 🚀 **8. Próximos Passos**

- Criar AMIs automatizadas usando Lambda + EventBridge.  
- Testar replicação de snapshots entre regiões.  
- Montar pipelines de infraestrutura com Terraform ou CloudFormation.  

---

Essas notas servirão como reforço para estudos futuros e como base para práticas mais avançadas em computação na nuvem usando AWS.