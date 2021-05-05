# zenvia-qualified-lead

Este repositório contém a aplicação criada no artigo tutorial da [Prensa.li](https://prensa.li/) sobre como [gerar leads qualificados](https://prensa.li/zenvia/como-gerar-leads-qualificados/).

## Como executar

### Cofiguração inicial

Para executar esta aplicação você precisa fazer o cadastro no [site da Zenvia](https://accounts.zenvia.com/login?state=hKFo2SB1QzNIYVBNMTRRZnoxV21EVHR6aTBsdlA3U0ZoRTBFOKFupWxvZ2luo3RpZNkgTmI3WmV5R0pfOGhXR1BGbGdyYW1sQmN1Yjh4VHpEQm6jY2lk2SBrTG1KQWh1eVFNQUdFR3ZPUkVGNVAxMzVPNmFRbXdmVg&client=kLmJAhuyQMAGEGvOREF5P135O6aQmwfV&protocol=oauth2&scope=openid%20profile%20email&response_type=code&response_mode=query&nonce=WW5tbWlRb3V0cnRuZkRCYTc1a2FxNmlHUWdxNDdyTldIYVhKM1Ntc1VLdg%3D%3D&redirect_uri=https%3A%2F%2Fapp.zenvia.com%3Fauth0Redirect%3Dsignin&code_challenge=_y9ZUwi9UCsEgucoPUZY8sXZWkJV8DiGngSo7alo0sk&code_challenge_method=S256&auth0Client=eyJuYW1lIjoiYXV0aDAtc3BhLWpzIiwidmVyc2lvbiI6IjEuMTIuMSJ9) e criar o fluxo que enviará as informações para que esta API receba e armazene.

### Requisitos

- [node.js](https://nodejs.org/en/download/) 8 ou versão superior
- [yarn](https://classic.yarnpkg.com/en/docs/install/#windows-stable) (opcional, mas altamente recomendado)

Para instalar o [yarn](https://classic.yarnpkg.com/en/docs/install/#windows-stable), basta rodar em algum terminal:

```bash
npm install -g yarn
```

### Executando o projeto

Clone o projeto:

```bash
git clone https://github.com/apiplaybook/zenvia-qualified-lead.git
```

Rode o comando de criação do banco de dados a partir do schema definido:

```bash
npx prisma migrate dev --name init --preview-feature
```

Após clonar o projeto e fazer as configurações necessárias, execute a API com o comando:

```bash
yarn dev
```

ou

```bash
npm run dev
```

Caso você for utilizar esta aplicação localmente e queira testar, será necessário expor a porta 3000 (se você executar a aplicação em outra porta, terá que expô-la). Para isso você pode usar o ngrok (mais informações no artigo na Prensa).
