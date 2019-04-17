# GIT

| Comando                                       					| Descrição                                							|
| :-------------------                            					| :-------------------                  							|
|git init 															|(inicializa o controle do git no local requisitado)				|
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
|git branch -r 														|(exibe todas as branchs do remote)									|
|git checkout <branch> 												|(usa a branch)														|
|git checkout -b <branch> 											|(cria branch)														|
|git merge <desenvolvimento> 										|(realizar ação para atualizar sua branch a partir de outra)		|
|git format-patch -1 master                                         |																	|
|git diff v0.1 v0.2 												|	(verifica as diferenças entre os arquivos)						|
|git blame css/index.css 											|(lista todo os histórico detalhado do arquivo indicado)			|
|git tag 															|(ver versões do seu projeto)										|
|git log 															|(lista os commits e seus comentários)								|
|git log -p 														|	(imprime também os commits nos quais não houve modificação)		|
|git wathchanged -p 												|	(mais detalhado)												|
|git remote 														|	(mostra os repositorios remotos)								|
|git remote add origin <url do github> 								|(linka o repositorio local com o remoto do github)					|
|git push <origin> <master> 										|	(anvia os commits para o repositorio e a branch designada)		|
|git push -u ou --set-upstream 										|(atrela a branch remota à local, fazendo com que não seja mais necessário passar como parâmetros a origem e a branch no comando)	|


* working directory: representa o estado atual dos arquivos no repositório;
* index, ou staging area: representa uma visão preliminar das modificações que queremos definir para nosso projeto. Podemos utilizar o comando git add para adicioná-los;
* HEAD: último passo completo do nosso projeto. Serve de referência para comparação do trabalho com o working directory.
