Este teste foi feito utilizando o Kali-Linux em WSL2 (Windows Subsystem Linux 2).

Se deseja rodar/instalar Linux em seu ambiente Windows sem ferramentas de virtualização, como Virtualbox, é só seguir o link:
https://www.kali.org/docs/wsl/wsl-preparations/

Abaixo seguem os testes realizados em minha máquina. ->

# Phishing para captura de senhas do Facebook

### Ferramentas

- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux

- Acesso root: ``` sudo su ```
- Iniciando o setoolkit: ``` setoolkit ```
- Tipo de ataque: ``` Social-Engineering Attacks ```
- Vetor de ataque: ``` Web Site Attack Vectors ```
- Método de ataque: ```Credential Harvester Attack Method ```
- Método de ataque: ``` Site Cloner ```
- Obtendo o endereço da máquina: ``` ifconfig ```
- URL para clone: http://www.facebook.com

### Resutados

![Alt text](./passwd.png "Optional title")
