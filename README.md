# Pipeline Calculadora - Priscila Mendes

Projeto desenvolvido em Python como atividade sobre Integração e Entrega Contínua, utilizando pytest para testes automatizados e GitHub Actions para execução da pipeline.

## 📋 Sobre o projeto

A aplicação consiste em uma calculadora simples que realiza quatro operações matemáticas:

- ➕ Soma
- ➖ Subtração
- ✖️ Multiplicação
- ➗ Divisão

Além da aplicação, foram criados testes automatizados para verificar se cada operação está funcionando corretamente.

## 🧪 Testes automatizados

Os testes foram desenvolvidos utilizando o pytest.

Cada operação possui um arquivo de teste próprio:

Arquivo| Operação
"test_soma.py"| Soma
"test_subtracao.py"| Subtração
"test_multiplicacao.py"| Multiplicação
"test_divisao.py"| Divisão

Para executar todos os testes localmente, utilize:

pytest

## ⚙️ GitHub Actions

O projeto possui uma pipeline configurada com GitHub Actions.

A pipeline é executada automaticamente sempre que ocorre um "push" na branch "main".

Ela realiza as seguintes etapas:

1. Faz o checkout do código do repositório.
2. Configura o Python 3.12.
3. Instala o pytest.
4. Executa os testes automatizados.

Jobs

Cada operação possui um job separado:

- "teste_soma"
- "teste_subtracao"
- "teste_multiplicacao"
- "teste_divisao"

Todos os jobs utilizam o ambiente:

runs-on: ubuntu-latest

## 🚀 Executando o projeto

### 1. Clonar o repositório

git clone URL_DO_REPOSITORIO

### 2. Entrar na pasta

cd Pipeline_Calculadora

3. Instalar o pytest

pip install pytest

4. Executar os testes

pytest

Se todos os testes estiverem funcionando corretamente, o pytest apresentará os testes como aprovados.

## 🔄 Pipeline

A pipeline está localizada em:

.github/workflows/pipeline.yml

O workflow utiliza:

- "actions/checkout@v4"
- "actions/setup-python@v5"
- Python "3.12"
- "pytest"
- "ubuntu-latest"

## 🎯 Objetivo

O objetivo do projeto é praticar a criação de uma pipeline de Integração e Entrega Contínua, utilizando GitHub Actions para automatizar a execução dos testes da aplicação.

## 👩‍💻 Tecnologias utilizadas

- Python 3.12
- Pytest
- Git
- GitHub
- GitHub Actions
