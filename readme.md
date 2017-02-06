# Project Manager

Foi desenvolvido uma aplicação com o objetivo de gerenciar projetos.

O usuário pode:

 - adicionar, alterar e excluir projetos, anotações, clientes e usuários.

 - O usuario podera alaterar o status do projeto para Em andamento, concluído.

 - Na tela principal sera mostratdo todos os projetos e o progresso de cada um.

# Passo a Passo

- Clone este repositório para a pasta do seu servidor web :
    - Exemplo: git clone https://github.com/lisianemorais/projectmanage.git /var/www/ProjectManager
- No terminal, acesse o diretório recém criado e execute o comando "composer install" para que o composer possa baixar e instalar todas as dependências do projeto.

    Exemplo: cd /var/www/html/ProjectManager sudo composer install

-   Após a instalação das dependências, crie o arquivo .env na raiz do projeto e o configure com os dados do ambiente de produção ( Banco de dados e etc... ).
-   Agora temos que migrar as tabelas do banco de dados. No terminal, acesse o diretório da aplicação e rode o comando: php artisan migrate .

-   Para acessar o sistema é necessário usuario e password
    - user: user@projectmanager.com
    - password: 123456
# Vagrant-Setup

No diretorio vagrant estão os arquivos para confirgurar o Vagrant

Servidor LAMP (Linux, Apache, MySQL, PHP)

Configuração do Vagrant (com provisionamento em Shell Script) para criar uma máquina virtual (Ubuntu Server 14.04 64 Bits) de desenvolvimento em PHP.

# Pacotes Inclusos:

-   PHP 5.6
-   MySQL 5.5
-   Git
-   PhpMyAdmin
-   Composer
-   cURL
-   Vim
-   Redis (Para mais detalhes consulte arquivo setup.sh)

# Você vai precisar:

 -  Virtualbox - https://www.virtualbox.org/
 -  Vagrant - http://www.vagrantup.com/
 
# Modo de Uso

- Salve os arquivos em um diretório
- Abra o Terminal, Entre no diretório vagrant ( Ou o que você definir na hora de salvar )
- Inicie a máquina virtual com o comando:
    - vagrant up

Após este comando 'vagrant up', o Vagrant ficará responsavel por baixar o sistema operacional ( neste caso Ubuntu Server 64 ), configurar a máquina virtual no VirtualBox e posteriormente baixar, instalar e configurar todos os pacotes do script 'setup.sh' (A primeira vez realmente é um pouco mais demorado).

Quando tudo estiver pronto, um servidor web estará disponível no endereço http://localhost:8080, e a instalação do PHPMyAdmin está em http://localhost:8080/phpmyadmin, para acessar utilize:

    Login: root
    Senha: vagrant

obs:(A senha padrão para todos os serviços é vagrant).

Coloque seu código no diretório "www". Todo o conteúdo dele estará disponível via http://localhost:8080. 

