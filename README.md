<h1 align="center">Sistema de Informações Climáticas em Tempo Real</h1>

<p align="center">
  Aplicação Java que consulta informações climáticas em tempo real de qualquer cidade do mundo através da WeatherAPI.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 17"/>
  <img src="https://img.shields.io/badge/Apache_Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" alt="Maven"/>
  <img src="https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white" alt="JSON"/>
  <img src="https://img.shields.io/badge/API_REST-4CAF50?style=for-the-badge" alt="API REST"/>
</p>

<hr>

<h2>Demonstração</h2>

<p align="center">
  <img src="./assets/demo.gif" alt="Demonstração do projeto rodando" width="700"/>
</p>

<hr>

<h2>Sobre o Projeto</h2>

<p>
  Este projeto foi desenvolvido como prática de consumo de APIs REST em Java, aplicando boas práticas de segurança com variáveis de ambiente e gerenciamento de dependências via Maven. O usuário informa o nome de uma cidade e recebe dados climáticos atualizados em tempo real.
</p>

<h2>Funcionalidades</h2>

<ul>
  <li>Busca de informações climáticas por nome da cidade</li>
  <li>Exibição de temperatura atual e sensação térmica</li>
  <li>Consulta de umidade do ar</li>
  <li>Informações sobre velocidade do vento</li>
  <li>Leitura de pressão atmosférica</li>
  <li>Descrição da condição climática</li>
  <li>Tratamento de erros para cidades não encontradas</li>
</ul>

<h2>Tecnologias Utilizadas</h2>

<ul>
  <li><strong>Java 17</strong> — Linguagem principal</li>
  <li><strong>Maven</strong> — Gerenciamento de dependências e build</li>
  <li><strong>HttpClient</strong> — Cliente HTTP nativo do Java para requisições</li>
  <li><strong>org.json</strong> — Biblioteca para manipulação de JSON</li>
  <li><strong>dotenv-java</strong> — Gerenciamento de variáveis de ambiente</li>
  <li><strong>WeatherAPI</strong> — API externa de dados climáticos</li>
</ul>

<h2>Como Executar</h2>

<h3>Pré-requisitos</h3>

<ul>
  <li>Java 17 ou superior instalado</li>
  <li>Maven instalado</li>
  <li>Chave gratuita da <a href="https://www.weatherapi.com/signup.aspx">WeatherAPI</a></li>
</ul>

<h3>Passos</h3>

<p><strong>1.</strong> Clone o repositório:</p>

<pre><code>git clone https://github.com/MauroFJ/Sistema-Informacoes-Climaticas.git
cd Sistema-Informacoes-Climaticas.git</code></pre>

<p><strong>2.</strong> Crie um arquivo <code>.env</code> na raiz do projeto (baseado no <code>.env.example</code>) e adicione sua chave da API:</p>

<pre><code>WEATHER_API_KEY=sua_chave_aqui</code></pre>

<p><strong>3.</strong> Compile e execute pelo Maven:</p>

<pre><code>mvn compile exec:java -Dexec.mainClass="ProjetoSistemaDeInformacaoClimaticaEmTempoReal" -q</code></pre>

<h2>Exemplo de Saída</h2>

<pre><code>Digite o nome da cidade: São Paulo

Informações Metereológicas para São Paulo, Brazil
Data e Hora 2026-04-16 14:30
Temperatura Atual 24.5°C
Sensação Térmica 25.8°C
Condição do Tempo Partly cloudy
Umidade 65%
Velocidade do Vento 12.4 km/h
Pressão Atmosférica 1015.0 mb</code></pre>

<h2>Segurança</h2>

<p>
  A chave da API é armazenada no arquivo <code>.env</code>, que é ignorado pelo Git (através do <code>.gitignore</code>), garantindo que credenciais sensíveis não sejam expostas no repositório. Um arquivo <code>.env.example</code> é fornecido como referência para quem for configurar o projeto.
</p>

<h2>Estrutura do Projeto</h2>

<pre><code>Projeto-Informacoes-Climaticas/
├── assets/
│   └── demo.gif
├── src/
│   └── main/java/
│       └── ProjetoSistemaDeInformacaoClimaticaEmTempoReal.java
├── .env.example
├── .gitignore
├── pom.xml
└── README.md</code></pre>

<hr>


<h2>
  Desenvolvido por <strong>Mauro</strong>
</h2>

<p>
  <a href="https://github.com/MauroFJ">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://linkedin.com/in/MauroFJ">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
</p>
