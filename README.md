ai-cad-orchestrator
Uma aplicação desktop desenvolvida em Python (tkinter) que integra o Google Gemini e a API do Meshy AI para auxiliar na criação e estruturação de modelos 3D a partir de imagens técnicas e cotas informadas pelo usuário.

🚀 Funcionalidades
Análise Visual Inteligente: Carregue uma imagem ou desenho técnico de uma peça para que o Gemini identifique o objeto e liste as dimensões necessárias (frente, topo, lateral, raios, diâmetros, espessuras).

Campos Dinâmicos com Scroll: A interface gera automaticamente campos de texto personalizados baseados nas medidas solicitadas pela IA.

Consolidação de Prompt Técnico: Combina a imagem original com as cotas numéricas preenchidas pelo usuário para criar um prompt em inglês altamente otimizado e restrito às dimensões informadas.

Integração com Meshy AI (Image-to-3D): Envia a imagem convertida em Base64 e o prompt estruturado via API para gerar o modelo tridimensional automaticamente.

🛠️ Tecnologias Utilizadas
Python 3.x

Tkinter (Interface Gráfica)

Google GenAI SDK (google-genai)

Pillow (PIL) (Processamento de Imagens)

Requests (Comunicação HTTP com a API)

⚙️ Instruções de Instalação e Uso
1. Pré-requisitos
Certifique-se de ter o Python instalado na sua máquina. Instale as bibliotecas necessárias executando o comando no seu terminal:

Bash
pip install google-genai pillow requests
2. Configuração das Chaves de API
Abra o código fonte e insira as suas chaves de API pessoais nas variáveis correspondentes no topo do script:

Python
GEMINI_API_KEY = "SUA_CHAVE_GEMINI_AQUI"
MESHY_API_KEY = "SUA_CHAVE_MESHY_AQUI"
⚠️ Aviso de Segurança: Nunca publique o seu código no GitHub contendo chaves de API válidas expostas. Utilize variáveis de ambiente se preferir manter suas credenciais seguras.

3. Executando a Aplicação
No terminal, navegue até a pasta do projeto e execute:

Bash
python nome_do_arquivo.py
