LiterAlura - Catálogo de Livros

Descrição do Projeto
O LiterAlura é um catálogo de livros interativo desenvolvido em Java que permite buscar, armazenar e consultar informações sobre livros e autores. O projeto consome dados da API Gutendex (baseada no Projeto Gutenberg), armazena as informações em um banco de dados local e oferece uma interface de console para interação com o usuário.

Funcionalidades Principais
✔ Busca de livros por título através da API Gutendex
✔ Armazenamento em banco de dados (H2 embutido ou configurável)
✔ Consultas avançadas:

Listar todos os livros cadastrados

Listar todos os autores registrados

Filtrar autores vivos em um determinado ano

Buscar livros por idioma (ex: en, es, pt, fr)
✔ Interface textual intuitiva via console

Tecnologias e Requisitos

Java JDK 17+

Maven (gerenciamento de dependências)

Spring Boot (framework base)

Spring Data JPA + Hibernate (persistência)

Banco de dados H2 (padrão) ou configuração para MySQL/PostgreSQL

Jackson (processamento de JSON)

HTTP Client (consumo da API)

Configuração Inicial

Clone o repositório:

git clone [URL_DO_REPOSITORIO]  

Importe como projeto Maven na sua IDE (Eclipse, IntelliJ, etc.).

Configure o arquivo application.properties (se necessário ajustar banco de dados).

Execute a classe Main.java para iniciar.

Como Usar
Ao iniciar, o sistema exibirá um menu interativo com as opções:

Buscar livro por título: Digite um título para consultar na API.

Listar livros registrados: Mostra todos os livros salvos no banco.

Listar autores registrados: Exibe autores e seus detalhes.

Autores vivos em um ano: Filtra autores por ano de nascimento/falecimento.

Livros por idioma: Filtra por código de idioma (ex: pt para português).

Sair: Encerra a aplicação.

Estrutura do Código

src/  
├── main/  
│   ├── java/  
│   │   ├── model/          # Entidades (Livro, Autor)  
│   │   ├── repository/     # Repositórios JPA  
│   │   ├── service/        # Lógica (API Service, DB Service)  
│   │   ├── util/           # Conversores e validadores  
│   │   └── Main.java       # Ponto de entrada  
│   └── resources/         # application.properties  
└── test/                   # Testes unitários  

API Utilizada
🔗 Gutendex – Baseada no Projeto Gutenberg, oferece metadados de livros em domínio público.

Licença
MIT License. Contribuições são bem-vindas via issues ou pull requests!

Observações

Para trocar o banco de dados (ex: MySQL), ajuste as propriedades em application.properties.

O sistema é case-insensitive para buscas por título.

Idiomas suportados seguem códigos ISO 639-1 (ex: en, pt, fr).

Pronto para mergulhar no mundo dos livros! 📚✨
