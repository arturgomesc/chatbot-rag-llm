# Executando a Aplicação Backend do Chat
Este backend utiliza o framework **Quart** para disponibilizar endpoints que extraem dados de repositórios e realizam interações de chat com essas informações.

## Pré-requisitos
- Verifique se você possui **Python 3.6** ou superior instalado. Para confirmar a versão instalada, utilize:

    ```bash
    python --version
    ```

- Também é preciso instalar as bibliotecas Python necessárias. Para isso, execute:

    ```bash
    pip install -r requirements.txt
    ```

## Iniciando o Servidor
Para executar o servidor, acesse o diretório onde está localizado o arquivo `main.py` e rode:

```bash
python main.py
```

O servidor será iniciado e ficará aguardando conexões (por padrão, na porta 5000).

## Observação
Antes de iniciar o servidor, abra o arquivo repo.py e substitua o token do GitHub na função form_metadata pelo seu token pessoal.

# Executando a Interface do Usuário do Chatbot

Este guia descreve como executar e interagir com o chatbot por meio de sua interface de usuário.

## Pré-requisitos

- Node.js e npm (Node Package Manager) instalados na sua máquina. Você pode obtê-los no site oficial: https://nodejs.org/

## Passos Para Executar o Chatbot

1. **Acesse o diretório do projeto**. Abra seu terminal e navegue até o diretório do projeto:

    ```bash
    cd path/to/local_directory/chatbot_v2.0
    ```

2. **Instale as dependências do projeto**. No diretório do projeto, rode o seguinte comando para instalar os pacotes necessários:

    ```bash
    npm install
    ```

3. **Inicialize o projeto**. Após instalar as dependências, execute:

    ```bash
    npm start
    ```

    Isso iniciará o servidor de desenvolvimento e o chatbot poderá ser acessado em http://localhost:3000 no seu navegador.

## Parando o Chatbot

caso queira parar de rodar o chatbot, pressione `Ctrl + C` no terminal onde o projeto está rodando.

## Observação

O Chatbot faz uma requisição POST para o backend por meio das rotas em http://127.0.0.1:5000/extract (para extrair informações do repositório) e em http://127.0.0.1:5000/lang-chat-sources (para conversar, utilizando seu token da OPENAI para autorização). Verifique se a API está em execução e se o token da OPENAI é válido.

# Automatizando o Processo de Obtenção das Respostas e Documentos das Perguntas
## Pré-requisitos
- Verifique se você possui Python 3.6 ou superior instalado. Para confirmar a versão, utilize:

    ```bash
        python --version
    ```

- Você também deve utilizar o seguinte código para instalar os pacotes necessários:

    ```bash
        pip install -r requirements.txt
    ```
## Executando o Script
Para executar o script que automatiza o processo para todas as 150 perguntas, navegue até o diretório dos scripts e execute:

```bash
    python script/automating_script.py
```

## Observação
Antes de rodar o script, abra o arquivo repo.py e substitua o token do GitHub na função form_metadata pelo seu token pessoal.
