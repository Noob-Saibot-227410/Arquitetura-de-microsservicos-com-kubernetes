<!DOCTYPE html>
<html>
<body>
  <h1><i class="fas fa-code"></i> Projeto de Arquitetura de Microsserviços com Python e Kubernetes</h1>
  <h2><i class="fas fa-cog"></i> Pré-requisitos</h2>
  <ul>
<li><img src="https://img.icons8.com/color/48/000000/python.png"/> Python 3.6 ou superior</li>
<li><img src="https://img.icons8.com/color/48/000000/docker.png"/> Docker</li>
<li><img src="https://img.icons8.com/color/48/000000/kubernetes.png"/> Kubernetes</li>
<li><img src="https://img.icons8.com/color/48/000000/database-restore.png"/> Banco de dados (MySQL, Postgres, etc)</li>
  </ul>

  <h2><i class="fas fa-play"></i> Passo a Passo</h2>

  <h3>1. Clonar o repositório</h3>
  <pre><code>git clone https://github.com/seu-usuario/projeto-microsservicos.git
cd projeto-microsservicos
</code></pre>

  <h3>2. Criar imagens Docker</h3>
  <pre><code>docker build -t api-nomes:latest api-nomes/
docker build -t api-idades:latest api-idades/
</code></pre>

  <h3>3. Criar deploy e serviço no Kubernetes</h3>
  <pre><code>kubectl apply -f kubernetes/
</code></pre>

  <h3>4. Acessar a aplicação</h3>
  <p>Acesse a URL <code>http://localhost:8000</code> em seu navegador.</p>

  <h2><i class="fas fa-folder"></i> Estrutura do Projeto</h2>
  <ul>
    <li><strong>api-nomes/</strong>: API responsável por gerenciar os nomes dos usuários</li>
    <li><strong>api-idades/</strong>: API responsável por gerenciar as idades dos usuários</li>
    <li><strong>kubernetes/</strong>: Arquivos de deploy e serviço do Kubernetes</li>
  </ul>

  <h2><i class="fas fa-info-circle"></i> Informações Adicionais</h2>
  <p>Este projeto é apenas para fins educacionais.</p>

</body>

</html>
