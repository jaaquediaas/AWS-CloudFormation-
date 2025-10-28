# AWS-CloudFormation-
Projeto Base:  Infraestrutura automatizada com AWS CloudFormation.

## Objetivo
Este laboratório tem como objetivo implementar uma infraestrutura automatizada na AWS usando **CloudFormation**.  
A proposta é criar uma **instância EC2** de forma totalmente automatizada, aplicando o conceito de Infraestrutura como Código (IaC).

---

## Conceito
O **AWS CloudFormation** permite definir e provisionar recursos de nuvem usando **templates** (em JSON ou YAML).  
Com isso, toda a infraestrutura pode ser criada, atualizada ou removida de forma controlada e versionada.

---

## O que este template faz
- Cria **uma instância EC2** do tipo `t2.micro` (elegível ao Free Tier).  
- Define automaticamente um **nome (Tag)** para a instância.  
- Retorna o **ID da instância** como saída (Output).

---

## Como executar

1. Acesse o console da AWS.  
2. Vá até o serviço **CloudFormation**.  
3. Clique em **Create stack → With new resources (standard)**.  
4. Faça upload do arquivo `template.json`.  
5. Clique em **Next** até a tela de confirmação e depois em **Create stack**.  

Aguarde alguns minutos — a instância EC2 será criada automaticamente.

---

## 📦 Estrutura do projeto

├── template.json # Template CloudFormation

└── README.md # Documentação do laboratório


---

## Observações
- O **AMI ID** (`ami-0c02fb55956c7d316`) é válido na região **us-east-1**.  
  Caso use outra região, substitua por um AMI equivalente ao **Amazon Linux 2**.  
- Todos os recursos são elegíveis ao **Free Tier**.

---

## Conceitos praticados
- Infraestrutura como Código (IaC)
- Automação com AWS CloudFormation
- Criação e provisionamento de instância EC2
- Uso de templates JSON

---

## Autor
Projeto desenvolvido como exercício prático de AWS CloudFormation.

