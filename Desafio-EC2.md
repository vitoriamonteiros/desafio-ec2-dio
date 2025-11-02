# Desafio EC2 - DIO

## Descrição
Este repositório é para documentar a prática realizada para o gerenciamento de instâncias EC2 na AWS, com objetivo é consolidar os conceitos aprendidos no curso, aplicando-os de forma prática e documentar. 

## Objetivos
- Aplicação de conceitos de criação, configuração e gerenciamento de instâncias EC2.
- Criar e utilizar AMIs para replicar ambientes.
- Criar Snapshots EBS para backup e recuperação de dados.
- Documentar processos técnicos de forma clara e organizada.
- Utilizar GitHub como ferramenta de documentação e compartilhamento de conhecimento.

## Passo a Passo da Atividade

### Passo 1. Criar uma instância EC2
- Acesse o console AWS EC2.
- Clique em “Launch Instance”.
- Escolha a Amazon Machine Image (AMI) desejada (Linux/Windows).
- Selecione o tipo de instância (ex.: t2.micro para testes gratuitos).

### Passo 2. Configurar o grupo de segurança (Security Group)
- Permitir acesso SSH (porta 22) para Linux ou RDP (porta 3389) para Windows.
- Configurar regras adicionais conforme necessidade (ex.: HTTP/HTTPS).

### Passo 3. Acessar a instância
- Para Linux: use `ssh -i chave.pem usuario@ip-publico`.
- Para Windows: utilize RDP com usuário e senha gerados.

### Passo 4. Trabalhar com AMIs
- Configurar a instância conforme necessário.
- Criar uma **AMI** da instância para replicação futura.
- Registrar o ID da AMI para uso posterior.

### Passo 5. Trabalhar com Snapshots EBS
- Criar **Snapshots EBS** dos volumes anexados à instância.
- Verificar tamanho, tipo de armazenamento e implicações de custo.
- Utilizar snapshots para backup e recuperação de dados.

### Passo 6. Monitoramento e otimização
- Verificar métricas básicas de CPU, memória e disco via CloudWatch.
- Considerar desligamento automático ou redução de tamanho da instância para otimização de custos.

## Conclusões:
- Aprendi como criar e gerenciar instâncias EC2 de forma prática.
- Entendi o modelo de responsabilidade compartilhada da AWS: a AWS gerencia a infraestrutura física, enquanto o usuário é responsável pelo sistema operacional e aplicações.
- Compreendi a importância de **AMIs e Snapshots EBS** para replicação de ambientes e backup de dados.
- Observações sobre otimização de custos: desligar instâncias quando não estiverem em uso e escolher o tipo certo de instância e volume EBS.
- O monitoramento contínuo é essencial para garantir desempenho adequado e controle de gastos.

## Referências
[Documentação AWS EC2](https://docs.aws.amazon.com/ec2/)
