
## Atividade Assíncrona - Semana 2 (23/09/2020 a 29/09/2020)

**Autor: Marcos Wesley Soares Alves**

**Matricula: 20181070130258**

## Instalação do SSH

  - Primeiramente vamos atualizar o repositório debian onde está localizados os pacotes. Após acessar o servidor a partir do virtual box, digite o comando abaixo para fazer a atualização:
    
        apt-get update


- Com o repositório atualizado, agora vamos instalar o serviço **SSH** através do comando:

        apt-get install ssh


- **Acessando o servidor a partir do cliente**

    A partir do nosso ambiente de realização de atividades práticas onde temos dois computadores (cliente1 e cliente2). Vamos acessar a partir do cliente1 (sem interface gráfica) o servidor via SSH. 

    No debian o SSH cliente já está previamente carregado. Para verificar você pode digitar ssh na linha de comando. Se o serviço estiver disponível será apresentado algumas informações como na imagem abaixo:

    <div align='center'>
        <img src='img1.png'>
    </div>





    Para fazer um acesso remoto do cliente via ssh ao servidor, vamos digitar o seguinte comando:

            ssh root@192.168.0.254

    No primeiro acesso que eu fizer via ssh a qualquer máquina vai aparecer essa mensagem perguntando se eu quero me conectar e vai informar um fingerprint da chave de criptografia da máquina. Essa chave será gravada em um arquivo para futuramente se eu acessar uma outra máquina cujo ip for o mesmo, será verificado se essa chave é a mesma. Por questão de segurança sempre será informado caso ele encontre uma nova chave ou uma chave diferente pra um determinado ip. Sabendo disso podemos colocar sim e apertar a tecla enter.

    <div align='center'>
        <img src='img2.png'>
    </div>

    Será solicitado a senha do usuário que você está tentando acessar, no nosso caso o usuário é root.

    <div align='center'>
        <img src='img3.png'>
    </div>

    Após informar a senha você vai estar conectado ao servidor.

     <div align='center'>
        <img src='img4.png'>
    </div>

    Para verificar as máquinas que estão conectadas ao servidor, você pode usar o comando *who* ou apenas *w*.

     <div align='center'>
        <img src='img5.png'>
    </div>

    Através dos comandos é possível verificar que a máquina de ip 192.168.0.1 está conectado ao servidor.

    Vimos nessa seção como instalar e nos conectar a um servidor via ssh(Secure Shell). Porém devemos tomar cuidado com algumas configurações de acesso como por exemplo a porta e o usuário ao qual estamos nos conectando, pois isso pode causar diversos problemas de segurança. Esse será o assunto do próximo tópico.

   
## Alterando configurações no arquivo sshd_config

-


- Boas práticas de alteração no arquivo de configuração;




## Observações:
 - Mostrar na prática o uso do winscp e putty


## Cópia de um arquivo do servidor (considerar o cenário de simulação) usando uma aplicação gráfica

