# Laboratorio de Ansible con Docker

## Objetivo
Automatizar la configuracion de dos servidores Ubuntu utilizando Ansible y Docker.

## Tecnologias utilizadas
- Ubuntu 24.04
- Docker y Docker Compose
- Ansible
- Python 3

## Archivos del proyecto
- docker-compose.yml: configura los contenedores.
- inventory.ini: define los servidores.
- playbook.yml: contiene las tareas de automatizacion.
- README.md: documentacion del proyecto.

## Iniciar los servidores
docker compose up -d

## Verificar la conexion
ansible docker -i inventory.ini -m ping

## Ejecutar el playbook
ansible-playbook -i inventory.ini playbook.yml

## Tareas realizadas
1. Identificar el nombre de cada servidor.
2. Mostrar el sistema operativo.
3. Crear el directorio /tmp/ansible-demo.
4. Crear el archivo info.txt.
5. Crear los directorios logs, backup y config.
6. Mostrar un mensaje si el sistema operativo es Ubuntu.

## Resultado
El playbook se ejecuto correctamente en server1 y server2.
Ambos servidores finalizaron con failed=0.
