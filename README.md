**nome : Luiz Augusto Bello**

**matrícula: 202010242**

# Introdução

Esse relatório é complementar à Atividade Prática 06, realizada dia 28 de Outubro em sala de aula. O relatório possui o intuito de representar como um relatório de dados formal deve ser estruturado, juntamento com as operações de processamento de dados e códigos no R.

**Dataset: [Disease Risk from Daily Habits](https://www.kaggle.com/datasets/mahdimashayekhi/disease-risk-from-daily-habits)**

------------------------------------------------------------------------

## Resumo do Dataset

Este conjunto de dados contém informações sobre o perfil de saúde e estilo de vida de **100.000 indivíduos**. É composto por **40 colunas de características (features)** e uma coluna alvo, totalizando 41 colunas.

A estrutura do dataset inclui uma mistura de dados **numéricos** (como idade e IMC), **categóricos** (como gênero e tipo de dieta) e **ordinais** (como nível de estresse).

------------------------------------------------------------------------

**Classificação: A Coluna `target`**

A coluna principal para análise é a `target`, que realiza uma **classificação binária**. Ela indica se um indivíduo foi diagnosticado com uma determinada doença não especificada.

-   **healthy**: O indivíduo é considerado saudável.
-   **diseased**: O indivíduo é considerado doente.

O dataset é **desbalanceado**, com aproximadamente **70%** dos registros classificados como `healthy` e **30%** como `diseased`.

------------------------------------------------------------------------

### Colunas Numéricas Principais

Estas colunas contêm medições quantitativas sobre a saúde e os hábitos do indivíduo.

| Característica | Descrição |
|:-------------------------|:---------------------------------------------|
| **age** | Idade do indivíduo. |
| **bmi** | Índice de Massa Corporal (IMC). |
| **blood_pressure** | Pressão arterial sistólica (em mm Hg). |
| **cholesterol** | Nível de colesterol (em mg/dL). |
| **heart_rate** | Frequência cardíaca de repouso (em bpm). |
| **glucose** | Nível de glicose no sangue. |
| **insulin** | Nível de insulina no sangue. |
| **calorie_intake** | Consumo médio diário de calorias. |
| **sugar_intake** | Consumo diário de açúcar (em gramas). |
| **screen_time** | Tempo diário de tela (em horas). |
| **stress_level** | Nível de estresse autorreportado (escala de 0 a 10). |
| **mental_health_score** | Pontuação de bem-estar mental autorreportada (escala de 0 a 10). |

### Colunas Categóricas Principais

Estas colunas descrevem características qualitativas e hábitos de vida.

| Característica | Descrição |
|:-------------------------|:---------------------------------------------|
| **gender** | Gênero (Masculino / Feminino). |
| **diet_type** | Tipo de dieta seguida (ex: Vegana, Onívora). |
| **occupation** | Tipo de emprego ou status de ocupação. |
| **sleep_quality** | Qualidade subjetiva do sono. |
| **mental_health_support** | Se o indivíduo tem acesso a recursos de saúde mental. |
| **exercise_type** | Tipo de exercício praticado (Nenhum, Cardio, Força, Misto). |
| **healthcare_access** | Facilidade de acesso a cuidados de saúde. |
| **insurance** | Se possui ou não seguro de saúde. |
| **family_history** | Histórico familiar de doenças. |
| **caffeine_intake** | Nível de consumo de cafeína. |

------------------------------------------------------------------------