Este teste foi feito utilizando o Kali-Linux em WSL2 (Windows Subsystem Linux 2).

Se deseja rodar/instalar Linux em seu ambiente Windows sem ferramentas de virtualização, como Virtualbox, é só seguir o link:
https://www.kali.org/docs/wsl/wsl-preparations/

Abaixo seguem os testes realizados em minha máquina. ->

O WSL instala a versão 'mínima' do Kali, então é necessário instalar a ferramente ```setoolkit```manualmente.

Utilize: git clone https://github.com/trustedsec/social-engineer-toolkit.git dentro do terminal do Kali.

Este comando criará um diretório chamado social-engineer-toolkit no seu diretório atual.

Entre no diretório que acabou de ser criado: cd social-engineer-toolkit

Execute o script de instalação: sudo python3 setup.py install

Este comando instalará o Setoolkit no seu sistema.

Em seguida, utilize ```sudo setoolkit```para iniciar o programa ou siga o processo abaixo:

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
