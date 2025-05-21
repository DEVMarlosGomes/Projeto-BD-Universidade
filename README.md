# 🎓 Projeto BD Universidade  
### 📘 Um modelo de banco de dados acadêmico completo  
**Dev: Marlos Gomes**

---

## 📌 Sobre o Projeto

Este projeto tem como objetivo modelar um sistema de banco de dados para uma universidade fictícia.  
Ele contempla **disciplinas**, **alunos**, **professores**, **prédios**, **salas**, **matrículas** e muito mais!  
Ideal para fins **educacionais**, **simulações de queries SQL** e **prática de modelagem relacional**.  

---

## 🧠 Funcionalidades

✅ Cadastro de disciplinas  
✅ Relacionamento entre disciplinas e pré-requisitos  
✅ Cadastro de alunos e professores  
✅ Estrutura física (prédios e salas)  
✅ Alocação de aulas por semestre  
✅ Matrícula de alunos em disciplinas

---

## 🛠️ Tecnologias Utilizadas

- PostgreSQL 🐘  
- SQL Puro 🧾  
- Modelo Relacional (MER/DER)  
- [DBeaver](https://dbeaver.io/) para testes e visualização

---

## 💡 Objetivo Pessoal
Este projeto faz parte do meu aprendizado contínuo em Análise e Desenvolvimento de Sistemas, onde estou consolidando conhecimentos em modelagem de dados, normalização e consultas SQL.

## 🤝 Contribuições
Sinta-se à vontade para abrir issues, sugerir melhorias ou apenas deixar um ⭐️ se gostar do projeto!

## 📬 Contato
Me acompanhe para mais projetos como esse:
# LinkedIn https://www.linkedin.com/in/marlos-gomes/

# © 2025 - Marlos Gomes 🚀

## 📊 Exemplo de Consulta

🔍 Verificar disciplinas com pré-requisitos:

```sql
SELECT 
    d1.nome_disciplina AS disciplina,
    d2.nome_disciplina AS pre_requisito
FROM 
    tbl_disciplina_prerequisito dp
JOIN 
    tbl_disciplina d1 ON dp.cod_disciplina = d1.cod_disciplina
JOIN 
    tbl_disciplina d2 ON dp.cod_prerequisito = d2.cod_disciplina; '''


