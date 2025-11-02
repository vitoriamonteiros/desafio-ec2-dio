# ☁️ Desafio EC2 - DIO  

## 📘 Descrição  
Este repositório documenta a prática realizada sobre **instâncias EC2 na AWS**, com o objetivo de aplicar os conceitos aprendidos no curso e registrar o processo de forma organizada.  

---

## 🎯 Objetivos  
- Criar e gerenciar uma **instância EC2**.  
- Criar e utilizar **AMIs**.  
- Criar **Snapshots EBS** para backup.  
- Praticar a documentação no **GitHub**.  

---

## 🧭 Passo a Passo  

**1️⃣ Criar uma instância EC2**  
- Acesse o console da AWS.  
- Clique em **“Launch Instance”**.  
- Escolha a AMI (ex.: Amazon Linux 2) e o tipo de instância (`t2.micro`).  

**2️⃣ Configurar o grupo de segurança**  
- Permitir **SSH (porta 22)** para Linux ou **RDP (porta 3389)** para Windows.  

**3️⃣ Acessar a instância**  
- **Linux:**  
  ```bash
  ssh -i chave.pem usuario@ip-publico
