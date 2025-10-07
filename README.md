# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href="https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Cap 1 - Batimentos de Dados – Mapeando o Coração Moderno

## Beginner Coders

## 👨‍🎓 Integrantes:
- <a href="https://www.linkedin.com/in/luana-porto-pereira-gomes/">Luana Porto Pereira Gomes</a>
- <a href="https://www.linkedin.com/in/luma-x">Luma Oliveira</a>
- <a href="https://www.linkedin.com/in/priscilla-oliveira-023007333/">Priscilla Oliveira </a>
- <a href="https://www.linkedin.com/in/paulobernardesqs?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app">Paulo Bernardes</a>

## 👩‍🏫 Professores:
### Tutor(a)
- <a href="https://www.linkedin.com/in/leonardoorabona/">Leonardo Ruiz</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi</a>

---

## 📜 Descrição

Este projeto foi desenvolvido com o objetivo de **simular o funcionamento de um sistema inteligente de triagem médica**.  
A proposta aborda duas etapas principais:
1. **Interpretação de sintomas (IA baseada em regras)** — utilizando frases clínicas e um mapa de conhecimento.
2. **Classificação automática de risco (IA baseada em aprendizado de máquina)** — para distinguir casos de **alto risco** e **baixo risco**.

O projeto demonstra, de forma prática, como a **Inteligência Artificial pode apoiar decisões clínicas** e otimizar o atendimento em triagens médicas.

---

### 🧠 Parte 1 — Extração de Sintomas e Sugestão de Diagnóstico

Nesta etapa, o sistema:
- Lê um arquivo `.txt` contendo **relatos simulados de pacientes**;
- Analisa os textos em busca de **palavras-chave (sintomas)**;
- Cruza os sintomas com um **mapa de conhecimento médico** (`.csv`);
- Sugere o **diagnóstico mais provável**, baseado em correspondências encontradas.

📄 **Arquivos utilizados:**
- `frases-sintomas.txt` → Relatos clínicos simulados.  
- `sintomas_doencas_mapa_completo.csv` → Mapa com sintomas e doenças associadas.  
- `saida_diagnosticos.csv` → Saída gerada com sintomas e diagnósticos sugeridos.  

📊 **Exemplo de saída:**
| Paciente | Frase | Sintomas Encontrados | Diagnóstico Sugerido |
|-----------|--------|----------------------|----------------------|
| Paciente 1 | “Sinto dor no peito e falta de ar ao esforço” | Falta de ar | Endocardite |
| Paciente 2 | “Nas últimas semanas tenho sentido fraqueza e tontura” | Tontura | Hipertensão Arterial |

📸 **Figura 1 — Saída gerada pelo sistema na Parte 1 (diagnóstico baseado em sintomas)**  
*(Insira aqui a imagem do seu resultado do Colab com a tabela de saída gerada)*  

---


### 🤖 Parte 2 — Classificação de Risco com Machine Learning

Nesta etapa, foi criado um **classificador de texto** capaz de analisar frases clínicas e prever o **nível de risco do paciente**, utilizando técnicas de *Machine Learning*.

🧩 **Etapas principais:**
- Leitura do arquivo `dataset_risco.csv` com frases e rótulos (“alto risco” e “baixo risco”);
- Vetorização de texto com **TF-IDF**;
- Treinamento e teste de modelos (Regressão Logística, SVM e MultinomialNB);
- Avaliação com métricas de desempenho e **matriz de confusão**.

📈 **Melhor resultado obtido:**
- Modelo: `MultinomialNB`
- Acurácia final: **0.83**

📊 **Métricas de desempenho:**
| Classe | Precision | Recall | F1-score | Support |
|---------|------------|---------|-----------|----------|
| Alto Risco | 1.00 | 0.67 | 0.80 | 3 |
| Baixo Risco | 0.75 | 1.00 | 0.86 | 3 |
| **Acurácia** | **0.83** | **0.83** | **0.83** | 6 |

📸 **Figura 2 — Relatório de desempenho do classificador (TF-IDF + MultinomialNB)**  
*(Insira aqui a captura de tela do relatório de acurácia com as métricas do modelo)*  

---

### 🔹 Matriz de Confusão
A matriz de confusão mostra o desempenho do modelo em prever corretamente os casos de **alto risco** e **baixo risco**.

| Real \ Previsto | Alto Risco | Baixo Risco |
|------------------|-------------|--------------|
| **Alto Risco** | 2 | 1 |
| **Baixo Risco** | 0 | 3 |

📸 **Figura 3 — Matriz de Confusão: Classificação de Risco**  
*(Insira aqui o print da matriz de confusão gerada no Colab)*  

---

### Links:
[🔗 Clique aqui para assistir ao vídeo](https://youtu.be/B4OQ8L7OS84) <br>
[Acesse o notebook](https://colab.research.google.com/drive/13XjixufqLO0jlZPsGyk4uIs05JAKoBG0?usp=drive_link)



## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>assets</b>: arquivos relacionados a elementos visuais do repositório, como imagens e ícones.

- <b>data</b>: Base de dados.

- <b>notebook</b>: código python em .ipynb

- <b>README.md</b>: guia completo e explicativo sobre o projeto (este arquivo).

---

## 🗃 Histórico de lançamentos

* 0.5.0 - XX/XX/2025
* 0.4.0 - XX/XX/2025
* 0.3.0 - XX/XX/2025
* 0.2.0 - XX/XX/2025
* Estrutura inicial do projeto - 26/08/2025
