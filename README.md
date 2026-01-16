🤖 AutoClassify AI - Triagem Inteligente de E-mails

Um sistema de inteligência artificial moderno para o setor financeiro, capaz de classificar e-mails, analisar arquivos e gerar respostas automáticas com base na intenção do cliente.

🏗️ Arquitetura Front-end

Interface: Construída com HTML5 e CSS3 Moderno (Responsivo).

Lógica de UI: JavaScript Vanilla (Fetch API para comunicação assíncrona).

Componentes: Sistema de cards para histórico e feedback visual de análise.

Ícones: Font Awesome / Lucide Icons.

📱 Responsividade
O sistema foi totalmente adaptado para oferecer uma experiência otimizada:

📱 Dispositivos móveis (< 768px)
Layout em coluna única para facilitar a leitura.

Inputs de texto adaptados para teclado mobile.

Menu de histórico colapsável.

🖥️ Área de trabalho (> 1024px)
Layout em duas colunas: Histórico lateral e Painel de Análise central.

Aproveitamento máximo da largura para visualização de grandes textos.

Backend (FastAPI)

Framework: FastAPI (Python 3.10) para alta performance.

IA & ML: * Scikit-Learn: Para classificação de texto (Produtivo vs Improdutivo).

Hugging Face (Flan-T5): Para geração de linguagem natural.

NLTK: Processamento de linguagem natural e limpeza de texto em Português.

Processamento de Arquivos: Integração com PyPDF2 para leitura de anexos.

Endpoints Principais:

/api/classify: Recebe texto ou arquivo e retorna a análise completa.

/: Rota raiz que serve a interface do usuário.

Segurança & Infraestrutura
Containerização: Docker (Unificação de Front e Back).

Sanitização: Limpeza de Regex para evitar inputs maliciosos.

CORS: Configuração de middleware para segurança nas requisições.

🔗 Ver Projeto no Render

📸 Demonstração do Projeto
Interface Principal:

<img width="938" height="926" alt="image" src="https://github.com/user-attachments/assets/f223c4f0-496b-473e-b3fb-98e38bf89134" />
<img width="919" height="738" alt="image" src="https://github.com/user-attachments/assets/1d798d8f-09d4-40b5-b6c9-bd150c3330e6" />

🚀 Funcionalidades

📋 Implementadas

✅ Classificação automática (Produtivo/Improdutivo).

✅ Detecção de Intenção (Suporte, Financeiro, Comercial).

✅ Sugestão de Resposta em Português via IA Generativa.

✅ Upload e leitura automática de arquivos PDF e TXT.

✅ Histórico local de análises (LocalStorage).

✅ Interface 100% responsiva (Mobile-First).

💾 Futuras

📊 Dashboard estatístico de volumetria de e-mails.

📧 Integração direta via IMAP/Gmail API.

👥 Painel administrativo para ajuste de pesos do modelo.

🛠 Tecnologias Utilizadas

Linguagem: Python 3.10

Framework: FastAPI

IA/ML: Scikit-Learn, Transformers (Hugging Face)

NLP: NLTK

Interface: JS Vanilla, CSS Grid/Flexbox

Deployment: Docker, Render

🗄️ Estrutura da Lógica de IA

Modelo de Classificação

Tipo: TF-IDF Vectorizer + MultinomialNB.

Classes: Suporte, Financeiro, Comercial, Improdutivo.

Geração de Resposta

Modelo: Flan-T5 com Prompt Engineering em Português.

🚀 Como Executar

1. Clonar o repositório
Bash

git clone https://github.com/Isaac-A-Rocha/email-classifier.git
2. Executar via Docker (Recomendado)
Bash

docker build -t email-classifier .
docker run -p 8000:8000 email-classifier
3. Executar Manualmente (Desenvolvimento)
Bash

# Backend

cd backend
pip install -r ../requirements.txt
uvicorn main:app --reload

👨‍💻 Autor:
Isaac Alves Rocha - Desenvolvedor do Projeto
