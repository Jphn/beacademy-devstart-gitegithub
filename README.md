<a href="https://www.beacademy.com.br/devstartpaylivre/" target="_blank"><img src="https://www.beacademy.com.br/wp-content/uploads/2022/02/Cubo.png" align="right" width="60"/></a>

# Git e Github - DevStart

## Comandos

Aqui vai uma lista com os principais, ou praticamente todos, os comandos apresentados durante o módulo de Git e Github lecionado pelo professor Régis Santos.

> **OBS.:** Os sinais de maior que e menor que são meramente ilustrativos e não devem ser inclusos. Todos os dados inseridos pelo usuário devem estar entre aspas duplas, exceto no caso de pontos literais. **Ex.:** ```git commit -m "mensagem"```

----------

**Configurar o nome de usuário e o email do Git.**

```sh
  git config --global user.name <nome> 
  git config --global user.email <email> 
```

----------

**Inicializar o repositório.**

> Caso o repositória já tenha sido inicializado o comando ira notificar o usuário.

```sh
  git init
```

**Mostrar o status do repositório atual.**

```sh
  git status
```

**Adicionar uma determinada alteração na lista de alterações preparadas.**

> Utilize um ponto no campo nome para adicionar todas as alterações na lista.

```sh
  git add <nome>
```

**Remover uma ou mais alterações da lista de alterações preparadas.**

> Adicione o **```-r```** antes do **```--cached```** para remover todas as alterações da lista.

```sh
  git rm --cached <nome>
```

**Preparar todas as alterações na lista com uma mensagem escrita pelo usuário.**

> Caso o usuário não esteja em um repositório compartilhado as alterações serão preparadas e automaticamente enviadas. Senão, será necessário utilizar o **```push```**.

```sh
  git commit -m <mensagem>
```

**Mostrar o log de todos os commits feitos.**

> Adicione o **```--oneline```** para facilitar a visualização das informações.

```sh
  git log
```

----------

**Mostrar a lista de todas as branchs, demarcando a branch atual.**

```sh
  git branch
```

**Criar uma branch com o nome selecionado.**

```sh
  git branch <nome>
```

**Deletar uma branch específica.**

```sh
  git branch -d <nome>
```

**Mudar para a branch selecionada.**

> Adicione o **```-b```** antes do nome da branch caso a branch em questão ainda não exista. O Git irá cria a branch e mudar para ela logo em seguida.

```sh
  git checkout <nome>
```

**Mesclar a branch selecionada com a branch atual.**

```sh
  git merge <nome>
```

----------

**Gerar uma chave SSH para linkar Git e Github.**

```sh
  ssh-keygen -t ed25519 -C <email>
```

**Clonar um repositório existente.**

```sh
  git clone <endereço>
```

**Sincronizar as informações do repositório local com as do remoto.**

```sh
  git pull 
```

**Atualizar o repositório remoto com as alterações locais.**

```sh
  git push 
```

----------

**Guardar alterações não concluidas como rascunho.**

> Adicione a opção **```--include-untracked```** para incluir novos arquivos.

```sh
  git stash
```

**Mostar lista de stashes salvos.**

```sh
  git stash list
```

**Retomar stash.**

> Especifique a stash após o pop para retomar a stash específica. Da seguinte forma **```git stash pop <stash>```**.

```sh
  git stash pop
```

**Reverter commits feitos.**

> Adicione o **```<commit>```** para especificar o commit a ser revertido.

```sh
  git revert
```

**Mostrar as diferenças entre as branchs.**

```sh
  git diff
```

## Autor

- [@Jphn](https://www.github.com/Jphn)

[![beAcademy](https://www.beacademy.com.br/wp-content/uploads/2019/11/Logo-Topo.png)](https://www.beacademy.com.br/)

[![paylivre](https://web.paylivre.com/static/media/logo-blue.c7100186.png)](https://www.paylivre.com/)
