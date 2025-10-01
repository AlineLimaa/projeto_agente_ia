# 🤖 Sistema de Análise Inteligente de Dados - Grupo Oscar Calçados

Um sistema que permite analisar dados de forma inteligente através de uma interface web simples e um assistente de IA conversacional.

## ✨ O que este sistema faz?

Este sistema foi criado para facilitar a análise de dados para pessoas que não têm conhecimento técnico avançado. Com ele você pode:

- 📊 **Importar dados** de arquivos CSV ou planilhas do Google Sheets
- 🤖 **Conversar com uma IA** que entende suas perguntas em linguagem natural
- 📈 **Visualizar dados** em tabelas organizadas
- 💡 **Obter insights** automaticamente dos seus dados
- 🚨 **Detectar fraudes** com algoritmos avançados de análise

## 🔄 Como funciona?

1. 📤 **Você importa seus dados** (arquivos CSV ou links do Google Sheets)
2. 🗄️ **O sistema organiza tudo** no banco de dados
3. 💬 **Você faz perguntas** como "Quais são os produtos mais vendidos?"
4. 🧠 **A IA analisa e responde** de forma clara e objetiva
5. 🚨 **Detecta fraudes automaticamente** quando solicitado

## 📋 O que você precisa para usar?

### Pré-requisitos básicos:

- 🐍 **Python 3.11 ou superior** (linguagem de programação)
- 🍃 **MongoDB** (banco de dados para armazenar seus dados)
- 🔑 **Chave da API OpenAI** (para o assistente de IA funcionar)

### Como obter o que precisa:

🐍 **Python**: Baixe em [python.org](https://www.python.org/downloads/)

🍃 **MongoDB**: Baixe em [mongodb.com](https://www.mongodb.com/try/download/community)

🔑 **Chave OpenAI**: Crie uma conta em [openai.com](https://openai.com) e gere uma API key

## 🚀 Instalação passo a passo

### 1. 📥 Baixe o projeto

```bash
git clone https://github.com/seu-usuario/projeto_agente_ia.git
cd projeto_agente_ia
```

### 2. 📦 Instale as dependências

```bash
pip install -r requirements.txt
```

### 3. ⚙️ Configure as variáveis de ambiente

Crie um arquivo chamado `.env` na pasta principal do projeto com o seguinte conteúdo:

```
OPENAI_API_KEY=sua_chave_openai_aqui
MONGO_URI=mongodb://localhost:27017/
DB_NAME=dbGrupoOscar
```

### 4. 🍃 Inicie o MongoDB

**Windows:**

```bash
net start MongoDB
```

**Linux/Mac:**

```bash
sudo systemctl start mongod
```

### 5. ▶️ Execute a aplicação

```bash
python main.py
```

### 6. 🌐 Acesse no navegador

Abra seu navegador e vá para: `http://localhost:5000`

## 💻 Como usar o sistema

### 📊 Importando dados

1. Na página principal, você verá uma seção "Importação de CSV"
2. Você pode:
   - 🔗 **Colar um link** do Google Sheets
   - 📁 **Enviar um arquivo CSV** do seu computador
3. Clique em "Importar" e aguarde a importação

### 🤖 Conversando com a IA

1. Na seção "Chat com Agente IA", digite sua pergunta
2. Exemplos de perguntas que você pode fazer:
   - 📊 "top 10 lojas mais frequentes em devolução"
   - 🏆 "top 5 produtos mais devolvidos"
   - 📅 "quantas devoluções aconteceram no dia 15/01/2025"
   - 🏪 "top 20 lojas com mais ajustes de estoque"
   - 👥 "top 15 usuários que mais cancelam"
   - 🚨 "faça uma análise de fraude"
   - 📋 "mostre as top 10 lojas em formato de tabela"

### 👁️ Visualizando dados

1. Na lista "Coleções existentes", clique no nome da sua coleção
2. Você verá uma tabela com todos os dados importados
3. Use a paginação para navegar entre os registros

## 💬 Exemplos de perguntas que você pode fazer

### 📊 **Rankings e Contagens (100% funcionais):**

- 🏆 "top 10 lojas mais frequentes em devolução"
- 📦 "top 5 produtos mais devolvidos"
- 👥 "top 20 usuários que mais cancelam"
- 🏪 "top 15 lojas com mais ajustes de estoque"
- 📊 "quantos registros existem na coleção de devolução"

### 📅 **Consultas por Data (100% funcionais):**

- 📅 "quantas devoluções aconteceram no dia 15/01/2025"
- 📊 "quantos cancelamentos entre 10/01 e 20/01/2025"
- 📈 "quantos ajustes de estoque no dia 25/01/2025"
- 📋 "quantas devoluções entre 01/01 e 31/01/2025"

### 📋 **Formatos de Resposta (100% funcionais):**

- 📊 "mostre as top 10 lojas em devolução em formato de tabela"
- 📦 "top 5 produtos mais frequentes em tabela"
- 🏪 "ranking das 15 lojas com mais cancelamentos em formato de tabela"

### 🚨 **Detecção de Fraude (100% funcional):**

- 🔍 "faça uma análise de fraude"
- 🚨 "relatório de fraude"
- 📊 "análise de fraude"
- 🔎 "detectar fraude"
- ⚠️ "verificar suspeitas"

### 🎯 **Diferentes Quantidades (1, 3, 5, 10, 15, 20, 50, 100):**

- 🥇 "top 1 loja mais frequente em devolução"
- 🏆 "top 3 produtos mais devolvidos"
- 📊 "top 50 usuários que mais cancelam"
- 🏪 "top 100 lojas com mais ajustes de estoque"

## ⚠️ **Limitações Atuais do Agente**

O agente atual é **excelente** para análises básicas, mas **NÃO possui** as seguintes funcionalidades avançadas:

### ❌ **Funcionalidades NÃO disponíveis:**
- Análise de correlação entre variáveis
- Análise temporal avançada (dias da semana, horários)
- Análise de risco e anomalias
- Análise financeira (impacto de valores)
- Detecção de padrões suspeitos
- Análise de tendências e sazonalidade
- Machine Learning para classificação

### ✅ **O que funciona perfeitamente:**
- Rankings simples (top N)
- Contagens por data específica
- Contagens por período
- Consultas básicas de coleções
- Detecção de fraude (algoritmos implementados)
- Formatação em tabelas

**💡 Dica:** Use as perguntas listadas acima para obter os melhores resultados!

## 📁 Estrutura do projeto

```
projeto_agente_ia/
├── main.py                    # Arquivo principal da aplicação
├── requirements.txt           # Lista de dependências
├── README.md                  # Documentação principal
├── DETECCAO_FRAUDE.md         # Documentação do sistema de fraude
├── DOCUMENTACAO_TECNICA.md    # Documentação técnica detalhada
├── backend/                   # Código do servidor
│   └── app/
│       ├── agents/           # Assistente de IA
│       │   └── mongodb_agent.py  # Agente principal com IA
│       ├── database/         # Configuração do banco
│       │   └── db_config.py  # Configurações do MongoDB
│       ├── modules/          # Funcionalidades principais
│       │   ├── detector_fraude.py  # Sistema de detecção de fraude
│       │   ├── importar_csv.py     # Importação de dados CSV
│       │   └── historico_conversas.py  # Sistema de histórico
│       └── utils/            # Ferramentas auxiliares
│           └── utils.py      # Utilitários gerais
└── frontend/                 # Interface web
    ├── templates/            # Páginas HTML
    │   └── index.html        # Página principal
    └── static/               # Estilos CSS
```

## 🔧 Resolvendo problemas comuns

### ❌ Erro: "MongoDB não está rodando"

**✅ Solução:** Inicie o MongoDB:

- Windows: `net start MongoDB`
- Linux/Mac: `sudo systemctl start mongod`

### 🔑 Erro: "Chave da OpenAI inválida"

**✅ Solução:**

1. Verifique se a chave está correta no arquivo `.env`
2. Confirme se você tem créditos na conta OpenAI

### 📦 Erro: "Dependências não encontradas"

**✅ Solução:** Reinstale as dependências:

```bash
pip install -r requirements.txt --force-reinstall
```

### 🌐 Erro: "Porta 5000 já está em uso"

**✅ Solução:**

1. Feche outros programas que possam estar usando a porta 5000
2. Ou mude a porta no arquivo `main.py`

## 🚨 Sistema de Detecção de Fraude

O sistema inclui algoritmos avançados para detectar possíveis fraudes nos dados:

### 🔍 Tipos de fraude detectados:

1. **Volume anômalo de devoluções**: Identifica produtos com devoluções acima do normal
2. **Movimentações suspeitas em curto intervalo**: Detecta movimentações suspeitas em curto espaço de tempo
3. **Cliente reincidente em trocas/divergências**: Identifica clientes com histórico de problemas
4. **Produto reincidente em trocas/divergências**: Detecta produtos com padrões suspeitos recorrentes

### 📊 Relatórios de fraude:

- **Níveis de risco**: ALTO e MÉDIO
- **Resumo executivo** com estatísticas detalhadas
- **Formatação HTML rica** com cores e tabelas organizadas
- **Detalhes completos** de cada suspeita encontrada
- **Download Excel** para análise posterior

### 💡 Como usar:

Simplesmente digite no chat:

- "faça uma analise de fraude"
- "relatorio de fraude"
- "análise de fraude"
- "detectar fraude"

O sistema detecta automaticamente quando você menciona fraude e executa a análise completa em todas as coleções disponíveis.

## 🛠️ Tecnologias utilizadas

- 🐍 **Python**: Linguagem principal
- 🌐 **Flask**: Framework para criar a interface web
- 🍃 **MongoDB**: Banco de dados para armazenar os dados
- 🤖 **OpenAI**: API para o assistente de IA
- 📊 **Pandas**: Para processar arquivos CSV
- 🎨 **Bootstrap**: Para o design da interface
- 🚨 **Algoritmos de Detecção**: Para análise de fraude
- 🔍 **LangChain**: Framework para integração com IA
- 📈 **FAISS**: Para busca vetorial e similaridade
- 📋 **OpenPyXL**: Para geração de relatórios Excel
