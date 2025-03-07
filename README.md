# Chatbot de Atendimento para Drone Fictício

Este projeto consiste em um chatbot baseado em LLM (Large Language Model) para atendimento ao cliente de uma marca fictícia de drones. O assistente virtual é capaz de responder perguntas sobre manuais, garantias, especificações técnicas e assistências técnicas. Caso o mesmo não seja capaz de responder a pergunta, o chatbot retorna uma resposta genérica para direcionamento para atendimento humano.

## Tecnologias Utilizadas

- **OpenAI** - Para geração de respostas e embeddings
- **Streamlit** - Interface gráfica para o chatbot
- **FAISS** - Banco de dados vetorial para busca semântica
- **Flask** - API para consultas e gerenciamento de atendimentos

## Arquitetura do Chatbot

![Arquitetura do Chatbot](https://github.com/ThiagoJFreitas/skytrack_chatbot_LLM/blob/main/assets/arquitetura.jpg)

## Como Rodar o Projeto

### Pré-requisitos

- Python instalado (>= 3.10)

### Passo a Passo

1. Clone o repositório:

```bash
https://github.com/ThiagoJFreitas/skytrack_chatbot_LLM.git
cd skytrack_chatbot_LLM
```

2. Crie o ambiente virtual:

```bash
python -m venv venv
```

3. Ative o ambiente virtual:

- No Windows:

```bash
venv\Scripts\activate
```

- No Linux ou MacOS:

```bash
source venv/bin/activate
```

4. Instale as dependências:

```bash
pip install -r requirements.txt
```

5. Configure a chave da API OpenAI:

No arquivo `config.yaml`, adicione a sua chave da OpenAI:

```yaml
api_key:
  key: "sua_api_key"

model:
  name: "gpt-4o"
```

6. Rode o servidor Flask:

```bash
python app.py
```

7. Abra uma nova aba no terminal (com o ambiente virtual ativado) e inicie a interface do chatbot com Streamlit:

```bash
streamlit run chat.py
```

8. Acesse a interface do chatbot pelo navegador através do link que o Streamlit gerar.

---

9. Screenshots

![Interface do Chatbot](https://github.com/ThiagoJFreitas/skytrack_chatbot_LLM/blob/main/assets/demo1.jpg)
![Interface do Chatbot](https://github.com/ThiagoJFreitas/skytrack_chatbot_LLM/blob/main/assets/demo2.jpg)


---

## Contribuições

Você pode contribuir com o projeto através de pull requests. Se você deseja adicionar novas funcionalidades ou corrigir bugs, siga os passos abaixo:

1. Fork o repositório.
2. Crie uma nova branch para suas alterações.
3. Faça suas alterações e teste-os.
4. Commit suas alterações com uma mensagem de commit descritiva.
5. Crie um pull request para o repositório original.

Lembre-se de seguir as convenções de codificação e organização do projeto.

## Licença

Este projeto está sob a licença MIT.
