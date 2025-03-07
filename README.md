# Aprendendo sobre o Docker

**Docker** é uma plataforma de contêinerização que permite empacotar, distribuir e executar aplicações de maneira isolada e portátil. Ele facilita a criação de ambientes leves e consistentes para o desenvolvimento e a execução de software.

## Comandos Básicos do Docker

### 1. `docker images`
- **Descrição**: Mostra as imagens Docker instaladas no seu sistema.

### 2. `docker pull <nome_da_imagem>`
- **Descrição**: Baixa uma imagem para o seu sistema. Exemplo: `docker pull ubuntu`.  
  Também pode incluir versões, como: `docker pull node:14.21.1-alpine`.

### 3. `docker rm <nome_da_imagem>`
- **Descrição**: Remove uma imagem do Docker.

### 4. `docker run -it <nome_da_imagem>`
- **Descrição**: Executa uma imagem de forma interativa, permitindo que você interaja com ela no terminal.

### 5. `docker stop <nome_do_conteiner>`
- **Descrição**: Para um contêiner em execução.

### 6. `docker ps`
- **Descrição**: Exibe os contêineres em execução, mostrando seu ID, nome e tempo de criação.

### 7. `docker ps -a`
- **Descrição**: Exibe todos os contêineres (em execução e parados), com informações adicionais sobre seu status.

### 8. `docker rm $(docker ps -f status=exited -q)`
- **Descrição**: Remove todos os contêineres que foram parados com `exit`.

### 9. `docker ps -f status=exited -q`
- **Descrição**: Lista todos os contêineres que saíram (status "exited"), para que você possa reusá-los ou removê-los.

### 10. `docker rm <nome_do_conteiner>`
- **Descrição**: Remove um contêiner específico usando seu nome.

### 11. `docker run -d --name <nome_do_conteiner> <imagem>`
- **Descrição**: Cria e executa um contêiner em segundo plano com o nome especificado. Exemplo: `docker run -d --name meu_container ubuntu`.

docker run --rm -it -w "/usr/src/app" -v "${PWD}:/usr/src/app" node bash

### 12. `docker run --rm -it -w "/usr/src/app" -v "${PWD}:/usr/src/app" node bash`
**Explicação dos parâmetros:**

`--rm → Remove o container ao sair (opcional).`<br>
`-it → Modo interativo (para abrir um terminal dentro do container).`<br>
`-w "/usr/src/app" → Define o diretório de trabalho dentro do container.`<br>
`-v "${PWD}:/usr/src/app" → Monta a pasta atual (${PWD}) dentro do container no caminho /usr/src/app.`<br>

---

Esses comandos básicos são essenciais para quem está começando a aprender Docker. Eles permitem que você manipule imagens e contêineres de forma eficiente!

---

**Dicas:**  
- Lembre-se de que sempre que você cria ou remove imagens/contêineres, eles podem ocupar ou liberar bastante espaço no seu sistema, então sempre verifique o que está em execução ou armazenado.
