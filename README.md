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