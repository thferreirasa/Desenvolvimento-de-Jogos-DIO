# Curso Versionamento de Código com Git e GitHub

Tabela com os comandos que podem ser usados no GitBash que aprendi durante o curso:

Linha de Comando | O que faz
------- | ---------
git config --global credential.helper cache | salva credencial do GitHub temporiariamente na máquina
git config -global credential.helper store | salva credencial do GitHub permanentemente na máquina
cat | + nome do arquivo, mostrar conteúdo do arquivo
ls | listar arquivos do diretório
-al | ao usar o comando ls, mostrar arquivos ocultos
~ | significa que está no diretório atual
. | significa pasta/arquivo oculto
git clone | + url, copia repositório remoto localmente, no final pode colocar um novo nome para o repositório (só localmente)
mkdir | + nome da pasta, cria pasta
cd | + nome da pasta, abre a pasta
git remote -v | mostra repositórios remotos que está vinculado
git remote add origin | + url, vincular repositório local a remoto
git clone _url_ --branch _nomedabranch_ --single-branch | clona uma branch específica
git status | mostra o status da árvore de preparação/staging area
touch | + nome do arquivo, cria arquivo vazio
git add | + nome do arquivo ou . , adiciona arquivo na área de preparação/staging area
git commit -m "_mensagem_" | faz commit dos arquivos da área de preparação/staging area
git push -u origin main | envia alterações locais para o repositório remoto
git pull | atualiza repositório local com informações do repositório remoto
git log | histórico de commits
echo _nomedoarquivo_ >.gitignore | o Git ignora o arquivo ou pasta
echo >.gitignore | remove o arquivo ou pasta do .gitignore, e o Git reconhece ele
touch _nomepasta_/.gitkeep | cria pasta vazia que o Git reconhece
rm -rf .git | diretório deixa de ser repositório Git
git restore | + nome do arquivo, restaura versão anterior
git commit --amend -m "_mensagem_" | cria novo título para commit
git reset --soft _id do commit_ | desfaz commit, pegando os arquivos que estavam nos commits posteriores ao indicado e adicionam eles na staging area
git reset --mixed _id do commit_ | desfaz commit, padrão de git reset, pega os arquivos dos commits posteriores ao indicado e adiciona na árvore de trabalho como untracked files
git reset --hard _id do commit_ | desfaz commit, ignora completamente arquivos de commits anteriores e desfaz eles
git reflog | histórico mais detalhado das alterações feitas
git restore --staged | + nome do arquivo, tira arquivos da staging area
git chekout -b | + nome da branch, cria branch nova e entra nela
git checkout main | volta pra branch principal
git branch -v | mostra o último commit de cada branch
git merge | + nome da branch, mescla a branch com a main branch
git stash | retira/arquiva modificação
git stash list | lista modificações arquivadas
git stash pop | traz alteração arquivada de volta para a branch, exclui alteração da lista de alterações arquivadas
git stash apply | traz alteração arquivada de volta para a branch, mantém alteração da lista de alterações arquivadas