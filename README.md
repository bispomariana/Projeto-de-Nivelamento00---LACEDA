# ⚖️ Desafio de Nivelamento LACEDA 2026 - Eixo de Ciência e Engenharia de Dados

Bem-vindo(a) ao projeto de nivelamento da LACEDA! Este desafio foi desenhado para consolidar seus conhecimentos em manipulação, limpeza, análise exploratória e geração de insights.

⏱️ **Prazo de Entrega:** 17/07

---

## 📊 O Desafio
Você recebeu um conjunto de dados do departamento de Recursos Humanos de um grande escritório de advocacia (`dados/funcionaris.csv`). 

Sua missão é atuar como Cientista/Engenheiro(a) de Dados para **identificar os principais fatores que estão levando ao desligamento (evasão) dos colaboradores** e apresentar suas conclusões em forma de insights e dashboards.

### 📥 O que a Liga está fornecendo:
1. Conjunto de dados dos Funcionários (`dados\funcionarios.csv`).
2. Conjunto de dados dos Departamentos (`dados/departamentos.csv`).
3. Conjunto de dados das Filiais (`dados/filiais.csv`).

---

### 📁 Dicionário de Dados (Metadados)

Para guiar sua análise e seus tratamentos, abaixo está a descrição de cada tabela e o significado de suas respectivas colunas:

#### 1. Tabela: `funcionarios.csv`
*   **id_colaborador:** Identificador único e numérico de cada funcionário.
*   **nome:** Nome completo do colaborador.
*   **genero:** Identidade de gênero declarada pelo profissional.
*   **nivel:** Nível de senioridade no escritório (Júnior, Pleno, Sênior, Sócio).
*   **data_admissao:** Data em que o colaborador foi contratado pelo escritório.
*   **data_promocao:** Data da última promoção do colaborador (pode estar vazia caso ele nunca tenha sido promovido).
*   **salario_base:** Salário bruto mensal contratual do funcionário.
*   **percentual_bonus:** Porcentagem do salário anual que o colaborador recebe como bônus por performance.
*   **id_departamento:** Código identificador do departamento onde o colaborador atua (Chave Estrangeira).
*   **id_filial:** Código identificador da filial física onde o colaborador está alocado (Chave Estrangeira).
*   **id_reporta_a:** ID do gestor/líder direto a quem esse funcionário responde (Auto-relacionamento). Sócios não possuem gestores diretos.
*   **processos_actifs:** Volume de processos jurídicos sob a responsabilidade direta deste advogado no último trimestre.
*   **horas_extras_mes:** Média de horas extras computadas e prestadas pelo colaborador no último mês.
*   **score_satisfacao:** Nota de 1.0 a 5.0 atribuída pelo funcionário na pesquisa interna e anônima de clima organizacional.
*   **home_office:** Campo indicador se o colaborador trabalha em regime 100% remoto.
*   **status_atual:** Situação do contrato do colaborador no escritório (Ativo ou Desligado).

#### 2. Tabela: `departamentos.csv`
*   **id_departamento:** Código identificador único do setor jurídico (Chave Primária).
*   **nome_departamento:** Nome da especialidade/área (Civil, Trabalhista, Corporativo, Tributário).
*   **id_chefe_departamento:** ID do Sócio responsável pela gestão nacional daquela área.

#### 3. Tabela: `filiais.csv`
*   **id_filial:** Código identificador único da unidade física do escritório (Chave Primária).
*   **cidade:** Cidade onde a filial está localizada.
*   **estado:** Unidade Federativa (UF) da filial.
*   **id_socio_diretor:** ID do Sócio regional que lidera a operação daquela filial específica.

> ⚠️ **Atenção:** Os dados extraídos dos sistemas internos do escritório podem conter ruídos, falhas de digitação, omissões ou problemas de formatação. Parte fundamental da sua avaliação será identificar, limpar e padronizar essas inconsistências antes de iniciar a sua análise estatística.

---

### 📤 O que você deve entregar:
Para concluir o nivelamento, você deve commitar neste repositório (via Pull Request ou em sua branch de entrega):
- [ ] **Notebook (.ipynb):** Contendo todo o código de tratamento, análise exploratória e estatística.
- [ ] **Documentação/Relatório:** Explicando as premissas adotadas e a conclusão final.
- [ ] **Dashboards / Visualizações:** Gráficos claros que facilitem a tomada de decisão.
- [ ] *(Opcional)* Modelo preditivo, análise estatística avançada ou dados complementares.

---

## ⚙️ Como Participar e Entregar
1. Faça um **Fork** deste repositório para a sua conta pessoal.
2. Crie uma branch com o seu nome: `git checkout -b nome-sobrenome`.
3. Desenvolva seu projeto na pasta raiz ou em uma pasta própria com seu nome.
4. Ao finalizar, abra um **Pull Request** para o repositório principal da LACEDA.

## 📒Materiais de Apoio:
1. https://www.youtube.com/watch?v=Z_SPrzlT4Fc&list=PLucm8g_ezqNoAkYKXN_zWupyH6hQCAwxY
2. https://www.youtube.com/watch?v=NCG9niOlm40&list=PLHz_AreHm4dkBs-795Dsgvau_ekxg8g1r&index=7
3. https://www.youtube.com/watch?v=Dnt4H_WCrWE&list=PLbIBj8vQhvm2WT-pjGS5x7zUzmh4VgvRk&index=11

*Nota: A segunda parte da avaliação consistirá em uma entrevista com banco de perguntas conceituais sorteadas e a apresentação do seu projeto.*
