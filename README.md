// docker-php-develop-ambient

# ambiente-apache2-php7.2-mysql-postgres-redis



**Pré-requisitos:** Docker e docker-compose instalados.

**procedimentos:**

1. Clonar o repositório no local desejado;

   ```
   git clone https://github.com/sandersonferraz/ambiente-apache2-php7.2-mysql-postgres-redis.git
   ```

   

2. Renomear para docker;

   ```
   /ambiente-apache2-php7.2-mysql-postgres-redis > /docker
   ```

   

3. Criar uma pasta para os projetos fora da pasta docker;

   ```
   /docker
   /projetos
   ```

   

4. Entrar  dentro da pasta docker;

5. Abrir o arquivo docker-compose.yml com um editor de texto;

6. Na linha 13 do arquivo citado a cima, definir o caminho do projeto a qual estará trabalhando;

   ```
   - ../projetos:/var/www/html -> Estado atual.
   Para
   - ../projetos/laravel:/var/www/html -> Exemplo de um projeto Laravel dentro da pasta projetos. Que será indexidado para dentro da pasta /var/www/hrml do container com o apache2 e php.
   ```

   

7. Alterar as senhas **secret** nas linhas 34, 47 e 57 se desejar;

8. Salvar o arquivo  docker-compose.yml;

9. Executar o comando a baixo:

   ```
   docker-compose up -d
   ```





## HAVE A GOOD TIME!!!
