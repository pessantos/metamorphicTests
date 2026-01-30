# Metamorphic Tests

Este repositório contém os **artefatos experimentais de Testes Metamórficos (Metamorphic Testing)** desenvolvidos no contexto de uma **dissertação de mestrado**, cujo objetivo é avaliar sistemas baseados em dados e modelos computacionais.

O repositório apoia a **execução, organização e análise dos experimentos**, possibilitando a reprodutibilidade dos testes e a avaliação sistemática dos resultados obtidos em diferentes níveis de complexidade.

---

## 1. Contexto científico e trabalho de base

Os experimentos realizados neste repositório derivam e estendem o trabalho disponibilizado pelo grupo de pesquisa Conect2AI, conforme o repositório e o artigo científico a seguir:

- Repositório base (sistema original):  
  https://github.com/conect2ai/MDPI2023-pollution

- Artigo científico associado:  
  https://www.mdpi.com/2071-1050/16/2/708

- Grupo de pesquisa Conect2AI:  
  https://www.instagram.com/conect2ai

---

## 2. Sistema sob Teste (SUT)

O **Sistema Sob Teste (SUT)** utilizado nos experimentos de Testes Metamórficos corresponde ao conjunto de notebooks, modelos preditivos e simulações disponibilizados no repositório base mencionado anteriormente.

Esse sistema compreende:
- Análise de dados de viagens veiculares
- Modelos preditivos para variáveis utilizadas no cálculo de emissões
- Simulações baseadas em SUMO e grafos urbanos

O SUT é utilizado como base para a definição, aplicação e avaliação das relações metamórficas investigadas na dissertação.

---

## 3. Organização dos Testes Metamórficos

Os Testes Metamórficos foram organizados em **níveis de complexidade crescente**, conforme o desenho experimental definido na dissertação, sendo implementados em notebooks Jupyter independentes:

- `Level_1_metamorphic_tests.ipynb`
- `Level_2_metamorphic_tests.ipynb`
- `Level_3_metamorphic_tests.ipynb`

Cada notebook contempla:
- A definição dos casos de teste metamórficos
- A aplicação das relações metamórficas
- A execução dos testes sobre o SUT
- A coleta e análise das métricas por caso de teste

---

## 4. Planos de Teste Metamórfico

Os **Planos de Teste Metamórfico** estão documentados na pasta `metamorphic_test_plans/` e descrevem, de forma estruturada, o planejamento dos testes executados em cada nível experimental.

Arquivos disponíveis:
- `Test_Plan_Level_1.md`
- `Test_Plan_Level_2.md`
- `Test_Plan_Level_3.md`

Cada plano de teste apresenta:
- O objetivo do nível de teste
- A caracterização das relações metamórficas aplicadas
- A estratégia de execução dos casos de teste
- O vínculo entre os testes planejados e os notebooks de execução

Esses documentos formalizam o **desenho experimental dos Testes Metamórficos**, garantindo rastreabilidade, clareza metodológica e apoio à reprodutibilidade dos experimentos descritos na dissertação.

---

## 5. Notebooks oriundos do sistema original

Os notebooks listados a seguir **não foram desenvolvidos especificamente para os Testes Metamórficos**, mas fazem parte do **sistema original sob teste**, sendo utilizados como suporte à execução dos experimentos:

- `initial_analysis.ipynb`
- `predict_maf.ipynb`
- `predict_afr.ipynb`
- `predict_co2.ipynb`
- `predict_maf_lightweight.ipynb`
- `predict_afr_lightweight.ipynb`
- `simulate_sumo.ipynb`
- `create_graph_network.ipynb`

Esses notebooks foram originalmente desenvolvidos no contexto do repositório base e são mantidos neste repositório **exclusivamente para fins de reprodução do sistema sob teste**, não constituindo artefatos de Testes Metamórficos.

A separação entre o sistema sob teste e os artefatos de teste é adotada para garantir **clareza metodológica e validade experimental**.

---

## 6. Resultados experimentais

Os resultados consolidados dos experimentos estão disponíveis na pasta `results/`, na forma de arquivos **PDF**, contendo:

- Gráficos gerados durante a execução dos testes
- Métricas obtidas por caso de teste metamórfico
- Resultados organizados por nível de teste

Arquivos disponíveis:
- `L1 - Metamorphic Test Cases.pdf`
- `L2 - Metamorphic Test Cases.pdf`
- `L3 - Metamorphic Test Cases.pdf`

---

## 7. Ambiente experimental e reprodutibilidade

As dependências e o ambiente de execução dos experimentos estão descritos nos arquivos:

- `requirements.txt`
- `environment.yml`

Esses arquivos permitem a **reprodução do ambiente experimental** adotado no desenvolvimento da dissertação.

---

## 8. Contexto acadêmico

Os materiais disponibilizados neste repositório têm como finalidade:
- Apoiar a **reprodutibilidade dos experimentos** descritos na dissertação
- Facilitar a análise comparativa entre diferentes níveis de Testes Metamórficos
- Servir como base para estudos futuros na área de **Qualidade de Software e Testes de Sistemas Baseados em Machine Learning**

Este repositório possui finalidade exclusivamente acadêmica e científica.
