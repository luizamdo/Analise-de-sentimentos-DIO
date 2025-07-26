# 🚀 Projeto: Análise de Sentimentos com Imagens e Texto no Azure

## 🌟 Desafio DIO - Curso de IA Generativa

---

## 🎯 Objetivo

Criar uma aplicação que analisa **sentimentos em textos** e **emoções faciais em imagens**, utilizando serviços do **Microsoft Azure**.

---

## 📊 Arquitetura

```
Usuário -> Interface Web -> Azure Functions
               |                    |
           Upload              Azure Cognitive Services:
      Texto + Imagem  -->   Text Analytics + Face API
                                     |
                          Visualização (Power BI / Streamlit)
```

---

## 🚧 Recursos Utilizados (Azure)

| Recurso                   | Finalidade                                 |
| ------------------------- | ------------------------------------------ |
| **Cognitive Services**    | Text Analytics: sentimento em texto        |
|                           |

---

## 📚 Etapas do Projeto

### 1. Criação dos Recursos no Azure

* Criar grupo de recursos: `rg-sentimentos-dio`
* Criar Cognitive Services: ativar Face API e Text Analytics
* Criar Azure Function App: para execução do backend

---

### 2. Azure Function (Backend)

Função em Python para:

* Detectar sentimentos em texto (positivo, neutro, negativo)
* Detectar emoções faciais (alegria, tristeza, raiva, etc.)

---


### 3. Visualização dos Resultados

* Exibir resultados em **Streamlit**
* Alternativa: criar dashboard em **Power BI** conectado ao Blob ou CosmosDB

---

## 📅 Exemplo de Uso

* Upload do texto: "Hoje estou me sentindo muito bem."
* Upload da imagem com rosto
* Resultado:

  * Sentimento textual: `positivo`
  * Emoção facial: `alegria`

---

## 📁 Estrutura do Projeto

```
/sentimentos_dio/
├── app/                  # Frontend com Streamlit
│   └── app.py
├── backend/              # Funções do Azure
│   └── analyze.py
├── images/               # Imagens de exemplo
├── requirements.txt      # Dependências Python
└── README.md             # Instruções do projeto
```

---

## 📷 Exemplo de Imagem de Rosto

Use imagens como esta para testar a detecção facial:

![Rosto feliz](https://learn.microsoft.com/en-us/azure/cognitive-services/face/media/face-detection-sample.jpg)

---

## ✅ Entrega para o Desafio DIO

* [ ] App funcional com upload de texto/imagem
* [ ] Azure Functions com lógica de sentimento/emocão
* [ ] Prints ou dashboard com resultados
* [ ] Código publicado no GitHub
* [ ] README completo com instruções

---

**Feito com ❤️ Luizamdo**
