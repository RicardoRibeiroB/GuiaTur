# 🌍 Projeto: Aplicativo de Turismo Regional com React Native e Node.js

## 📖 Sobre
Este projeto tem como objetivo desenvolver um sistema completo para **centralizar informações turísticas** de regiões do interior de São Paulo.  

O aplicativo permitirá que usuários **pesquisem e montem roteiros turísticos**, **compartilhem experiências**, **avaliem atrações e eventos** e interajam de forma colaborativa.  
Além disso, contará com um módulo administrativo para **gestores, promotores de eventos e empreendedores locais**.  

Com arquitetura escalável e foco em acessibilidade, o sistema busca **promover o turismo rural, cultural e corporativo**, apoiando tanto a população local quanto visitantes.

---

## 📂 Repositório
### Estrutura principal
- **turismo-frontend** → Aplicativo mobile em **React Native** (consultas, roteiros, experiências).  
- **turismo-backend** → API em **Node.js + Express**, com autenticação, banco de dados e lógica de negócios.  

---

## 🛠️ Ferramentas Utilizadas
- **Git**: Controle de versão  
- **VSCode**: Editor de código  
- **Postman / Thunder Client**: Testes de APIs  
- **Figma**: Prototipagem da interface  

---

## ⚙️ Tecnologias
### Frontend
- **React Native** `v0.74.x`  
- **Expo** (se aplicável)  
- **TypeScript** `v5.x`  
- **Firebase Auth** para autenticação  
- **Axios** para requisições  

### Backend
- **Node.js** `v22.x`  
- **Express** `v4.x`  
- **MongoDB** `v7.x`  
- **Mongoose** `v8.x`  
- **JWT** para autenticação  
- **Docker** para deploy (planejado)  

---

## 🚀 Como Rodar o Projeto  

### 🔧 Backend
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/turismo-backend.git
cd turismo-backend

# Instale as dependências
npm install

# Configure as variáveis de ambiente (.env)
PORT=4000
MONGO_URI=sua_string_de_conexao
JWT_SECRET=sua_chave_secreta

# Inicie o servidor
npm run dev
