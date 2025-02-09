# Azure OpenAI - Desenvolvimento de Aplicações com IA

## 📌 Descrição
Este repositório contém exemplos e aplicações práticas utilizando o **Azure OpenAI**, incluindo chamadas de API e integração com o **Semantic Kernel** para criar soluções inteligentes baseadas em IA.

---

## 📖 Sobre o Azure OpenAI
O **Azure OpenAI** oferece acesso aos modelos de IA da OpenAI, como **GPT-4**, **GPT-3.5**, **Codex** e **DALL·E**, hospedados na infraestrutura segura e escalável da **Microsoft Azure**. É possível criar aplicações inteligentes que entendem e geram linguagem natural, automatizam tarefas e otimizam processos empresariais.

### 🔹 Principais Recursos:
✅ **Geração de Texto** – Criação de conteúdos automatizados, assistentes virtuais e resumos.  
✅ **Análise de Linguagem Natural** – Compreensão e extração de insights de textos.  
✅ **Tradução e Reformulação de Texto** – Melhorias automáticas na escrita e tradução entre idiomas.  
✅ **Geração de Código com Codex** – Assistência na escrita de código para diversas linguagens de programação.  
✅ **Criação de Imagens com DALL·E** – Geração de imagens baseada em descrições textuais.  
✅ **Integração com Semantic Kernel** – Uso de IA para criar fluxos de trabalho dinâmicos e personalizados.

---

## 🚀 Desenvolvimento de Aplicações
Este repositório explora como **utilizar o Azure OpenAI na prática**, com exemplos que incluem:

🔹 **Chamadas de API** – Como interagir com os modelos do Azure OpenAI usando REST APIs.  
🔹 **Uso do SDK da Azure** – Implementação de chamadas via Python e outras linguagens.  
🔹 **Integração com Semantic Kernel** – Construção de aplicações dinâmicas que combinam IA com fluxos de trabalho personalizados.  
🔹 **Casos de Uso Práticos** – Aplicações em chatbots, assistentes virtuais, automação de atendimento e análise de sentimentos.  

---

## 🌐 Uso da API do Azure OpenAI
O **Azure OpenAI API** permite que os desenvolvedores interajam diretamente com os modelos de IA por meio de chamadas REST. Com isso, é possível integrar inteligência artificial em diversas aplicações de forma flexível e escalável.

### 🔹 Exemplo de Chamada de API em Python
```python
import openai

openai.api_type = "azure"
openai.api_base = "https://seu-endpoint.openai.azure.com/"
openai.api_key = "sua-chave-aqui"
openai.api_version = "2023-06-01-preview"

response = openai.ChatCompletion.create(
    engine="gpt-4",
    messages=[{"role": "user", "content": "Olá, como você está?"}]
)

print(response["choices"][0]["message"]["content"])
```

Essa API pode ser usada para diversas finalidades, incluindo automatização de processos, análise de textos e geração de conteúdo.

---

## 🤖 Integração com Semantic Kernel
O **Semantic Kernel** é um SDK que permite a criação de **aplicações baseadas em IA**, combinando modelos do OpenAI com fluxos de trabalho personalizados e integração com sistemas empresariais.

### 🔹 Recursos do Semantic Kernel:
✅ **Memória Contextual** – Gerencia e armazena informações ao longo do tempo.  
✅ **Orquestração de Tarefas** – Permite a execução de fluxos complexos utilizando IA.  
✅ **Extensibilidade** – Integração fácil com outros serviços da Azure e OpenAI.  

### 🔹 Exemplo de Uso no Semantic Kernel
```python
from semantic_kernel import Kernel

kernel = Kernel()
kernel.add_openai_chat_completion(
    model_name="gpt-4",
    api_key="sua-chave-aqui",
    api_base="https://seu-endpoint.openai.azure.com/"
)

response = kernel.run("Explique a importância do Azure OpenAI em poucas palavras.")
print(response)
```

O Semantic Kernel possibilita a criação de **soluções de IA altamente interativas e contextuais**, permitindo maior personalização e controlo sobre a experiência do utilizador.
