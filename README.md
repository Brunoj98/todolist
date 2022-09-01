# todolist

FUNDAMENTOS DESSE TO DO LIST.

Adicionar nova tarefa
Completar e "descompletar" tarefa 
Editar a tarefa 
Excluir uma tarefa
Criar busca 
Criar filtro
Salvar todos os dados na local storage
----

- O 'retângulo' do ToDo, ficará dentro do Container.
- O Background do site, ficará dentro do Body.
- Cabeçalho ficará dentro do container em uma tag sêmantica (HEADER).
- Form contendo 1 Parágrafo (Adicione a sua tarefa:).
- Dentro do Form tem uma div(form-control), que englobará tanto o input quanto um button de submit
o button de submit tera um type="submite", para enviar o formulário.
- Para dar forma ao button, usei "fa-thin.fa-plus" = (<i class="fa-thin fa-plus"></i>)
- Form id="edit-form" = Formulário de edição, dentro dele criei uma div com um input do tipo
texto.
- Ainda dentro do "edit-form", criei um button do tipo submit para personalizar o botão usei:
<i class="fa-solid fa-check-double"></i>.
- Criei um button para cancelar a edição ID="cancel-edit-btn". (Simplesmente cancela o que a gente estava querendo fazer e o usuário pode voltar onde estava normalmente).
- Após o formulário, criei uma div="toolbar".
- Por que Toolbar? Porque é a nossa barra de ferramentas. (PESQUISA) e (FILTRO)
- Dentro da Toolbar, criei outra div="search"(Pra gente poder selecionar ele posteriormente, e coloquei um <h4>Pesquisar:</h4>.
- Ainda dentro da "search" criei um formulário abaixo do "Pesquisar" e um input
do tipo texto, um ID="search-input" e também um Placeholder="Buscar", aqui eu não tenho submit por que o usuário vai digitar e automáticamente já vai sair "buscando".
- Vamos ter um button com ID="erase=button", qual será a função dele? apagar o que o usuário digitou, caso queira limpar a busca é só clicar ali e não precisar ficar apertando backspace.
-Depois de "search" criei uma div="filter"
- Dentro de filter vou ter um <h4>Filtrar</h4>, e um "select".
- Dentro do Select o usuário vai ter algumas opções:
		    					<option value="all">Todos</option>
                    					<option value="done">Feitos</option>
                    					<option value="todo">A fazer</option>
* all = Todos
* Done = Tarefas Feitas
* Todo = Tarefas a fazer

- Por fim, criei uma div="todo-list", e dentro dela criei outra div="todo".
- Dentro da "todo" adicionei alguns buttons usando "class", como vou ter que trabalhar
- repetindo alguns botões, tive que usar "class" ao invés de "ID".
EXEMPLO: <div class="todo">
                	<div class="todo">
                <h3>Estou fazendo alguma coisa...</h3>
                <button class="finish-todo">
                    <i class="fa-solid fa-check"></i>
                </button>
                <button class="edit-todo">
                    <i class="fa-solid fa-pen"></i>
                </button>
                <button class="remove-todo">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="todo">
                <h3>Estudar Javascript...</h3>
                <button class="finish-todo">
                    <i class="fa-solid fa-check"></i>
                </button>
                <button class="edit-todo">
                    <i class="fa-solid fa-pen"></i>
                </button>
                <button class="remove-todo">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
	
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~FINALIZADO A PARTE DE HTML~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

--- COMPLEMENTOS...
#DEFER = Como vamos trabalhar manipulando o DOM, o uso desse atributo vai fazer os arquivos
gerar primeiro que o HTML. Antigamente usava pra fazer isso usava o <script> no fim do Body
mas com esse atributo 'DEFER', não precisa mais disso.

#Font Awesomes = Biblioteca de itens usada nesse projeto.
