# 🍞 Кластеризация на основе плотности с помощью алгоритма DBSCAN

**Цель проекта**:  
Применить алгоритм DBSCAN для кластеризации данных.  
Изучить, как меняется поведение модели при разных параметрах `eps` и `min_samples`.

---

## 📦 Данные

**Название датасета**:  
`wholesome_customers_data.csv`

**Исходные статьи:**

Cardoso, Margarida G.M.S. (2013). Logical discriminant models â€“ Chapter 8 in Quantitative Modeling in Marketing and Management Edited by Luiz Moutinho and Kun-Huang Huarng. World Scientific. p. 223-253. ISBN 978-9814407717

Jean-Patrick Baudry, Margarida Cardoso, Gilles Celeux, Maria JosÃ© Amorim, Ana Sousa Ferreira (2012). Enhancing the selection of a model-based clustering with external qualitative variables. RESEARCH REPORT NÂ° 8124, October 2012, Project-Team SELECT. INRIA Saclay - ÃŽle-de-France, Projet select, UniversitÃ© Paris-Sud 11

**Источник данных**:     
https://archive.ics.uci.edu/ml/datasets/Wholesale+customers

**Описание**:    
Датасет содержит данные о клиентах некоторого оптового дистрибьютора. Здесь приведены денежные расходы за год по различным категориям продуктов. Каждая строка - информация об отдельном клиенте.

---

## 🧠 Этапы проекта

1. 🔍 **EDA и визуализация**:
   - Распределение точек
   - Исследование зависимостей между различными переменными
   - Исследование корреляций расходов по различным категориям 
   - Проверка шкал/масштабов признаков  
   - Использование `StandardScaler` 

2. 🧪 **Применение DBSCAN**:
   - Определение параметров `eps` и `min_samples`  
   - Использование метода локтя для подбора `eps`  
   - Визуализация результатов кластеризации
   - Вычисление средних значений расходов для каждого кластера

3. 📊 **Анализ результатов**:
   - Выделение кластеров  
   - Визуализация средних значений расходов для кластеров с помощью тепловой карты 

---

## ⚙️ Используемые технологии

- Python 3.x  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib, Seaborn 

---

## 📈 Результаты

- Выделено кластеров: `2`   
- Наилучшие параметры:
  - `eps = 2`  
  - `min_samples = 16`

---

## 📝 Выводы
 
> Параметры `eps` и `min_samples` критически влияют на чувствительность алгоритма.  
> В отличие от KMeans, DBSCAN лучше справляется с кластерами произвольной формы.

---

## 📬 Контакт

Есть идеи, вопросы или предложения? Пишите!

