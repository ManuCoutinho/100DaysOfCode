![image](https://github.com/ManuCoutinho/100DaysOfCode/blob/main/hacktoberfest_logo.png)
# Hacktoberfest 2022

## Começando

Confira [Contribution](https://github.com/ManuCoutinho/100DaysOfCode/blob/9ebf6125dd01ce503c3b3da5f5ac8459114688cc/CONTRIBUTING.md) Guia de Contribuição.

## Instruções:

*Certifique-se de ter uma conta no GitHub. Caso você não tenha uma, você pode criar sua conta visitando https://github.com/ e clicando na opção ``Sign up`` no canto superior direito.*

### 1. Registre-se no Hacktoberfest
##### Link para inscrição: https://hacktoberfest.digitalocean.com/
Clique em "Start Hacking" e adicione sua conta do GitHub.

### 2. Dê uma estrela e 'fork' este repositório
##### Você pode iniciar e  dá 'fork' neste repositório no GitHub navegando na parte superior deste repositório.

Quando você estiver na página principal de um repositório, verá um botão para "Star" e "Fork" o repositório no canto superior direito da página, abaixo do ícone do usuário.

### 3. Clone o repositório

Para fazer sua própria cópia local do repositório com o qual você gostaria de contribuir, vamos primeiro abrir uma janela de terminal.

Usaremos o comando `git clone` junto com a URL que aponta para sua bifurcação do repositório.

Esta URL será semelhante à URL acima, exceto que agora terminará com `.git.` Como exemplo, a URL poderá se apresentar assim: https://github.com/your-username/Hacktoberfest.git

Você também pode copiar a URL usando o botão verde “Clone or download” da página do repositório que você acabou de bifurcar da página do repositório original. Depois de clicar no botão, você poderá copiar o URL clicando no botão do fichário ao lado do URL:

Assim que tivermos a URL, estamos prontos para clonar o repositório. Para fazer isso, combinaremos o comando git clone com a URL do repositório na linha de comando em uma janela de terminal, ficando algo como a seguir:

`git clone https://github.com/your-username/100DaysOfCode.git`

### 4. Crie uma nova branch

Para criar sua ramificação(Branch), na janela do seu terminal, altere seu diretório para que você esteja trabalhando no diretório do repositório. Certifique-se de usar o nome real do repositório (ou seja, 100DaysOfCode) para alternar para esse diretório.

##### `cd 100DaysOfCode`

Agora, vamos criar nosso nova branch com o comando git branch. Certifique-se de nomeá-lo de forma descritiva para que outras pessoas que trabalham no projeto entendam no que você está trabalhando.


##### `git branch nome-da-nova-branch`

Agora que nossa nova ramificação foi criada, podemos alternar para ter certeza de que estamos trabalhando nessa ramificação usando o comando git checkout:

##### ` git checkout nova-branch `

Depois de inserir o comando git `checkout`, você receberá a seguinte saída:

###### `Saída:`
##### `Switched to branch 'nova-branch' `


Neste ponto, você pode modificar os arquivos existentes ou adicionar novos arquivos ao projeto em sua própria ramificação.

#### Faça alterações localmente

Depois de modificar os arquivos existentes ou adicionar novos arquivos ao projeto, você pode adicioná-los ao seu repositório local, o que pode ser feito com o comando git add. Vamos adicionar o sinalizador -A para adicionar todas as alterações que fizemos:

##### ` git add -A ` ou ` git add . `

Em seguida, queremos registrar as alterações que fizemos no repositório com o comando git commit.

*A mensagem do commit é um aspecto importante da contribuição do seu código; ele ajuda os outros contribuidores a entender completamente a mudança que você fez, por que a fez e quão significativa ela é. Além disso, as mensagens de confirmação fornecem um registro histórico das alterações do projeto em geral, ajudando futuros colaboradores ao longo do caminho.*


Se você tiver uma mensagem muito curta, poderá gravá-la com o sinalizador -m e a mensagem entre aspas:

###### ` Exemplo: `
##### ` git commit -m "Readme.md atualizado" `

###### Neste ponto, você pode usar o comando git push para enviar as alterações para o branch atual do seu repositório bifurcado:
###### ` Exemplo:`
##### ` git push -u origin nova-branch `

### 5. Atualize o repositório local

*Ao trabalhar em um projeto junto com outros contribuidores, é importante que você mantenha seu repositório local atualizado com o projeto, pois você não deseja fazer uma solicitação pull de código que causará conflitos. Para manter sua cópia local da base de código atualizada, você precisará sincronizar as alterações.*

Primeiro vamos configurar um controle remoto para o fork e depois sincronizar o fork.

### 6. Configure um Remote para o Fork

Em seguida, você terá que especificar um novo repositório upstream remoto para sincronizarmos com o fork. Este será o repositório original do qual você fez o fork. você terá que fazer isso com o comando git remote add.

##### ` git remote add upstream https://github.com/ManuCoutinho/100DaysOfCode `

Neste exemplo, // upstream // é o nome abreviado que fornecemos para o repositório remoto, pois em termos de Git, “upstream” refere-se ao repositório do qual você clonou. Se quiser adicionar um ponteiro remoto ao repositório de um colaborador, você pode fornecer o nome de usuário desse colaborador ou um apelido abreviado para o nome abreviado.

### 7. Sincronize a bifurcação

Depois de configurar um controle remoto que faz referência ao repositório upstream e original no GitHub, você está pronto para sincronizar sua bifurcação do repositório para mantê-lo atualizado.
Para sincronizar seu fork, do diretório do seu repositório local em uma janela de terminal, você terá que usar o comando // `git fetch` // para buscar os branches junto com seus respectivos commits do repositório upstream. Como você usou o nome abreviado “upstream” para se referir ao repositório upstream, você terá que passar isso para o comando:

##### ` git fetch upstream `

Mude para o branch master local do nosso repositório:

##### ` git checkout main `

Agora mescle quaisquer alterações que foram feitas no branch principal do repositório original, que você acessará através do seu branch upstream/main local, com o seu branch principal local:

##### ` git merge upstream/main `

### 8. Criar solicitação pull

Neste ponto, você está pronto para fazer um `pull request` para o repositório original.

Navegue até o seu repositório bifurcado e pressione o botão “Nova solicitação pull” no lado esquerdo da sua página Repo.

### Show! Você acabou de chegar mais perto de completar seu desafio Hacktoberfest.