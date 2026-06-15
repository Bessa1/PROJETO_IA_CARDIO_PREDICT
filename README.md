# ❤️ CardioPredict

> Sistema Inteligente para Predição de Doenças Cardiovasculares utilizando Inteligência Artificial.

Projeto desenvolvido para a disciplina de **Inteligência Artificial**, com o objetivo de aplicar técnicas de Machine Learning na identificação precoce do risco de doenças cardiovasculares a partir de dados clínicos simples.

---

## 📌 Sobre o Projeto

As doenças cardiovasculares representam a principal causa de morte no mundo, sendo responsáveis por aproximadamente **17,9 milhões de óbitos anuais**, segundo a Organização Mundial da Saúde (OMS).

Diante desse cenário, o **CardioPredict** foi desenvolvido como uma ferramenta de apoio à decisão clínica, capaz de identificar pacientes com maior probabilidade de desenvolver doenças cardiovasculares utilizando algoritmos de Inteligência Artificial.

Nosso objetivo não é substituir profissionais da saúde, mas demonstrar como a IA pode auxiliar na prevenção e triagem precoce.

---

## 🎯 Objetivo

Desenvolver um sistema inteligente capaz de:

* Identificar o risco cardiovascular de pacientes;
* Comparar diferentes algoritmos de Machine Learning;
* Selecionar o modelo mais eficiente;
* Disponibilizar uma interface funcional para testes em tempo real;
* Demonstrar a aplicação prática da IA na área da saúde.

---

## 📊 Dataset

O projeto utiliza o **Cardiovascular Disease Dataset**, contendo dados anonimizados de pacientes.

### Características da base:

* 👥 70.000 pacientes;
* 📋 14 variáveis clínicas;
* 🎯 Variável alvo binária:

  * 0 → Ausência de doença cardiovascular;
  * 1 → Presença de doença cardiovascular.

### Variáveis utilizadas

* Idade;
* Sexo;
* Pressão arterial;
* Colesterol;
* Glicose;
* Peso;
* Altura;
* Tabagismo;
* Consumo de álcool;
* Atividade física;
* IMC (feature derivada).

---

## ⚙️ Pipeline do Projeto

O desenvolvimento seguiu um fluxo completo de Machine Learning:

```text
Dados Clínicos
     ↓
Pré-processamento
     ↓
Engenharia de Features
     ↓
Treinamento dos Modelos
     ↓
Avaliação e Validação
     ↓
Integração com Front-end
     ↓
Sistema Funcional
```

---

## 🔬 Pré-processamento e Engenharia de Features

As principais etapas realizadas foram:

* Conversão da idade de dias para anos;
* Cálculo do Índice de Massa Corporal (IMC);
* Padronização dos atributos numéricos;
* Seleção das variáveis mais relevantes;
* Divisão estratificada entre treino e teste;
* Validação cruzada (K-Fold).

---

## 🤖 Modelos Avaliados

Foram implementados e comparados dois algoritmos:

### 🔵 Regressão Logística

Modelo baseline com alta interpretabilidade.

**Resultados:**

* Acurácia: 83,58%
* F1-Score: 0,8512
* AUC-ROC: 0,9176
* Cross Validation: 0,8525 ± 0,0021

---

### 🌲 Random Forest

Modelo selecionado como solução final devido ao seu desempenho superior.

**Resultados:**

* Acurácia: 93,09%
* F1-Score: 0,9371
* AUC-ROC: 0,9873
* Cross Validation: 0,9431 ± 0,0007

---

## 🏆 Melhor Modelo

O **Random Forest** foi escolhido como modelo final por apresentar maior precisão, estabilidade e capacidade de generalização.

---

## 🖥️ Aplicação Desenvolvida

Além da etapa analítica, o projeto foi expandido para uma aplicação funcional utilizando **Streamlit**.

### Funcionalidades:

* Inserção manual dos dados do paciente;
* Predição em tempo real;
* Comparação entre modelos;
* Visualização das métricas;
* Dashboard interativo;
* Demonstração prática durante a apresentação.

Esse diferencial permitiu transformar um modelo acadêmico em uma ferramenta próxima de um cenário real de utilização.

---

## 🛠️ Tecnologias Utilizadas

### Linguagem

* Python 3

### Bibliotecas

* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn

### Ferramentas

* Google Collab
* Git
* GitHub

---

## 🚀 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/cardiopredict.git
```

### 2. Acesse a pasta

```bash
cd cardiopredict
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Execute a aplicação

```bash
run app.py
```

---

## ⚖️ Considerações Éticas

O CardioPredict foi desenvolvido exclusivamente para fins acadêmicos.

Alguns pontos importantes incluem:

* O modelo não substitui profissionais da saúde;
* O dataset pode conter vieses de representação;
* É necessária validação externa antes de qualquer aplicação clínica;
* A decisão final deve permanecer sob responsabilidade humana.

> "A Inteligência Artificial deve apoiar o profissional da saúde, nunca substituí-lo."

---

## 👥 Integrantes

* Arthur Ferreira Costa, 1252222116
* Carlos Eduardo Bessa, 125221103864
* Guilherme Pereira de Albuquerque, 12522221460
* Rayssa Lima dos Santos, 125221110762

---

## 🎓 Informações Acadêmicas

**Disciplina:** Inteligência Artificial

**Universidade:** UAM – Universidade Anhembi Morumbi

**Ano:** 2026

---

## 📄 Licença

Este projeto foi desenvolvido exclusivamente para fins educacionais e acadêmicos.
