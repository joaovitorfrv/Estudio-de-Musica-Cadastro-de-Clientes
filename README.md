# Cadastro de Clientes para Estúdio de Música

Este projeto é uma aplicação full-stack desenvolvida para o gerenciamento de clientes de um estúdio de música. A aplicação permite realizar o cadastro, edição, exclusão e busca de clientes, além de exibir uma listagem completa dos registros na tela principal.

O sistema é composto por uma API no backend desenvolvida com **Flask** e uma interface de usuário no frontend utilizando **HTML**, **CSS** e **JavaScript** puro (Vanilla).

## 🚀 Funcionalidades

- **Listar Clientes**: Visualização de todos os clientes cadastrados no banco de dados.
- **Cadastrar Cliente**: Inserção de novos clientes com nome, data de nascimento, e-mail, celular e instrumentos.
- **Editar Cliente**: Atualização das informações de um cliente já existente na base.
- **Excluir Cliente**: Remoção de registros de clientes.
- **Buscar Cliente**: Pesquisa de clientes pelo nome através da barra de busca.

## 🛠️ Tecnologias Utilizadas

**Backend:**
- Python 3.x
- Flask
- SQLite (Banco de Dados)
- Swagger / OpenAPI (Documentação e testes da API)

**Frontend:**
- HTML5
- CSS3
- JavaScript

## ⚙️ Pré-requisitos

Antes de iniciar, certifique-se de ter instalado em sua máquina:
- [Python 3.x](https://www.python.org/downloads/)
- Ferramenta para criação de ambientes virtuais (`venv`)

## 🚀 Como Executar o Projeto

Para visualizar a interface e utilizar o sistema corretamente, **é necessário que o backend esteja em execução** antes de interagir com o frontend.

### 1. Clonando o repositório

```bash
git clone [https://github.com/joaovitorfrv/Engenharia-de-Software-MVP-Sprint-1](https://github.com/joaovitorfrv/Engenharia-de-Software-MVP-Sprint-1)
cd Engenharia-de-Software-MVP-Sprint-1
```

### 2. Configurando e Iniciando o Backend (API)

Na raiz do diretório do projeto, crie e ative o ambiente virtual:

1. **Crie o ambiente virtual:**
   ```bash
   python -m venv venv
   ```

2. **Ative o ambiente virtual:**
   - No **Windows**: `.\venv\Scripts\activate`
   - No **Linux/MacOS**: `source venv/bin/activate`

3. **Instale as dependências:**
   ```bash
   pip install -r app_back_end/requirements.txt
   ```

4. **Inicie o servidor Flask:**
   Navegue até a pasta do backend e inicie a aplicação:
   ```bash
   cd app_back_end
   flask run --host 0.0.0.0 --port 5000
   ```
   *A documentação da API (via Swagger) estará disponível no navegador em `http://127.0.0.1:5000`.*

### 3. Executando o Frontend

Com a API rodando no terminal, você pode acessar a interface do usuário:

1. Navegue até a pasta `app_front_end`.
2. Abra o arquivo `index.html` diretamente em seu navegador web. 
3. O arquivo `script.js` gerenciará todas as interações e fará as requisições CRUD diretamente para a API local.

## 📂 Estrutura do Projeto

```text
├── app_back_end/          # Backend da aplicação (API)
│   ├── app.py             # Arquivo principal de rotas e inicialização
│   ├── model/             # Modelos de dados e configuração do banco
│   ├── schemas/           # Schemas para validação de dados
│   ├── database/          # Banco de dados SQLite
│   └── requirements.txt   # Dependências do Python
├── app_front_end/         # Interface do usuário (Frontend)
│   ├── images/            # Ícones de ação (editar, excluir, etc.)
│   ├── index.html         # Estrutura principal da página
│   ├── style.css          # Estilização visual
│   └── script.js          # Lógica de integração com a API e manipulação do DOM
├── venv/                  # Ambiente virtual Python (gerado localmente)
└── README.md              # Documentação geral do projeto
```

## ✒️ Autor

- **João Vitor M. Frugiuele**

## 📄 Licença

Este projeto está licenciado sob a licença **MIT**.
