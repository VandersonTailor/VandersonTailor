<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Perfil - Vanderson Pinheiro</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            margin: 0;
            padding: 40px;
        }

        .container {
            max-width: 900px;
            margin: auto;
            background: #161b22;
            border-radius: 8px;
            padding: 20px;
        }

        h1 {
            text-align: center;
            color: #58a6ff;
        }

        /* Tabs */
        .tabs {
            display: flex;
            border-bottom: 2px solid #30363d;
            margin-bottom: 20px;
        }

        .tab {
            padding: 10px 20px;
            cursor: pointer;
            color: #8b949e;
        }

        .tab.active {
            color: #58a6ff;
            border-bottom: 3px solid #58a6ff;
            font-weight: bold;
        }

        /* Conteúdo */
        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
        }

        ul {
            line-height: 1.8;
        }

        .badge {
            display: inline-block;
            background: #238636;
            padding: 4px 8px;
            border-radius: 6px;
            margin: 4px;
            font-size: 14px;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>👋 Vanderson Pinheiro</h1>

    <div class="tabs">
        <div class="tab active" onclick="openTab('sobre')">Sobre</div>
        <div class="tab" onclick="openTab('skills')">Skills</div>
        <div class="tab" onclick="openTab('projetos')">Projetos</div>
        <div class="tab" onclick="openTab('contato')">Contato</div>
    </div>

    <div id="sobre" class="tab-content active">
        <p>
            Desenvolvedor Backend com foco em <strong>Java</strong>, APIs REST,
            automação de processos e sistemas web.
        </p>
        <p>
            Formado em Análise e Desenvolvimento de Sistemas, sempre buscando
            código limpo, boas práticas e soluções eficientes.
        </p>
    </div>

    <div id="skills" class="tab-content">
        <h3>💻 Tecnologias</h3>
        <span class="badge">Java</span>
        <span class="badge">Spring Boot</span>
        <span class="badge">REST API</span>
        <span class="badge">SQL</span>
        <span class="badge">JavaScript</span>
        <span class="badge">React</span>
        <span class="badge">Node.js</span>
        <span class="badge">Git</span>
        <span class="badge">Linux</span>
    </div>

    <div id="projetos" class="tab-content">
        <ul>
            <li>Sistemas internos de gestão</li>
            <li>APIs REST com Spring Boot</li>
            <li>Automação de relatórios</li>
            <li>Dashboards e painéis administrativos</li>
        </ul>
    </div>

    <div id="contato" class="tab-content">
        <p>📧 Email: seu-email@email.com</p>
        <p>💼 LinkedIn: linkedin.com/in/seu-perfil</p>
        <p>🐙 GitHub: github.com/seu-usuario</p>
    </div>
</div>

<script>
    function openTab(tabId) {
        const tabs = document.querySelectorAll('.tab');
        const contents = document.querySelectorAll('.tab-content');

        tabs.forEach(tab => tab.classList.remove('active'));
        contents.forEach(content => content.classList.remove('active'));

        document.getElementById(tabId).classList.add('active');
        event.target.classList.add('active');
    }
</script>

</body>
</html>
