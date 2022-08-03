# GIT

| Comando                                       					| Descrição                                							|
| :-------------------                            					| :-------------------                  							|
|git init 															|(inicializa o controle do git no local requisitado)				|
|git stash  															|salva os arquivos não commitados em uma lista na memória 				|
|git stash save "Message"  															|salva os arquivos não commitados em uma lista na memória com mensagem 				|
|git stash save --keep-index  															|salva os arquivos fora da stage area em uma lista                        |
|git stash -u   															|salva os arquivos não rastreados em uma lista na memória 				|
|git stash list 															|exibe as listas de arquivos salvos em memória 				|
|git stash apply 															|aplica a lista de arquivo que está no top				|
|git stash apply stash@{2} 															|aplica uma lista de arquivo específica				|
|git stash drop 															|remove a lista de arquivo que está no top				|
|git stash drop stash@{2} 															|remove uma lista de arquivo específica				|
|git stash pop  															|aplica a lista de arquivo que está no top e depois a remove				|
|git stash pop stash@{2} 															|aplica uma lista de arquivo específica e depois a remove				|
|git ls-files 														|(lista os arquivos controlados pelo git)							|
|git status 														|	(exibe o estado de todos os arquivos controlados ou não)		|	
|git add <<nome do arquivo 1> <nome do arquivo 2> ou . para todos> 	|(adiciona os arquivos para um próximo commit do git)				|
|git add -i 														|	(modo iterativo)												|
|git commit -m "<comentário>" 										|(cria um commit com comentário)									|
|git commit -a 														|(a opção -a inclui imediatamente no commit todos os arquivos modificados ou removidos! Porém, ela não adiciona os arquivos novos)	|
|git config --global user.email "<you@example.com>" 				|	(configura o email do usuário)									|
|git config --global user.name "<Your Name>" 						|(configura o nome do usuário)										|
|git clone https://github.com/blablabla/projeto.git 				|	(baixa a última versão do projeto)								|
|git fetch origin --prune 											|(atualiza as branchs locais verificando as excluídas no remote)	|
|git fetch --tags                                | (atualiza a lista de tags)	|
|git checkout 1.0.14-35 <-- numero da tag        | (faz o checkout a partir de uma tag)          |
|git merge origin/[numero da tag]              | (faz merge a partir de uma tag) |
|git branch -r 														|(exibe todas as branchs do remote)									|
|git checkout <branch> 												|(usa a branch)														|
|git checkout -b <branch> 											|(cria branch)														|
|git merge <desenvolvimento> 										|(realizar ação para atualizar sua branch a partir de outra)		|
|git format-patch -1 master                                         |	Cria um arquivo de patch																|
|git format-patch -1 <sha>                                         |	Cria um arquivo de patch de um commit específico |
|git stash show -p stash@{0} > patch.txt                                |	Cria um arquivo de patch de uma stash					|
|git apply patch.txt                                         |	Aplica o arquivo de patch																|
|git diff v0.1 v0.2 												|	(verifica as diferenças entre os arquivos)						|
|git blame css/index.css 											|(lista todo os histórico detalhado do arquivo indicado)			|
|git tag 															|(ver versões do seu projeto)										|
|git log 															|(lista os commits e seus comentários)								|
|git log -p 														|	(imprime também os commits nos quais não houve modificação)		|
|git wathchanged -p 												|	(mais detalhado)												|
|gitk 														|	historico visual do git								|
|git remote 														|	(mostra os repositorios remotos)								|
|git remote add origin <url do github> 								|(linka o repositorio local com o remoto do github)					|
|git push <origin> <master> 										|	(anvia os commits para o repositorio e a branch designada)		|
|git push -u ou --set-upstream 										|(atrela a branch remota à local, fazendo com que não seja mais necessário passar como parâmetros a origem e a branch no comando)	|
|`git config --system core.longpaths true`        | configuração para o git aceitar arquivos com com path muito extenso  |
|`gitk --all $( git fsck --no-reflog | awk '/dangling commit/ {print $3}' )`    | abre o gitk exibindo todos os commits (bom para o caso acidental de deleção de stash) |
|`git branch <nome da branch> <sha de 7 digitos>`            | cria uma branch local com o commit requerido |
|`git stash apply <nome da branch>`             | aplica a branch local |
|`grep -lr '<<<<<<<' --include="pom.xml" | xargs git merge origin/development -X ours` | comando louco muito específico para uma galerinha do barulho |
  


* working directory: representa o estado atual dos arquivos no repositório;
* index, ou staging area: representa uma visão preliminar das modificações que queremos definir para nosso projeto. Podemos utilizar o comando git add para adicioná-los;
* HEAD: último passo completo do nosso projeto. Serve de referência para comparação do trabalho com o working directory.
