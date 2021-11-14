## wordpress-docker

## Projeto de Bloco

Este trabalho foi desenvolvido para obter conhecimento da ferramenta GITHUB referente a instalação do Wordpress com Containers Docker.

## Docker e Contaneirs

Docker se resume em uma tecnologia semelhante a uma virtualização tradicional, que possibilita o empacotamento de uma aplicação ou ambiente inteiro dentro de um contêiner, daí temos a facilidade de portabilidade para qualquer outro ambiente com Docker instalado.

![image](https://user-images.githubusercontent.com/90536330/141665815-d9579080-b469-41c6-9fdd-f94e74f8d2f5.png)

Containers é a segregação dos processos no mesmo kernel, além de conter toda a aplicação instalada, também contém tudo o que você precisa para que seu sistema funcione (SO, bibliotecas, softwares, arquivos, etc).

![image](https://user-images.githubusercontent.com/90536330/141666436-2b73db67-c23a-4d7d-a4d0-7eec7fda524a.png)

Diferente das máquinas virtuais, o Docker dispensa uma camada com um hypervisor. Em vez disso, os containers funcionam como processos isolados, compartilhando diretamente o mesmo kernel da máquina hospedeira junto com outros containers e quaisquer outros serviços na mesma.

![image](https://user-images.githubusercontent.com/90536330/141666704-40fc3a99-9c19-4f00-ad7f-4bd19f1897ce.png)

Próximos passos será instalar o Docker, cada contêiner é uma aplicação isolada independentemente, vamos criar um contêiner para o Worpress e outro para o MySQL.

O Wordpress é um aplicativo para um sistema de gerenciamento de conteúdo voltado para a web, sua descrição é toda em PHP e os bancos de dados (para armazenamento dos conteúdos) é o MySQL.

## Instalação do Docker

Pré-requisito: aplicar o comando abaixo na pasta /etc/sudoers para aplicar permissões ao usuário.

```
ansible ALL=(ALL:ALL) NOPASSWD:ALL
```

Criar pasta com o comando mkdir.

```
mkdir wordpress-docker
```

Os comandos abaixo instalam vários pacotes de suporte, que serão necessários para as funções de funcionamento dos pacotes do Docker.

```
sudo apt-get install \
  apt-transport-https \
  ca-certificates \
  curl \
  software-properties-common
```




