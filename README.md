# Bolt Account Creator API

![Status](https://img.shields.io/badge/status-operational-brightgreen)
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Node](https://img.shields.io/badge/node-18.x-green)
![License](https://img.shields.io/badge/license-MIT-orange)

API automatizada para criação de contas na plataforma bolt.new com processamento eficiente e interface simplificada.

## ✨ Principais Funcionalidades

- 🤖 Criação automatizada de contas bolt.new
- 📧 Geração e gerenciamento de emails temporários
- ✅ Confirmação automática via captura de links de verificação
- 🔄 Sistema de fallback para maior resiliência
- 🌐 Interface RESTful para fácil integração

## 🛠️ Tecnologias

- **Backend**: Node.js, Express
- **Automação**: Puppeteer
- **Email**: API Temp Mail Solutions
- **Implantação**: Railway (Backend)
- **Containerização**: Docker

## 🔌 Endpoints

### `GET /api/status`

Verifica o status do serviço e disponibilidade.

### `POST /api/create-account`

Cria uma nova conta bolt.new e retorna as credenciais.

**Resposta de sucesso**:

```json
{
  "success": true,
  "accountInfo": {
    "email": "user12345@example.com",
    "username": "user_abc123",
    "password": "Pass_xyz789_123!",
    "confirmed": true
  }
}
```

## 🚀 Funcionamento

O sistema automatiza todo o fluxo de criação de contas:

1. Gera email temporário seguro
2. Preenche formulário de registro com dados aleatórios
3. Monitora caixa de entrada para receber confirmação
4. Processa links de verificação automaticamente
5. Retorna credenciais prontas para uso


## 👨‍💻 Autor

**[Noir]** - [Github](https://github.com/noir157)
