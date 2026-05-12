# 🪙 Sistema de Moeda Estudantil

<p align="center">
<img src="https://img.shields.io/badge/status-Em%20Desenvolvimento-yellow?style=for-the-badge"/>
<img src="https://img.shields.io/badge/versão-1.0.0-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/licença-MIT-green?style=for-the-badge"/>
</p>


---

## 💡 Sobre o Projeto

O **Sistema de Moeda Estudantil** é uma plataforma acadêmica que permite que professores
reconheçam o desempenho e comportamento de seus alunos por meio de **moedas virtuais**.
Os alunos podem acumular essas moedas e trocá-las por **vantagens oferecidas por
empresas parceiras**, como descontos em restaurantes, mensalidades e materiais.

O sistema conecta quatro atores principais: **Instituições de Ensino**,
**Professores**, **Alunos** e **Empresas Parceiras**, promovendo um
ecossistema de reconhecimento e benefícios.

---

## ✅ Funcionalidades

### 🎓 Aluno
- [x] Cadastro com dados pessoais e acadêmicos
- [x] Login e autenticação
- [x] Recebimento de moedas de professores
- [x] Notificação por email ao receber moedas
- [x] Consulta de extrato (saldo + histórico)
- [x] Troca de moedas por vantagens
- [x] Recebimento de cupom com código único por email

### 👨‍🏫 Professor
- [x] Login e autenticação (pré-cadastrado pela instituição)
- [x] Recebimento automático de 1.000 moedas por semestre
- [x] Envio de moedas a alunos com mensagem de motivo
- [x] Consulta de extrato (saldo + histórico de envios)

### 🏢 Empresa Parceira
- [x] Cadastro no sistema
- [x] Login e autenticação
- [x] Cadastro de vantagens (com descrição, foto e custo em moedas)
- [x] Notificação por email ao ter vantagem resgatada

### 🏫 Instituição de Ensino
- [x] Pré-cadastrada no sistema
- [x] Envio de lista de professores no momento da parceria

---

## 👥 Atores do Sistema

| Ator | Descrição |
|------|-----------|
| 🎓 **Aluno** | Usuário que recebe e troca moedas por vantagens |
| 👨‍🏫 **Professor** | Distribui moedas como reconhecimento aos alunos |
| 🏢 **Empresa Parceira** | Oferece vantagens em troca de moedas dos alunos |
| 🏫 **Instituição de Ensino** | Entidade pré-cadastrada que vincula professores e alunos |


---

## 📖 Histórias do Usuário

| ID | Ator | História | Prioridade |
|----|------|----------|------------|
| HU-01 | Aluno | Como aluno, quero me cadastrar no sistema para acessar a plataforma de mérito
| HU-02 | Aluno | Como aluno, quero consultar meu extrato para acompanhar meu saldo e histórico 
| HU-03 | Aluno | Como aluno, quero trocar moedas por vantagens disponíveis no sistema 
| HU-04 | Aluno | Como aluno, quero ser notificado por email ao receber moedas de um professor 
| HU-05 | Professor | Como professor, quero enviar moedas a um aluno com mensagem de reconhecimento 
| HU-06 | Professor | Como professor, quero consultar meu extrato para ver meu saldo e histórico de envios 
| HU-07 | Professor | Como professor, quero receber 1.000 moedas automaticamente a cada semestre 
| HU-08 | Empresa | Como empresa, quero me cadastrar e adicionar vantagens para os alunos resgatarem
| HU-09 | Empresa | Como empresa, quero ser notificada quando um aluno resgatar minha vantagem 
| HU-10 | Aluno | Como aluno, quero visualizar o catálogo completo de vantagens disponíveis no sistema, para que eu possa planejar como gastar minhas moedas e me motivar a conquistar mais.
| HU-11 | Aluno | Como aluno, quero consultar o histórico das minhas vantagens resgatadas, incluindo cupons e datas de resgate, para que eu possa acompanhar e gerenciar os benefícios já utilizados.
| HU-12 | Empresa | Como empresa parceira, quero editar ou desativar as vantagens que cadastrei no sistema, para que eu possa manter as ofertas atualizadas conforme a disponibilidade dos meus produtos ou serviços.







---



## 🗂️ Estrutura de Classes

| Classe | 
|--------|
| `Usuario` 
| `Aluno` 
| `Professor` 
| `EmpresaParceira` 
| `InstituicaoEnsino` 
| `Transacao` 
| `EnvioMoedas` 
| `ResgateVantagem` 
| `Vantagem` 
| `Cupom` 
| `Notificacao` 

---

## 🛠️ Tecnologias

> ⚠️ *As tecnologias serão definidas conforme o avanço do projeto.*

| Camada | Tecnologia  |
|--------|-------------------|
| Back-end |SpringBoot    |
| Front-end |React |
| Banco de Dados |MySQL  |


---

## 🚀 Como Executar

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/sistema-de-merito.git

# Entre na pasta do projeto
cd sistema-de-merito

# Instale as dependências
./mvnw install

# Configure as variáveis de ambiente
cp .env.example .env

# Execute o projeto
./mvnw spring-boot:run
```

> 📌 Certifique-se de configurar as variáveis de banco de dados e SMTP no arquivo `.env`

---

## 📁 Estrutura de Pastas

```
sistema-de-merito/
├── 📁 diagramas/
│   ├── diagrama-casos-de-uso.xml
│   └── diagrama-classes.xml
├── 📁 docs/
│   └── historias-usuario.md
├── 📁 src/
│   ├── 📁 main/
│   │   ├── 📁 java/
│   │   │   └── 📁 com/sistemamerito/
│   │   │       ├── 📁 model/
│   │   │       ├── 📁 service/
│   │   │       ├── 📁 controller/
│   │   │       └── 📁 repository/
│   │   └── 📁 resources/
│   └── 📁 test/
├── .env.example
├── pom.xml
└── README.md
```

---

## 🤝 Contribuição

1. Faça um **fork** do projeto
2. Crie uma **branch** para sua feature
 ```bash
 git checkout -b feature/minha-feature
 ```
3. Faça o **commit** das suas alterações
 ```bash
 git commit -m "feat: adiciona minha feature"
 ```
4. Faça o **push** para a branch
 ```bash
 git push origin feature/minha-feature
 ```
5. Abra um **Pull Request**

---

## 📝 Licença

Este projeto está sob a licença **MIT**.
Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<p align="center">
Desenvolvido por David Olinda e Jonas 
</p>
