# Executar o Projeto (Windows - Git Bash)

Este guia explica como executar o frontend Vue 3, o backend NestJS e o MongoDB no Windows, usando o Git Bash.

## Pré-requisitos

* Node.js e npm (ou Yarn) instalados
* MongoDB instalado e configurado
* Git Bash instalado

## Passos

1.  **Iniciar o MongoDB:**

    * Se o MongoDB estiver instalado como um serviço do Windows:
        ```bash
        net start MongoDB
        ```
    * Se o MongoDB estiver a correr como um processo:
        ```bash
        mongod
        ```

2.  **Iniciar o Backend (NestJS):**

    ```bash
    cd backend
    npm install
    npm run start:dev
    ```

3.  **Iniciar o Frontend (Vue 3):**

    ```bash
    cd frontend
    npm install
    npm run serve
    ```

## Notas

* Certifica-te de que o MongoDB está a correr e que a tua aplicação NestJS está configurada para se ligar ao MongoDB correto.
* Configura as variáveis de ambiente necessárias.
* Ajusta as portas se necessário.
* Configura o proxy reverso no `vue.config.js` do frontend para que as chamadas à API sejam encaminhadas para o backend.
