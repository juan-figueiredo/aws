Configuração do Ambiente de Desenvolvimento com Flask e SQLite

Introdução:

Neste tutorial passo a passo, vamos configurar um ambiente de desenvolvimento para criar uma aplicação web simples usando o framework Flask e um banco de dados SQLite. Ao final deste tutorial, você terá um ambiente funcional pronto para começar a desenvolver suas próprias aplicações web em Python.

Pré-requisitos:

Python instalado (v3.6 ou superior)
Pip (gerenciador de pacotes Python) instalado
Passo 1: Instalação do Flask:

Abra seu terminal ou prompt de comando e execute o seguinte comando para instalar o Flask usando o Pip:

bash
Copy code
pip install flask
Passo 2: Criação de um Ambiente Virtual:

Crie um ambiente virtual para isolar as dependências do seu projeto. No terminal, execute os seguintes comandos:

bash
Copy code
python -m venv venv
Ative o ambiente virtual:

No Windows:

bash
Copy code
venv\Scripts\activate
No MacOS/Linux:

bash
Copy code
source venv/bin/activate
Passo 3: Estrutura do Projeto:

Crie uma estrutura básica para o projeto:

bash
Copy code
mkdir meu_projeto
cd meu_projeto
Dentro do diretório, crie um arquivo chamado app.py para o código da sua aplicação.

Passo 4: Configuração do Flask:

No arquivo app.py, adicione o seguinte código para configurar uma aplicação Flask básica:

python
Copy code
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return 'Olá, mundo!'

if __name__ == '__main__':
    app.run(debug=True)
Passo 5: Executando a Aplicação:

De volta ao terminal, execute o seguinte comando para iniciar o servidor Flask:

bash
Copy code
python app.py
Acesse http://127.0.0.1:5000/ no seu navegador para ver a mensagem "Olá, mundo!".

Conclusão:

Parabéns! Você concluiu com sucesso a configuração do ambiente de desenvolvimento com Flask e SQLite. Este é um ponto de partida sólido para futuros desenvolvimentos em Python usando o framework Flask. Fique à vontade para explorar mais recursos e expandir sua aplicação conforme necessário.






