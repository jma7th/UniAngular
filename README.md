# UniAngular
Projeto de site (SPA, ou aplicação de página única) em Angular.
Tecnologias utilizadas no BackEnd: Python, Flask, SQLite, JWT.

# Leia-me:
Após download e instalação do Python, será necessário utilizar o pip para baixar as dependências.
Para o backend basta rodar o terminal na pasta do backend com o comando "pip install -r requirements.txt". 
Depois que tudo estiver instalado, é possível rodar um servidor através do flask, pelo comando "python main.py". Tanto a aplicação quanto o servidor e banco de dados estarão acessíveis pela porta "http://localhost:5000".

Uma vez rodando, será possível logar com um dos usuários cadastrados no BD (exemplo: login jmath78, senha cuscuz8000) para fins de teste da ferramenta. Através da combinação de login "admin" e senha e "adminpw", será possível ter acesso às funcionalidades de edição de banco de dados.

O projeto está em andamento e precisa de alguns ajustes, especificamente na autenticação e na comunicação de algumas requisições HTTP entre o front e o back. Também há planos de implementar token por localstorage.

Para o front, é necessário instalar o node.js e rodar o comando "npm install", porém uma versão minificada distributiva do código já está compactada na pasta do back e não necessita desse procedimento para funcionar.

Uma vez feita essa configuração, é possível construir um novo código com o comando "ng build --base-href /static/", que construirá um código na pasta FrontEnd/dist/FrontEnd. Depois é jogar o arquivo index.html na pasta BackEnd/dist/FrontEnd e o restante na pasta BackEnd/static. Uma aplicação em Python para automatizar o processo está sendo desenvolvida.

# Funções do projeto:
-> Gerenciar salas, associa cada sala à uma disciplina, com cada disciplina associada à um curso <br>
->Autenticação de usuários (em progresso) <br>
->Todas as consultas devem ser exibidas em tabela <br>
Usuários: <br>
->admin cria/edita/deleta quaisquer sala/disciplina/curso/usuário <br>
->aluno se associa à uma sala e disciplina já previamente feita <br>
->Exibir cursos, disciplinas e salas existentes não precisa de autenticação <br>
 
# Chaves e atributos utilizados na database:
Usuário: <br>
-> id(int) <br>
->email (string) <br>
->nome (string) <br>
->login (string) <br>
->senha (string) <br>
Curso: <br>
->id (int) <br>
->nome (string) <br>
->descr(string) <br>
Disciplina: <br>
->id (int) <br>
->nome (string) <br>
->dscr(string) <br>
->Sala (OBJ Sala) <br>
->curso (OBJ curso) <br>
Sala: <br>
->id(int) <br>
->num° sala(int) <br>
->andar(int) <br>

# Desenvolvido por:
João Matheus Andrade / jma7th
Enzo da Silva dos Anjos / Enzo7274