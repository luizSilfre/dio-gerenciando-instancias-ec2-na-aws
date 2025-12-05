# **Gerenciando Instâncias EC2 na AWS: Desafio Prático (Bootcamp TQI - DIO)**

Este repositório contém minhas anotações, insights e diagramas produzidos durante o laboratório do curso **"Gerenciando Instâncias EC2 na AWS"**, parte do bootcamp **TQI – Modernização com GenAI**. O objetivo deste desafio é consolidar os conceitos estudados, documentar o processo e criar um material de referência claro, organizado e útil para consultas futuras.

---

## 🎯 **Objetivos do Desafio**

- ✔️ Aplicar conceitos fundamentais de gerenciamento de instâncias EC2  
- ✔️ Documentar processos técnicos de forma clara e estruturada  
- ✔️ Utilizar o GitHub como ferramenta de versionamento e compartilhamento  
- ✔️ Criar diagramas de arquitetura representando cenários reais  

---

## 📚 **Referências Utilizadas**

- **AMIs no Amazon EC2**  
  https://docs.aws.amazon.com/pt_br/toolkit-for-visual-studio/latest/user-guide/tkv-ec2-ami.html

- **Funcionamento de snapshots no EBS**  
  https://docs.aws.amazon.com/pt_br/ebs/latest/userguide/how_snapshots_work.html
  
- **Aulas do curso**  


---

## 🧠 **Principais Conceitos Aprendidos**

### 🔹 **1. AMIs (Amazon Machine Images)**
Permitem inicializar novas instâncias EC2 com configurações pré-definidas: sistema operacional, pacotes, drivers e aplicações.

### 🔹 **2. EBS Snapshots**
Snapshots são cópias incrementais de volumes EBS, úteis para backup, replicação e criação de novos volumes.

### 🔹 **3. Arquiteturas Práticas Criadas no Laboratório**
Durante o laboratório, foram desenvolvidos diagramas representando cenários reais utilizando EC2, RDS, S3, DynamoDB e Lambda.

As imagens estão na pasta `/images`.

---

## 🏗️ **Diagramas Produzidos**

### 📌 **1. Arquitetura de Armazenamento com S3, DynamoDB e Lambda**

![Diagrama — Armazenamento S3, DynamoDB e Lambda](/images/Desafio%20S3%20-%20Simple%20Application.drawio.png)

### 📌 **2. Arquitetura de Aplicação Utilizando EC2 e RDS**

![Diagrama — Aplicação com EC2 e RDS](/images/Desafio%20EC2%20-%20Simple%20Application.drawio.png)

---

## ⚙️ **Atividades Práticas Realizadas**

- Criação e gerenciamento de instâncias EC2  
- Configuração de Security Groups  
- Criação e restauração de snapshots  
- Criação de AMIs personalizadas  
- Associação de volumes EBS  
- Desenho de arquiteturas na nuvem  
- Documentação técnica do processo  

---

## 📁 **Estrutura do Repositório**

```
/
├── README.md
├── images/
│   ├── Desafio S3 - Simple Application.drawio.png
│   └── Desafio EC2 - Simple Application.drawio.png
└── anotacoes/
    └── notas_estudo.md
```

---

## 📝 **Notas de Estudo**
As anotações detalhadas realizadas durante a prática estão disponíveis em:  
➡️ **[Notas de Estudo](/anotacoes/notas_estudo.md )**

---

## 🚀 **Conclusão**
Este desafio reforçou conceitos essenciais de EC2, AMIs, snapshots e boas práticas de gerenciamento. Um passo importante dentro da minha jornada no bootcamp **TQI – Modernização com GenAI**.

Se este material ajudar outros estudantes, já valeu a pena! 🚀