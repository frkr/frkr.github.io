---
title: WhatsApp com Inteligencia
layout: post
post-image: /assets/whatsapp.png
tags:
- WhatsApp
- Business
- IA
- Inteligencia
- Artificial
---

# Palavras Chave

- chat
- code
- image

---

###### chat

```
chat Crie um chatbot para o WhatsApp
```

###### Resposta

```
*Chatgpt:* _Texto a seguir é um BOT:_

Oi! Eu sou o seu chatbot para o WhatsApp. Estou aqui para ajudar você com qualquer dúvida que você possa ter. Por favor, diga-me o que você precisa e eu farei o meu melhor para ajudar.
```

---

###### code Java Crie um hello world 

```
chat Crie um chatbot para o WhatsApp
```

###### Resposta

```
Chatgpt: Texto a seguir é um BOT:
em Java.

java
public class HelloWorld {
public static void main(String[] args) {
System.out.println("Hello World!");
}
}


Compile o código:

bash
javac HelloWorld.java


Execute o código:

bash
java HelloWorld
```

---

# Exemplos

#### Chat Cliente

![Chat Cliente](/assets/cliente.jpg)

### Chat Telegram

![Chat Telegram](/assets/recebendo-telegram.png)

### Chat Slack

![Chat Slack](/assets/canaisslack.jpg)

---

![Chat Slack](/assets/msgsslack.jpg)

---

## Para o Facebook

| Passos | Descrição                                                                                                          | 
|--------|--------------------------------------------------------------------------------------------------------------------|
| 1      | Para recuperar mensagens ativas ou passivas, é necessário ter uma conta _Business_                                 |
| 2      | Criar um aplicativo é necessário para prover a API de integração Simples                                           |
| 3      | Algumas dicas de configuração. Adicionar um numero que *NÃO* tenha WhatsApp. A seção Webhook, deixar para o final. |
| 4      | Todos os dashboards, mensagens com templates e outros assuntos (como o status da linha)                            |
| 5      | Voltar a configurar a empresa para dar acesso a todos os recursos                                                  |
| 6      | Use uma linha virtual. Ou o IoT (M2M) da Vivo                                                                      |

---
###### Resumo: 

Para conseguir usar a API do WhatsApp, é necessário ter uma conta _Business_ no Facebook. Criar um aplicativo para prover a API de integração Simples. E então, amarrar um usuário de sistema com as permissões do WhatsApp ao aplicativo.

---

###### 1) [Meta Facebook Business](https://business.facebook.com/settings/)
###### 2) [Meta for Developers](https://developers.facebook.com/apps/create/)
###### 3) Configuração

![WhatsApp Config](/assets/whatsapp-config.png)
1. Adicionar produto
1. WhatsApp Business
1. Permissões e recursos - 2 permissões do WhatsApp
1. Começar - Etapa 5 - Adicionar Telefone
1. Configuração - Webhook

---
###### 4) [WhatsApp Business Manage](https://business.facebook.com/wa/manage/)
###### 5) Novamente na _Meta Facebook Business_

- Usuário de Sistema
- Apps
- Contas do WhatsApp
- Adicionar Método de Pagamento

###### 6) Uma linha de telefone virtual. Rapido e simples.
- [Linha de Telefone Virtual](https://www.linhavirtual.com.br/download)

# Por último, mas não menos importante

## [Pipedream](https://pipedream.com)

- Vai precisar de um _Permanent Access Token_ e um _Business Account ID_
- Usar também o _Authorization: Bearer_ no header

###### To connect your WhatsApp Business Cloud account to Pipedream, follow the below steps to find your Business Account ID and your Permanent Access Token:

### Business Account ID

- Sign in to the Facebook Business Manager for WhatsApp
- Find the account you want to use and click on it. A panel should open with information about the account, including the ID
- Copy that ID and paste it below

### Permanent Access Token

- Sign in to your Facebook Developer Account
- Select Apps Dashboard then Business Settings
- Select System Users then Add. Enter a username, select the role as Admin and click Create System User
- Select Add Assets then Apps. Select the app you want to assign to the user, enable Full Control access, and click Save Changes
- Select WhatsApp Accounts then Add People then Select the system user then Enable Full Control Access, and finally Assign
- Select System Users then Select the user, and Generate Access Token
- Select the app and enable whatsapp_business_messaging and whatsapp_business_management, and then click Generate Token
- And finally, paste that token below

For additional info on setting up a WhatsApp Business account, refer to their getting started docs.

---

# Bom, tem o ChatGPT

- [ChatGPT](https://platform.openai.com/docs/guides/completion)

```json
{
    "model": "text-davinci-003", 
    "temperature": 0,
    "max_tokens": 600,
    "top_p": 1,
    "frequency_penalty": 0.2,
    "presence_penalty": 0,
    "user": "" + user,
    "prompt": prompt,
}
```

```json
{
    "model": "code-davinci-002", 
    "max_tokens": 256
}
```
---
```bash
curl https://api.openai.com/v1/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -d '{
  "model": "text-davinci-001",
  "prompt": "Write a tagline for an ice cream shop.",
  "temperature": 0.4,
  "max_tokens": 64,
  "top_p": 1,
  "frequency_penalty": 0,
  "presence_penalty": 0
}'
```

# Notas:
- https://github.com/Wolox/react-chat-widget
- https://github.com/stuyy/chat-platform-react
- https://api.slack.com/bot-users
- https://core.telegram.org/bots