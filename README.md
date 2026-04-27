
# 🩺 Predição de Câncer do Colo do Útero: Integração de Machine Learning e Tomada de Decisão Multicritério (MCDM)

![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Área](https://img.shields.io/badge/%C3%81rea-Sa%C3%BAde%20P%C3%BAblica-blue)
![Tecnologias](https://img.shields.io/badge/Tecnologias-ML%20%7C%20MCDM-orange)

## 📌 Visão Geral
Este repositório contém a metodologia e os experimentos do meu Trabalho de Conclusão de Curso (TCC). O estudo foca no diagnóstico precoce do câncer do colo do útero — uma das neoplasias mais prevalentes na região Norte do Brasil — utilizando uma abordagem híbrida que une algoritmos de aprendizado de máquina e métodos de decisão multicritério para selecionar o modelo preditivo ideal.

## 🔬 Metodologia
A abordagem proposta seguiu um pipeline rigoroso de Data Science para lidar com a complexidade dos dados médicos:

1.  **Tratamento de Dados (SMOTETomek):** Aplicação de técnica de reamostragem híbrida para mitigar o desbalanceamento severo das classes (casos positivos vs. negativos).
2.  **Seleção de Atributos (Feature Selection):** Uso do algoritmo **Random Forest** para identificar as variáveis clínicas mais relevantes, reduzindo ruídos e dimensionalidade.
3.  **Modelagem:** Avaliação de diversos algoritmos clássicos de aprendizado supervisionado.
4.  **Seleção Multicritério (MCDM):**
    *   **AHP (Analytic Hierarchy Process):** Utilizado para a atribuição ponderada de pesos aos critérios de desempenho.
    *   **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution):** Utilizado para ranquear os modelos, considerando múltiplos indicadores simultaneamente.

## 🛠️ Tecnologias Utilizadas
*   **Linguagem:** Python
*   **Bibliotecas de ML:** `Scikit-Learn`, `Imbalanced-learn` (SMOTE)
*   **Métodos MCDM:** Implementação de cálculos matriciais para AHP e TOPSIS.
*   **Processamento de Dados:** `Pandas`, `NumPy`.

## 📈 Resultados Alcançados
Após a avaliação pelo método TOPSIS, os modelos foram ranqueados com base em sua capacidade discriminativa e eficácia geral:

| Ranking | Algoritmo | Desempenho |
| :--- | :--- | :--- |
| **1º** | **Random Forest** | **Eficácia Superior / Líder do Ranking** |
| 2º | Decision Tree | Capacidade discriminativa excepcional |

**Conclusão Técnica:** A combinação de pré-processamento robusto (SMOTETomek) com a avaliação multicritério provou ser eficaz para selecionar modelos em contextos médicos complexos, garantindo que o algoritmo escolhido seja equilibrado entre precisão, sensibilidade e outras métricas críticas.
