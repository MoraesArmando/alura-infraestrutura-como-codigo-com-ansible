# alura-infraestrutura-como-codigo-com-ansible


## DevOps 
O DevOps busca maneiras de **encurtar o seu ciclo de feedbacks** entre os times de desenvolvimento e estrutura, tornar o processo com repetições tanto do lado no lado da infraestrutura - como já é feito no lado do desenvolvimento. 
>Se pensarmos em uma forma simples de definir DevOps, trata-se de levarmos a **cultura ágil para a cultura de infraestrutura** e integrá-las.

Ao falarmos de DevOps, conseguiremos **automatizar** tudo aquilo que é feito na infraestrutura e garantir o **estado dos servidores**.

## Ansible
O Ansible é uma ferramenta para garantirmos esse estado. Ansible usa os scripts - neste caso, falamos de três modelos de script:

- Arquivo de inventário: que irá levantar as máquinas que serão configuradas;
- Playbook: "receita" que nos diz o que devemos fazer;
- Roles: permite modularizar o código.

## Comandos

$ ansible wordpress -i ./hosts -a "echo Hello, World!!!" -m shell

$ ansible wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'

**erro UNREACHABLE:***
$ ssh-keygen -t rsa
$ ssh-copy-id -i vagrant_id_rsa.pub vagrant@172.17.177.40
Obs: Talvez esteja necessário remover o arquivo ~/.ssh/known_hosts.


ansible-playbook -i ./hosts ./playbook.yml 
