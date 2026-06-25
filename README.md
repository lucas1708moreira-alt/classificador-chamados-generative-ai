# **Case QuantumFinance: Classificador de Chamados com Generative AI**

Este projeto foi desenvolvido como parte integrante da disciplina de Generative AI do MBA em Data Science e IA na FIAP. O objetivo é implementar e comparar diferentes abordagens para classificação de chamados financeiros, utilizando desde técnicas avançadas de Prompt Engineering até arquiteturas de Retrieval-Augmented Generation (RAG).

## Sobre o Projeto
O sistema visa otimizar a triagem de tickets de suporte da QuantumFinance, uma instituição financeira digital, categorizando automaticamente reclamações baseadas em texto livre. O desenvolvimento explora como modelos de linguagem de grande escala (LLMs) podem substituir ou complementar pipelines de NLP tradicionais.

## 🛠 Abordagens Exploradas
O notebook percorre uma jornada técnica de complexidade crescente:

* **Prompt Engineering**: Comparativo entre Zero-Shot, Few-Shot e Chain-of-Thought (CoT) para orientar a tomada de decisão do modelo (Claude 3.5 Haiku).

* **RAG (Retrieval-Augmented Generation)**: Implementação de uma base vetorial utilizando FAISS e embeddings via TF-IDF + SVD (LSA), garantindo recuperação semântica eficiente sem dependências complexas.

* **Modelo Campeão**: Combinação de RAG + CoT, que demonstrou a melhor performance em métricas de F1 Score.

* **Fine-Tuning (Extra)**: Estruturação de pipeline para ajuste fino (fine-tuning) supervisionado com GPT-3.5 Turbo.

## 📊 Resultados Principais
O pipeline RAG + CoT destacou-se pela capacidade de combinar contexto dinâmico recuperado da base de treinamento com o raciocínio estruturado do LLM, oferecendo um sistema auditável e de fácil manutenção para novas categorias.

## ⚙️ Tecnologias
* **Linguagem**: Python 3
* **LLM API**: Anthropic Claude (via SDK oficial)
* **Vetorial/Busca**: FAISS, Scikit-Learn
* **Processamento**: Pandas, NumPy
* **Visualização**: Seaborn, Matplotlib

---
*Referência ao notebook: "Trabalho_QuantumFinance_Generative_AI.ipynb"*[cite: 1]
