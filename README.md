# desafio-star-schema-professor-dio
# Desafio DIO: Modelagem Dimensional em Star Schema (Foco em Professores)

## 📌 Descrição do Projeto
Este projeto consiste na conversão de um modelo relacional de uma Universidade para um modelo dimensional em **Star Schema (Esquema em Estrela)** focado na análise do contexto dos **Professores**.

## 🎯 Objetivos e Premissas
- Estruturar o modelo multidimensional centrado no objeto de análise: **Professor**.
- Eliminar entidades fora do escopo do desafio (Alunos e Matrículas).
- Criar a **Tabela Fato** (`fato_ministracao`) e as **Tabelas Dimensão** (`dim_professor`, `dim_departamento`, `dim_disciplina`, `dim_curso` e `dim_data`).
- Inserir a dimensão de datas para permitir a análise temporal das ofertas de disciplinas e cursos.

## 📐 Estrutura do Modelo Dimensional (Star Schema)

![Diagrama Star Schema](Diagrama)

### Tabela Fato
- `fato_ministracao`: Reúne as chaves substitutas (*Surrogate Keys*) e as métricas `carga_horaria`, `qtd_disciplinas`, `qtd_prerequisitos` e a flag `is_coordenador`.

### Tabelas Dimensão
- `dim_professor`: Atributos cadastrais e titulação do corpo docente.
- `dim_departamento`: Informações do departamento, campus e coordenação.
- `dim_disciplina`: Nome e carga horária das disciplinas.
- `dim_curso`: Nome e modalidade dos cursos.
- `dim_data`: Calendário com granularidade temporal (mês, nome do mês, semestre, trimestre, etc.).

## 🛠️ Ferramentas Utilizadas
- **Excel / Power Query** para tratamento e estruturação dos dados.
- **Power BI** para criação dos relacionamentos e construção do esquema em estrela.
