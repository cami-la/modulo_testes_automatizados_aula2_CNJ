<h2>🐧 LINUX - Ubuntu</h2>

<h3>Instalação OpenJDK</h3>
<ol>
	<li>Abra o terminal e verifique o Java está instalado:</li>
    <code>java --version</code>
    <li>Para instalar o <em>openJDK-11</em>, digite no terminal:</li>
    <code>sudo apt-get install openjdk-11-jdk</code>
    <li>Verifique se foi instalado com sucesso:</li>
    <code>java --version</code>
    <li>Configure o ambiente <code>JAVA_HOME</code>:</li>
    <ul>
        <li>Verifique o caminho da instalação do Java:</li>
        <code>sudo update-alternatives --config java</code>
        <li>Copie o caminho que aparecerá no terminal. No meu caso:</li>
        <code>/usr/lib/jvm/java-11-openjdk-amd64/bin/java</code>
        <li>Edite o arquivo .bashrc</li>
        <code>sudo gedit ~/.bashrc</code>
        <li>Copie o código abaixo e cole no final do arquivo .bashrc</li>
        <code>JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64<br>
			export JAVA_HOME<br>
            export PATH=$PATH:$JAVA_HOME
        </code>
		<li>Salve o arquivo</li>
        <li>Verifique a alteração do documento:</li>
		<code>cat ~/.bashrc</code>
    </ul>
    <li>Feche o terminal e abra novamente</li>
    <li>Verifique se o Java está instalado</li>
    <code>java --version</code>
    <li>Instalação concluída!</li>
</ol>
<p align="right"><em>Créditos: <a href="https://www.youtube.com/watch?v=jARiy3DZdwg">DevSuperior</a></em></p>

<h3>Instalação Eclipse</h3>
<ol>
    <li>Entre no site oficial do Eclipse Foundation e faça o <strong><a href="https://www.eclipse.org/downloads/download.php?file=/oomph/epp/2021-06/R/eclipse-inst-jre-linux64.tar.gz">DOWNLOAD</a></strong></li>
    <li>Descompacte a pasta</li>
    <li>Procure o arquivo "eclipse-inst" e execute</li>
    <li>Escolha segunda a opção: Eclipse IDE for Enterprise Java and Web Developers</li>
    <li>Clique no folder da primeira opção e selecione o JDK que instalamos na nossa máquina</li>
    <li>Mantenha as opções "create start menu entry" e "create desktop shortcut"</li>
    <li>Install</li>
    <li>Accept now</li>
    <li>Launch</li>
    <li>Pesquise o Eclipse IDE nas suas aplicações</li>
    <li>Intalação concluída!</li>
</ol>

<h3>Instalação Visual Studio Code</h3>
<ol>
    <li>Entre no site oficial do Visual Studio Code</li>
    <li>Faça o <strong><a href="https://code.visualstudio.com/">DOWNLOAD</a></strong> do arquivo com a extensão .deb</li>
    <li>Escolha a opção Open With: Software install (default)</li>
    <li>Pesquise o VS code nas suas aplicações</li>
    <li>Intalação concluída!</li>
    <li>Configuração para desenvolvimento Java:</li>
    <ul>
        <li>Abrir o Vs code</li>
        <li>Abrir o menu de extensões: (Ctrl + Shift + X)</li>
        <li>Colar os comandos abaixo e fazer as instalações:</li>
        <code>vscode:extension/vscjava.vscode-java-pack</code><br>
        <code>vscode:extension/pivotal.vscode-boot-dev-pack</code>
        <li>Configuração concluída!</li>
    </ul>
</ol>

<h3>Instalação GIT</h3>
<ol>
	<li>Abra o terminal verifique se o GIT está instalado</li>
    <code>git --version</code>
    <li>Para instalar o GIT, execute o comando:</li>
    <code>sudo apt-get install git-all</code>
    <li>Verifique se o GIT realmente está instalado:</li>
    <code>git --version</code>
    <li>Configurações iniciais:</li>
    <ul>
    	<li>Configurar o nome de usuário:</li>
        <code>git config --global user.name "Seu nome"</code>
        <li>Configurar o endereço de e-mail: <em>(Mesmo do GitHub)</em></li>
        <code>git config --global user.email seuemail@email.br</code>
        <li>Verifique as configurações:</li>
		<code>git config --list</code>
    </ul>
    <li>Instalação concluída!</li>
</ol>

<h3>Instalação Apache Maven</h3>
<p>Pensando em facilitar a instalação, iremos utilizar uma ferramenta de gerenciamento de versões chamada <a href="https://sdkman.io/">SDKMAN!</a>
</p>
<ol>
    <li>Para Instalar o SDMAN!, execute no terminal:</li>
    <code>curl -s "https://get.sdkman.io" | bash</code>
    <li>Em seguida:</li>
    <code>source "$HOME/.sdkman/bin/sdkman-init.sh"</code>
    <li>Verifique se o SDKMAN! foi instalado:</li>
    <code>sdk --version</code>
    <li>Para instalar o <a href="https://sdkman.io/sdks">Apache Maven</a>:</li>
    <code>sdk install maven</code>
    <li>Verifique se o Apache Maven está instalado</li>
    <code>mvn --version</code>
    <li>Instalação concluída!</li>
</ol>
<hr>

<h2>🪟 WINDOWS</h2>

<h4>Instalação OpenJDK Zulu</h4>
<ol>
    <li>Entre no <a href="https://www.azul.com/downloads/?package=jdk"><strong>SITE AZUL</strong></a></li>
    <li>Faça o download do arquivo .zip do JDK 11.0.11+9. No meu caso, o x86 64-bit</li>
    <li>Vá no drive -> C://Arquivo de Programas</li>
    <li>Caso não tenha um diretório com o nome Java, crie</li>
    <li>Entre neste diretório e descompacte o download do zip JDK Zulu 11.0.11+9 neste diretório</li>
    <li>Copie caminho do diretório que você descompactou o zip JDK Zulu 11.0.11+9</li>
    <li>Configuração de ambiente <code>JAVA_HOME</code>:</li>
    <ul>
        <li>Menu iniciar -> Editar as varáveis de ambiente do sistema</li>
        <li>Irá abrir a janela Propriedades do Sistema, escolha a aba Avançado, em seguida clique em variáveis de Ambiente</li>
        <li>Na janela Variáveis de Ambiente,  crie um novo Variáveis do sistema</li>
        <li>Abrirá uma jabela: Nova Variável de Sistema</li>
        <li>Nome da variável: <code>JAVA_HOME</code></li>
        <li>Valor da variável: Cole o caminho do diretório que você descompactou o zip JDK Zulu 11.0.11+9 no passo 5 -> ok</li>
        <li>Na mesma janela Variáveis do Sistema, localize a variável Path, selecione e clique a opção Editar...</li>
        <li>Clique na opção Novo e cole o mesmo caminho do passo 5 acrescentando <code>\bin</code></li>
        <li>Continue com o path selecionado e clique na opção Mover para Cima até chegar no topo</li>
        <li>Finalizada a configuração!</li>
    </ul>
    <li>Abra o Prompt de Comando: Menu iniciar -> cmd</li>
    <code>java --version</code>
    <li>Instalação concluída!</li>
</ol>
<p align="right"><em>Créditos: <a href="https://www.youtube.com/watch?v=laC0fiI-IOM">DevSuperior</a></em></p>

<h3>Instalação Eclipse</h3>
<ol>
    <li>Entre no site oficial do Eclipse Foundation e faça o <strong><a href="https://www.eclipse.org/downloads/download.php?file=/oomph/epp/2021-06/R/eclipse-inst-jre-linux64.tar.gz">DOWNLOAD</a></strong></li>
    <li>Execute o arquivo</li>
    <li>Escolha segunda a opção: Eclipse IDE for Enterprise Java and Web Developers</li>
    <li>Clique no folder da primeira opção (Java 11 + VM) e selecione o JDK instalado máquina</li>
    <li>Mantenha as opções "create start menu entry" e "create desktop shortcut"</li>
    <li>Install</li>
    <li>Accept now</li>
    <li>Launch</li>
    <li>Pesquise o <em>Eclipse IDE</em> nas suas aplicações</li>
    <li>Instalação concluída!</li>
</ol>

<h3>Instalação Visual Studio Code</h3>
<ol>
    <li>Entre no site oficial do Visual Studio Code e faça o <strong><a href="https://code.visualstudio.com/">DOWNLOAD</a></strong> "Download for windows"</li>
    <li>Espere o download concluir e execute o arquivo</li>
    <li>Install -> Next -> Next ... Finish</li>
    <li>Pesquise o <em>VS Code</em> nas suas aplicações</li>
    <li>Intalação concluída!</li>
	<li>Configuração para desenvolvimento Java:</li>
    <ul>
        <li>Abrir o Vs code</li>
        <li>Abrir o menu de extensões: (Ctrl + Shift + X)</li>
        <li>Colar os comandos abaixo e fazer as instalações:</li>
        <code>vscode:extension/vscjava.vscode-java-pack</code>
        <code>vscode:extension/pivotal.vscode-boot-dev-pack</code>
        <li>Configuração concluída!</li>
    </ul>
</ol>

<h3>Instalação Apache Maven</h3>
<ol>
    <li>Entre no site ofical da Apache Maven e faça o <strong><a href="https://maven.apache.org/download.cgi">DOWNLOAD</a></strong> "Binary zip archive"</li>
    <li>Vá no drive -> C://Arquivo de Programas</li>
    <li>Caso não tenha um diretório com o nome Maven, crie</li>
    <li>Entre neste diretório e descompacte o download do zip apache-maven-3.8.5-bin.zip neste diretório</li>
    <li>Copie caminho do diretório que você descompactou o zip apache-maven-3.8.5-bin.zip</li>
    <li>Configuração de ambiente <code>M2_HOME</code>:</li>
<ul>
    <li>Menu iniciar -> Editar as varáveis de ambiente do sistema</li>
    <li>Irá abrir a janela Propriedades do Sistema, escolha a aba Avançado, em seguida clique em variáveis de Ambiente</li>
    <li>Na janela Variáveis de Ambiente, crie um novo Variáveis do sistema</li>
    <li>Abrirá uma janela: Nova Variável de Sistema</li>
    <li>Nome da variável: <code>M2_HOME</code></li>
    <li>Valor da variável: Cole o caminho do diretório que você descompactou zip apache-maven-3.8.5-bin.zip no passo 5 -> ok</li>
    <li>Na mesma janela Variáveis do Sistema, localize a variável Path, selecione e clique a opção Editar...</li>
    <li>Clique na opção Novo e cole o mesmo caminho do passo 5 acrescentando <code>\bin</code></li>
    <li>Continue com o path selecionado e clique na opção Mover para Cima até chegar no topo</li>
    <li>Finalizada a configuração!</li>
    </ul>
    <li>Abra o Prompt de Comando: Menu iniciar -> cmd</li>
    <code>mvn --version</code>
    <li>Instalação concluída!</li>
</ol>
<p align="right"><em>Créditos: <a href="https://www.treinaweb.com.br/blog/introducao-ao-maven-aprenda-como-criar-e-gerenciar-projetos-java">TreinaWeb</a></em></p>

<h3>Instalação GIT</h3>
<ol>
    <li>Entre no site oficial do <a href ="https://git-scm.com/downloads"><strong>GIT</strong></a></li>
    <li>Escolha a opção Windows e o instalador será baixado automáticamente</li>
    <li>Mantenha as opções pré selecionadas</li>
    <li>Next</li>
    <li>Install</li>
    <li>Antes de finaizar a instalação, selecione a opção "Lauch Git Bash"</li>
    <li>Verifique se o Java está instalado:</li>
    <code>git --version</code>
    <li>Configurações iniciais:</li>
    <ul>
    	<li>Configurar o nome de usuário:</li>
        <code>git config --global user.name "Seu nome"</code>
        <li>Configurar o endereço de e-mail: <em>(Mesmo do GitHub)</em></li> 
        <code>git config --global user.email seuemail@email.br</code>
        <li>Verifique as configurações:</li>
		<code>git config --list</code>
    </ul>
    <li>Instalação concluída!</li>
</ol>
<hr>

<h4><strong>Atalhos mais utilizados - ECLIPSE IDE</strong></h4>
<table>
	<tr>
		<th>Atalho</th>
		<th>Descrição</th>
	<tr>
	<tr>
		<td>Ctrl + N</td>
		<td>Cria uma nova classe Java</td>
	</tr>
	<tr>
		<td>Ctrl + D</td>
		<td>Deleta linha ou bloco</td>
	</tr>
	<tr>
		<td>Ctrl + I</td>
		<td>Identa o código selecionado</td>
	<tr>
	<tr>
		<td>Ctrl + Backspace</td>
		<td>Verifica o nome de uma classe ou objeto</td>
	</tr>
	<tr>
		<td>Ctrl + 1</td>
		<td>Quick Fix, (Rename, Extract, Convert, try-catch...)</td>
	</tr>
	<tr>
		<td>Ctrl + Shift + F</td>
		<td>Identa todo o código</td>
	</tr>
	<tr>
		<td>Ctrl + Shift + S</td>
		<td>Salvamento</td>
	</tr>
	<tr>
		<td>Ctrl + 3</td>
		<td>Quick Search (Abre um menu de ações)</td>
	</tr>
	<tr>
		<td>Shift + Alt + S</td>
		<td>Source (Gera com template: Getter and Setter, toString(), Constructor...)</td>
	</tr>
	<tr>
		<td>Shift + Alt + R</td>
		<td>Refatora a variável em todos os lugares</td>
	</tr>
	<tr>
		<td>main</td>
		<td>Cria o método main</td>
	</tr>
	<tr>
		<td>sysout</td>
		<td>Cria o output no console</td>
	</tr>
		<tr>
		<td>switch</td>
		<td>Cria um switch/case automaticamente</td>
	</tr>
</table>
<h4><strong>Atalhos mais utilizados - GIT</strong></h4>
<table>
	<tr>
		<th>Atalho</th>
		<th>Descrição</th>
	<tr>
	<tr>
		<td>git init</td>
		<td>Cria uma nova classe Java</td>
	</tr>
	<tr>
		<td>git status</td>
		<td>Deleta linha ou bloco</td>
	</tr>
	<tr>
		<td>git add</td>
		<td>Identa o código selecionado</td>
	<tr>
	<tr>
		<td>git branch</td>
		<td>Verifica o nome de uma classe ou objeto</td>
	</tr>
	<tr>
		<td>git checkout -b</td>
		<td>Quick Fix, (Rename, Extract, Convert, try-catch...)</td>
	</tr>
	<tr>
		<td>git commit -m</td>
		<td>Identa todo o código</td>
	</tr>
	<tr>
		<td>git pull</td>
		<td>Salvamento</td>
	</tr>
	<tr>
		<td>git push</td>
		<td>Quick Search (Abre um menu de ações)</td>
	</tr>
	<tr>
		<td>git fecth</td>
		<td>Source (Gera com template: Getter and Setter, toString(), Constructor...)</td>
	</tr>
	<tr>
		<td>git clone</td>
		<td>Refatora a variável em todos os lugares</td>
	</tr>
</table>

<h3>Fontes:</h3>
<ul>
	<li>https://pt.wikipedia.org/wiki/Editor_de_texto</li>
	<li>https://code.visualstudio.com/docs/languages/java</li>
	<li>https://www.devmedia.com.br/principais-atalhos-do-eclipse/25614</li>
  <li>https://www.dio.me/articles/tutorial-completo-do-maven-para-iniciantes</li>
  <li>https://comandosgit.github.io/</li>
<ul>
