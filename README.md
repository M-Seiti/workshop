Guia de Preparação para o Workshop de SonarQube

Para participar da atividade prática do workshop, recomendamos realizar previamente a instalação das ferramentas abaixo.

--------------------------------------------------
1. Instalar o Python
--------------------------------------------------

Download:
https://www.python.org/downloads/

Durante a instalação, marque a opção:

"Add Python to PATH"

e clique em "Install Now".

Após a instalação, abra o Prompt de Comando (CMD) e execute:

python --version

A saída deve ser semelhante a:

Python 3.x.x

Caso o comando não funcione, reinicie o computador e tente novamente.

--------------------------------------------------
2. Instalar o Visual Studio Code
--------------------------------------------------

Download:
https://code.visualstudio.com/download

Após a instalação, abra o VS Code normalmente para verificar se a instalação foi concluída com sucesso.

--------------------------------------------------
3. Instalar o Java (JDK 17 ou superior)
--------------------------------------------------

O SonarQube necessita do Java para funcionar.

Download:
https://adoptium.net/temurin/releases/?version=17

Baixe a versão mais recente do JDK 17 para Windows e siga a instalação padrão.

Após a instalação, abra o Prompt de Comando (CMD) e execute:

java -version

A saída deve ser semelhante a:

openjdk version "17.x.x"

Se o comando não for reconhecido, reinicie o computador e tente novamente.

--------------------------------------------------
4. Instalar o SonarQube Community Build
--------------------------------------------------

Download:
https://www.sonarsource.com/products/sonarqube/downloads/

Após baixar:

1. Extraia o arquivo ZIP.
2. Abra a pasta extraída do SonarQube.
3. Entre na pasta: sonarqube
4. Depois entre na pasta: bin
5. Depois entre na pasta: windows-x86-64

O caminho completo ficará semelhante a:

sonarqube\bin\windows-x86-64

6. Dentro dessa pasta, localize e execute o arquivo:
StartSonar.bat

Uma janela do terminal será aberta.

7. Aguarde alguns instantes enquanto o SonarQube é iniciado.

8. Quando a inicialização terminar, abra o navegador e acesse:

http://localhost:9000

Login inicial:

Usuário: admin
Senha: admin

No primeiro acesso, o sistema poderá solicitar a troca da senha padrão.

--------------------------------------------------
5. Instalar o SonarScanner CLI
--------------------------------------------------

Download:
https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-6.2.1.4610-windows-x64.zip

Após baixar:

1. Extraia o arquivo ZIP.
2. Renomeie a pasta para algo simples, como: sonar-scanner
3. Mova essa pasta para o disco C:

Exemplo:

C:\sonar-scanner

4. Abra o menu Iniciar do Windows.
5. Pesquise por: Variáveis de Ambiente
6. Clique em: Editar as variáveis de ambiente do sistema
7. Clique em: Variáveis de Ambiente
8. Na seção "Variáveis do Sistema", selecione: Path
9. Clique em: Editar
10. Clique em: Novo
11. Adicione o caminho:

C:\sonar-scanner\bin

12. Clique em OK até fechar todas as janelas.
13. Feche qualquer terminal que esteja aberto.
14. Abra um novo Prompt de Comando (CMD) e execute:

sonar-scanner --version

A saída deve ser semelhante a:

INFO: SonarScanner x.x.x

--------------------------------------------------
Verificação Final
--------------------------------------------------

Abra um novo Prompt de Comando (CMD) e execute:

python --version
java --version
sonar-scanner --version

Em seguida, confirme que o SonarQube abre normalmente no navegador:

http://localhost:9000

Se todos os passos estiverem funcionando, seu ambiente estará pronto para a atividade prática do workshop.
