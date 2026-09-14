# Projeto WoundSense: Investigação Computacional de Biomarcadores Digitais Multimodais

## 📋 Contexto do Projeto
O WoundSense é um projeto aplicado de Computação Biomédica focado na investigação de potenciais biomarcadores digitais. Utilizando imagens multimodais, o objetivo é realizar a caracterização objetiva de feridas crônicas de difícil cicatrização. O projeto utiliza a base de dados *Chronic Wounds Multimodal Image Database (WoundsDB). O intuito principal da investigação não é apenas criar um algoritmo com alto desempenho, mas compreender o percurso metodológico que transforma imagens biomédicas brutas em características quantitativas, convertendo-as em evidências potencialmente úteis para a avaliação clínica.

## 🏥 O Desafio Clínico e a Decisão em Saúde
Atualmente, a avaliação assistencial de feridas crônicas em acompanhamento ambulatorial depende fortemente da observação visual subjetiva e de medidas realizadas manualmente durante o atendimento. Essa abordagem dificulta a comparação objetiva do estado do paciente entre diferentes consultas. 

A decisão em saúde que este projeto pretende apoiar visa caracterizar objetivamente o estado da lesão para auxiliar seu monitoramento clínico contínuo. O projeto não tem a pretensão de construir um sistema autônomo de diagnóstico ou afirmar predição definitiva de cicatrização, focando em identificar características mensuráveis com plausibilidade biológica e clínica.

## 🔍 Abordagem Multimodal
Para superar as limitações da avaliação visual isolada, o projeto investiga se a combinação de diferentes modalidades de imagem fornece uma caracterização mais informativa da ferida. As características extraídas são divididas em três grandes dimensões:
*   **Características Visuais (Imagens RGB):** Capturam a aparência visual da lesão, permitindo avaliar aspectos relacionados a cor, textura, bordas e desordem estrutural da região.
*   **Características Térmicas (Termografia):** Representam a distribuição de temperatura, analisando a heterogeneidade térmica e as diferenças de calor entre a lesão e as regiões adjacentes.
*   **Características Geométricas (Profundidade/3D):** Mapeiam a geometria tridimensional através de estereovisão e sensores de profundidade, extraindo medidas estruturais como área, perímetro, formato e profundidade.

## 🚀 Pipeline de Investigação
A arquitetura do projeto foi estruturada em três fases de desenvolvimento para garantir a robustez científica dos biomarcadores:

1.  **Dos Dados Clínicos aos Biomarcadores Candidatos:** Exploração dos dados disponíveis, revisão da literatura científica e formulação de hipóteses sobre o que pode ser medido nas imagens para representar o estado da ferida.
2.  **Da Extração à Evidência Computacional:** Operacionalização dos candidatos por meio de extração de variáveis quantitativas. Esta etapa envolve análises estatísticas e modelagem computacional para investigar relações entre as características.
3.  **Validação e Interpretação:** Medição da robustez das evidências computacionais geradas, considerando a variabilidade entre imagens e a prevenção de *data leakage*. Envolve o confronto dos resultados com a literatura e a avaliação da plausibilidade clínica.

## 📂 Estrutura do Repositório
O desenvolvimento deste projeto foi dividido em três entregas principais, refletindo as fases da pipeline listada acima:

*   📁 **`/entrega_1/`**
    *   Contém o **relatório descritivo** e os **códigos** de exploração inicial. O foco desta etapa foi a compreensão do problema clínico, documentação (dicionário de dados), revisão da literatura e a formulação das hipóteses para os biomarcadores candidatos.
*   📁 **`/entrega_2/`**
    *   Contém o **notebook executável** e o **PDF da apresentação** dos resultados. Detalha o pré-processamento, a extração das características quantitativas (features), a aplicação de análises estatísticas e a modelagem computacional para gerar as evidências preliminares.
*   📁 **`/entrega_3/`**
    *   Contém os **códigos de validação** e o **relatório final** do projeto. Focado em avaliar a força da evidência através da validação cruzada do modelo, testes de robustez (repetibilidade das features), correção de múltiplos testes e a interpretação clínica final sobre o potencial dos biomarcadores.
