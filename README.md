<h1>SAS BRASIL CHALLANGE</h1>

<h2>Descrição</h2>
<p>Projeto criado para a companhia SAS BRASIL como forma de participação no processo seletivo para Programador Júnior.</p>

<h2>Status</h2>
<p>Projeto em andamento</p>

<h2>Pré-requisitos</h2>
<a href="https://www.docker.com/products/docker-desktop">Docker</a>
<a href="https://classic.yarnpkg.com/en/docs/install/#mac-stable">Yarn</a>
<a href="https://git-scm.com/downloads">Git</a>
<a href="https://nodejs.org/en/download/">Node</a>

<h2>Como usar</h2>

<h3>Clone este projeto</h3>
<ol>
    <li>git clone https://github.com/leonardo-santoz/sasbrasilchallange-api.git</li>
    <li>cd sasbrasilapichallange-api</li>
</ol>

<h3>Instale as dependências</h3>
<ol>
    <li>yarn</li>
</ol>

<h3>Configure o banco de dados</h3>
<ol>
    <li>docker run --name sasbrasil_db -e POSTGRES_PASSWORD=saspostgres@ -p 5432:5432 -d postgres:alpine</li>
    <li>Abra um gerenciador de banco de dados de sua preferência. Sugiro fortmente o <a href="https://dbeaver.io/">dbeaver</a></li>
    <li>Crie uma conexão postgres utilizando database postgres e password saspostgres@</li>
    <li>crie uma database com o nome sasbrasil_db</li>
</ol>

<h3>Execute as migrations</h3>
<ol>
    <li>yarn sequelize db:migrate</li>
</ol>

<h3>Execute o projeto</h3>
<ol>
    <li>yarn dev:server</li>
</ol>

<h2>Para testar as rotas...</h2>
<ol>
    <li>Instale o <a href="https://insomnia.rest/download/">insomnia core</a>, execute-o e importe o arquivo sasbrasil-docs.json</li>
</ol>
