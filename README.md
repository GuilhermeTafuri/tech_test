 *Upload e Processamento de PDFs com Armazenamento de CPFs 

## Descrição  
Esta aplicação oferece uma solução simples e eficiente para **fazer upload de PDFs**, **extrair e validar CPFs** contidos nesses arquivos, e **armazená-los no Firebase Realtime Database**. O processo é dividido em duas partes: o **frontend** permite o upload do arquivo, enquanto o **backend** processa o PDF para localizar os CPFs, valida-os e os armazena. Além disso, a aplicação permite visualizar **todos os CPFs já armazenados**, incluindo os recém-encontrados.

---

##  Funcionalidades  
- **Upload de PDFs**: O usuário pode fazer o upload de um arquivo PDF no frontend da aplicação.  
- **Processamento de PDF**: O backend lê o conteúdo do PDF e encontra todos os CPFs no formato `XXX.XXX.XXX-XX`.  
- **Validação de CPFs**: Valida os CPFs encontrados, verificando se estão no formato correto.  
- **Armazenamento no Firebase**: Todos os CPFs válidos são salvos no Firebase Realtime Database.  
- **Listagem de CPFs**: A aplicação exibe os CPFs recém-encontrados e todos os CPFs já armazenados no Firebase.  

---

##  Tecnologias Utilizadas
- **Frontend:** Vue, com Axios para fazer requisições HTTP ao backend.  
- **Backend:** Node.js com Express para processar o PDF e realizar a validação dos CPFs.  
- **Banco de Dados:** Firebase Realtime Database para armazenar e recuperar os CPFs.  
- **Leitura de PDF:** [pdf-parse](https://www.npmjs.com/package/pdf-parse) para extrair o conteúdo textual dos arquivos PDF.  

---

##  Pré-requisitos
Antes de rodar a aplicação, certifique-se de que você tem o seguinte instalado:
- **Node.js** (versão 16 ou superior)
- Conta no [Firebase](https://firebase.google.com)
- Configuração do **Realtime Database** no Firebase  

---

##  Configuração do Firebase  
Siga os passos abaixo para configurar o Firebase em seu projeto:

1. Crie um novo projeto no [Firebase Console](https://console.firebase.google.com/).  
2. Ative o **Realtime Database** no Firebase. No início, você pode deixar as regras de segurança no modo de teste ou configurá-las conforme necessário.
3. Copie as credenciais do Firebase e cole no arquivo `firebaseConfig.js`:
  
```js
const firebaseConfig = {
    apiKey: "AIzaSyBy1Y_c77SOfQafFyLV84qWcAUWnAS5E0k",
    authDomain: "teste-683a1.firebaseapp.com",
    projectId: "teste-683a1",
    storageBucket: "teste-683a1.firebasestorage.app",
    messagingSenderId: "289942572221",
    appId: "1:289942572221:web:03f69d06ca604491d17bd4",
    measurementId: "G-YH4N7XHWL4"}

#  teste

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```--------------------------------------------

### Bibliotecas

https://www.npmjs.co- Biblioteca
https://www.npmjs.com/package/fire- Integração com o Firebase
Express - Framework para criação do
https://www.npmjs.com/packa- Permissão para requisições entre o frontend e backend

contato:
Email: guilherme.toribio02@gmail.com
