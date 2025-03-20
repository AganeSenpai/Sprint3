Challenge API - Logística Empresarial

Integrantes:

Nome: Fernando Shinji Tanigushi RM: 553587

Nome: Carlos Eduardo Ariza Sartorio RM: 553461

Nome: João Vitor Valaitis Paulo RM: 553972

Bem-vindo ao projeto Challenge! Esta API foi desenvolvida para gerenciar a checagem de sinistros na área de odontologia, auxiliando na verificação da veracidade das informações.

📋 Funcionalidades Principais

Gerenciamento de Usuários (Funcionários e Dentistas)

Registro e acompanhamento de Sinistros

Controle de Visitas

Verificação e validação de informações

🛠️ Tecnologias Utilizadas

.NET 8

ASP.NET Core Web API

Entity Framework Core

Oracle Database

Swagger/OpenAPI

xUnit (para testes)

Docker (opcional)

🏗️ Arquitetura

O projeto Challenge foi desenvolvido seguindo a Clean Architecture, dividindo a aplicação em camadas para garantir maior manutenção, escalabilidade e organização. As principais camadas incluem:

Domain: Responsável pelas entidades e regras de negócio.

Application: Contém os casos de uso e serviços da aplicação.

Infrastructure: Gerencia a comunicação com o banco de dados e outras ferramentas.

API: Disponibiliza endpoints para acesso aos recursos da aplicação.

Abordagem Escolhida: Arquitetura Monolítica

Optamos por uma arquitetura monolítica devido aos seguintes fatores:

Simplicidade: A estrutura monolítica é mais simples de desenvolver e gerenciar no início do projeto.

Custo: Com uma equipe reduzida, manter uma aplicação monolítica reduz os custos operacionais.

Comunicação Direta: Não há necessidade de comunicação entre múltiplos serviços, reduzindo a latência e possíveis falhas.

Facilidade de Testes: Com todos os componentes em um único local, os testes são mais rápidos e eficientes.

No entanto, o projeto foi desenvolvido de forma modular, permitindo uma futura transição para microsserviços caso haja crescimento da aplicação.

🧑‍💻 Configuração do Ambiente

Pré-requisitos:

Visual Studio ou Visual Studio Code

.NET 8 SDK

Oracle Database (ou Docker com imagem do Oracle)

Postman ou qualquer ferramenta para testar APIs

Configurando a String de Conexão

No arquivo appsettings.json, configure a string de conexão para o Oracle:

🚀 Execução do Projeto

Clone o repositório.

Navegue até a pasta do projeto.

Restaure as dependências.

Execute as migrações para criar o banco de dados.

Execute a aplicação.

Acesse o Swagger em: http://localhost:5000/swagger/index.html

🛎️ Endpoints Disponíveis

Usuários

GET /api/Usuarios - Lista todos os usuários

GET /api/Usuarios/{id} - Busca um usuário por ID

POST /api/Usuarios - Cria um novo usuário

PUT /api/Usuarios/{id} - Atualiza um usuário existente

DELETE /api/Usuarios/{id} - Remove um usuário

Sinistros

GET /api/Sinistros - Lista todos os sinistros

GET /api/Sinistros/{id} - Busca um sinistro por ID

POST /api/Sinistros - Cria um novo sinistro

PUT /api/Sinistros/{id} - Atualiza um sinistro existente

DELETE /api/Sinistros/{id} - Remove um sinistro

Visitas

GET /api/Visitas - Lista todas as visitas

GET /api/Visitas/{id} - Busca uma visita por ID

POST /api/Visitas - Cria uma nova visita

PUT /api/Visitas/{id} - Atualiza uma visita existente

DELETE /api/Visitas/{id} - Remove uma visita
