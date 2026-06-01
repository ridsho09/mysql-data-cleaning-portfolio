# SQL Data Cleaning Project – World Layoffs Dataset

## Project Overview

This project focuses on cleaning and preparing a dataset of layoffs using MySQL.

The dataset contains information on company layoffs across different industries and countries.

The main objective was to clean messy data and prepare it for exploratory data analysis.

Dataset source:
https://www.kaggle.com/datasets/swaptr/layoffs-2022

---

## Tools Used

- MySQL
- GitHub
- Kaggle Dataset

---

## Data Cleaning Steps

### 1. Created Staging Table

A staging table was created to preserve the raw dataset before cleaning.

```sql
CREATE TABLE layoffs_staging LIKE layoffs;
INSERT layoffs_staging
SELECT * FROM layoffs;
