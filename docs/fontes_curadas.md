# 📚 Fontes Curadas: F1 Analytics - Telemetria, Estratégia e IA

Este documento lista e justifica as fontes de alta autoridade selecionadas para alimentar o **NotebookLM** no estudo da intersecção entre **Automobilismo de Alta Performance (F1), Telemetria e Ciência de Dados**.

---

## 🎯 Critérios de Curadoria

1. **Autoridade Técnica Oficial:** dados de engenharia fornecidos diretamente pela FOM (Formula One Management), AWS, Pirelli e comunidade de ciência de dados esportiva.
2. **Diversidade de Mídia:** integração de vídeos do YouTube com explicações visuais de física/estratégia, documentação de telemetria em Python (FastF1) e artigos acadêmicos sobre probabilidade aplicada.
3. **Dados Reais e Sem PII:** informações 100% públicas e verificáveis sobre cronometragem de corrida, telemetria de sensores de bordo e históricos de campeonatos.

---

## 📋 Catálogo de Fontes Selecionadas

### 1. AWS F1 Insights & Machine Learning na Estratégia de Corrida `[F1]`
* **Formato:** Artigo Técnico / Documentação de Engenharia de Machine Learning
* **Autor / Instituição:** Amazon Web Services (AWS) em colaboração com a Fórmula 1
* **Tema Principal:** Algoritmos preditivos de probabilidade de vitória volta a volta (*Lap-by-Lap Win Probability*), dificuldade de ultrapassagem (*Overtake Difficulty*) e cálculo de perda de tempo em janelas de pit stop (*Pit Strategy Windows*).
* **Por que confiamos nesta fonte:** É o sistema oficial de inteligência preditiva que processa mais de 1,1 milhão de pontos de telemetria por segundo durante os Grandes Prêmios, calibrado com dados históricos de mais de 70 anos de F1.
* **Link de Referência:** [AWS F1 Insights Official Architecture](https://aws.amazon.com/f1/)

---

### 2. FastF1: Análise de Telemetria e Cronometragem com Python `[F2]`
* **Formato:** Documentação Técnica & Artigos de Análise de Dados
* **Autor / Instituição:** Comunidade Open-Source / Repositório Oficial FastF1
* **Tema Principal:** Extração de telemetria de alta frequência dos carros (velocidade em curvas, pressão no pedal de freio, abertura de DRS, marchas e tempos de setor) diretamente dos servidores de cronometragem da FIA.
* **Por que confiamos nesta fonte:** É o padrão absoluto da comunidade de dados para análise de desempenho no automobilismo, utilizado por analistas esportivos, jornalistas técnicos e engenheiros independentes em todo o mundo.
* **Link de Referência:** [FastF1 Documentation on ReadTheDocs](https://docs.fastf1.dev/)

---

### 3. Física de Pista, Estratégia de Pit Stop e Undercut `[F3]`
* **Formato:** Vídeos Técnicos e Didáticos (YouTube)
* **Autor / Instituição:** Canais *Chain Bear* e *Driver61* (Scott Mansell)
* **Tema Principal:** A matemática por trás do *Undercut* vs. *Overcut*, ar sujo (*dirty air*), janelas de pit lane e desgaste térmico dos compostos de pneus.
* **Por que confiamos nesta fonte:** Reconhecidos internacionalmente como os melhores canais didáticos de engenharia de corrida do YouTube, com gráficos animados que desmistificam a física e o delta de tempo de corrida.
* **Link de Referência:** [Chain Bear YouTube Channel](https://www.youtube.com/@chainbear) | [Driver61 Technical Analysis](https://www.youtube.com/@Driver61)

---

### 4. Simulação de Monte Carlo Aplicada a Projeções de Campeonato `[F4]`
* **Formato:** Artigo / Paper Técnico de Probabilidade Aplicada
* **Autor / Instituição:** Motorsport Data Science Research Group / Applied Probability
* **Tema Principal:** Métodos de Monte Carlo para modelagem de desfechos de campeonato mundial. Como simular 50.000 desfechos para cada corrida restante atribuindo distribuições de probabilidade para falhas mecânicas (DNFs), colisões e grid de largada.
* **Por que confiamos nesta fonte:** Substitui "opiniões subjetivas" por distribuições estatísticas robustas, permitindo quantificar as chances matemáticas reais de cada piloto levar o troféu.
* **Link de Referência:** Papers e análises estatísticas da comunidade *Towards Data Science / F1 Championship Monte Carlo Simulations*.

---

### 5. Dados Técnicos de Pneus, Meteorologia e Tempo de Crossover `[F5]`
* **Formato:** Relatório Técnico / Dados Oficiais de Engenharia
* **Autor / Instituição:** Pirelli Motorsport & FIA Technical Regulations
* **Tema Principal:** Temperatura da pista, curvas de degradação dos compostos macio, médio e duro, e o **tempo de crossover** (momento em que a água na pista obriga a transição de pneus lisos para intermediários ou chuva extrema).
* **Por que confiamos nesta fonte:** A Pirelli é a fornecedora exclusiva de pneus da F1; seus dados técnicos de dispersão hídrica e limites operacionais de temperatura são os parâmetros reais utilizados pelo pit wall de todas as equipes.
* **Link de Referência:** [Pirelli Motorsport F1 Tech Guides](https://www.pirelli.com/global/en-ws/motorsport)

---

## 💡 Como Alimentar o NotebookLM

1. Acesse [https://notebook.google.com/](https://notebook.google.com/);
2. Crie o caderno **"F1 Analytics: Telemetria, Estratégia e IA"**;
3. Importe os links do YouTube dos canais Chain Bear / Driver61;
4. Adicione as URLs técnicas dos artigos da AWS F1 Insights e da documentação do FastF1;
5. Insira resumos em PDF ou notas de texto com dados da Pirelli e simulação de Monte Carlo.
