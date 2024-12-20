# GRANDE NOTA:

### Apesar de gerar o IP e acessar a página fake, não pude obter os mesmos resultados dos teste, pois o WSL tem rede diferente da internet.

### Decidi por não encontrar forma de fazer o WSL usar a mesma rede doméstica da Internet

### EDIT: talvez o erro sej por outro motivo, pois os links 'criar conta' e 'esqueci senha' funcionam, ou seja, levam à página oficial. Talvez o problema seja no botão 'login' da página fake.

Este teste foi feito utilizando o Kali-Linux em WSL2 (Windows Subsystem Linux 2).

Se deseja rodar/instalar Linux em seu ambiente Windows sem ferramentas de virtualização, como Virtualbox, é só seguir o link:
https://www.kali.org/docs/wsl/wsl-preparations/

Abaixo seguem os testes realizados em minha máquina. ->

O WSL instala a versão 'mínima' do Kali, então é necessário instalar a ferramente ```setoolkit```manualmente. Faça como aseguir:

Abra um terminal e execute os seguintes comandos: ```sudo apt update``` e ```sudo apt full-upgrade -y```

O comando apt update atualiza a lista de pacotes disponíveis. O comando apt full-upgrade atualiza os pacotes instalados para suas versões mais recentes, incluindo a remoção de pacotes obsoletos. O -y confirma automaticamente as ações, economizando tempo.

Instalar as dependências:

O Setoolkit depende de várias outras ferramentas e bibliotecas para funcionar corretamente. Instale as dependências usando o seguinte comando: ```sudo apt install git python3 python3-pip python3-requests libapache2-mod-php -y```

Utilize: ```git clone https://github.com/trustedsec/social-engineer-toolkit.git``` dentro do terminal do Kali.

Este comando criará um diretório chamado social-engineer-toolkit no seu diretório atual.

Entre no diretório que acabou de ser criado: ```cd social-engineer-toolkit```

Execute o script de instalação: ```sudo python3 setup.py install```

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
