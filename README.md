# 🤖 SQL BOT – Rule-Based NLP to SQL Generator

## 🚀 Overview

SQL BOT is an intelligent rule-based system that converts **natural language input into dynamic SQL queries**.

It uses:
- NLP parsing
- Config-driven SQL generation
- Multi-table JOIN handling
- Dynamic WHERE clause construction

This project demonstrates how business rules can be translated into SQL using a **scalable rule engine instead of hardcoded queries**.

---

## 🎯 Key Features

✅ Natural language → SQL conversion  
✅ Dynamic JOIN resolution across multiple tables  
✅ Config-driven (`sql_generation.txt`) – no hardcoding  
✅ Supports:
- WHERE conditions
- JOIN rules
- SUBQUERY logic
- ORDER BY
- TOP (NoOfPlansReqd)

✅ Extensible architecture (just update config file)

---

## 🏗️ Architecture
User Input
↓
NLP Parser (parse_conditions / parse_user_input)
↓
Rule Engine (generate_sql)
↓
SQL Query Generation
↓
Database Execution (pyodbc)
## 📁 Project Structure


sqlbot/
│
├── app.py # Streamlit UI
├── parser/
│ ├── txt_parser.py # Rule file parser
│ ├── nlp_parser.py # NLP condition parser
│
├── services/
│ ├── rule_engine.py # SQL generation engine
│ ├── rule_loader.py # Rule loader
│
├── sql_generation.txt # Rule configuration (CORE)
├── requirements.txt
├── README.md
├── .gitignore

<img width="1814" height="965" alt="image" src="https://github.com/user-attachments/assets/c09cce82-6bdc-4573-84f4-39f942c6a4e8" />
