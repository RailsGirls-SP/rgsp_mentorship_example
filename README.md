# Rails Girls SP - Festa da Instalação

Bem-vindas! 
Esse guia tem como objetivo auxiliá-las na preparação do ambiente de desenvolvimento. Abaixo, você encontrará as instruções para instalar as ferramentas necessárias e criar um projeto Rails usando DevContainers.

---

## Pré-requisitos

Para este projeto, será necessário instalar:
- Docker
- VSCode com a extensão DevContainers
- rails-new

---

### 1. Instalar o Docker

Siga a documentação oficial para instalar o Docker em seu sistema operacional:
- [Docker - Documentação Oficial](https://docs.docker.com/desktop/)
- [Linux](https://docs.docker.com/desktop/install/linux/)
- [Mac](https://docs.docker.com/desktop/install/mac-install/)
- [Windows](https://docs.docker.com/desktop/install/windows-install/)

### 2. Instalar o VSCode e DevContainers

Baixe o [VSCode](https://code.visualstudio.com/Download) e instale a extensão DevContainers:
- [DevContainers para VSCode](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

### 3. Instalar o app Rails-new

Siga as instruções do [Rails-new](https://github.com/rails/rails-new?tab=readme-ov-file#installation) para fazer o download do executável:
1. Acesse a página de *releases* e baixe o release mais recente.
2. Descompacte o arquivo e mova o executável `rails-new` para um diretório de sua preferência.

> **Recomendação**: Crie uma pasta de projeto ou workspace para manter o ambiente organizado.

#### **Troubleshooting (MacOS)**
Caso o `rails-new` não abra, siga os passos abaixo:
1. Acesse **Privacidade e Segurança** em seu sistema.
2. Role até Segurança e autorize o aplicativo `rails-new`.
   - [Instruções para permitir apps de desenvolvedores desconhecidos](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unknown-developer-mh40616/mac)

---

## Criando o Projeto

Para iniciar um novo projeto Rails dentro do Docker usando DevContainer, siga os passos abaixo:

1. Crie o projeto com o comando:
   ```bash
   ./rails-new rgsp_mentorship_example --main --database=postgresql --devcontainer


2. Abra o projeto com o DevContainer no VSCode:
 - Pressione CMD/CTRL + SHIFT + P e selecione DevContainers: Open Folder in Container.
 > Isso iniciará o container Docker e abrirá os arquivos no VSCode.

3. Para iniciar o servidor Rails:
```bash
bin/rails s
```
> Nota: Como estamos utilizando o Rails no Docker e não como uma gem, todos os comandos Rails devem ser precedidos de bin/rails.

### Recursos Adicionais
Para mais informações sobre o framework Rails:

 - [Rails Guides - Get Started](https://guides.rubyonrails.org/getting_started.html)
 - [MVC e Você](https://guides.rubyonrails.org/getting_started.html#mvc-and-you)
 - [CRUD](https://guides.rubyonrails.org/getting_started.html#crudit-where-crudit-is-due)
