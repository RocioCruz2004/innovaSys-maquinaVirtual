# Proyecto InnovaSys - Ansible
Este repositorio contiene la automatizacion del servidor innovasys para la materia taller de sistemas operativos II.
el playbook se instala y configura de forma automatica:
- APACHE: pagina de bienvenida que se hizo
- SAMBA: recurso compartido para el grupo de desarrolladores

# Ejecucion del playbook
1. clonar este repositorio en el nodo de control (LinuxLite)
2. editar el archivo "inventory" y asegurarse de que la IP y el usuario del servidor Ubuntu operador sean correctos (102.168.10.100)
3. Ejecutar el playbook con: ansible-playbook -K site.yml

#como verificarlo
- Para apache se abre el navegador como http://192.168.10.100
- Para samba desde el gestor de archivos poner smb://192.168.10.100/Proyectos y entrar como usuario devuser1 con la contra definida en group_vars/all.yml
