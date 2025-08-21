# Exploring NYC Public School Test Result Scores 🏫

Analyze SAT performance across New York City public schools to uncover insights on math proficiency, top-performing schools, and borough-level score variability.  
This project leverages pandas and descriptive statistics to answer real-world education questions.

---

## ❓ Guiding Questions
1. Which NYC schools have the best math results?  
   - Schools with math averages ≥ 80% of the maximum possible score (800).  

2. What are the top 10 performing schools based on the combined SAT scores?  
   - Sum of math, reading, and writing scores.  

3. Which single borough has the largest standard deviation in combined SAT score?  
   - Includes borough name, number of schools, mean SAT, and standard deviation.  

---

## 📊 The Data

### **schools.csv**
| Column          | Description |
|------------------|-------------|
| `school_name`   | Name of the school |
| `borough`       | NYC borough where the school is located |
| `building_code` | Identifier for school building |
| `average_math`  | Average SAT math score |
| `average_reading` | Average SAT reading score |
| `average_writing` | Average SAT writing score |
| `percent_tested` | Percentage of students tested |

---

## 🔎 How I Approached the Project  

### 1. Finding schools with the best math scores  
I subset the data to include only schools with math averages ≥ 640 (80% of 800) and stored them in `best_math_schools`.  

### 2. Identifying the top 10 performing schools  
I calculated total SAT scores across math, reading, and writing, then sorted results in descending order to identify the top 10 schools in a DataFrame `top_10_schools`.  

### 3. Locating the borough with the largest SAT variability  
I grouped by borough to compute number of schools, average SAT, and standard deviation of SAT. Then I filtered for the borough with the largest `std_SAT`, rounded to two decimals.  

---

## 📌 Key Deliverables
- Subset schools with strong math performance (≥ 640 average).  
- Ranked top 10 schools by combined SAT performance.  
- Identified borough with the highest score variability using mean & std calculations.  
- Strengthened **pandas** skills: filtering, aggregation, grouping, sorting, and statistical calculations.  

---

## 🛠️ Skills Used
- **Python**: pandas, numpy  
- Data wrangling & cleaning  
- Grouping & aggregation  
- Sorting and ranking  
- Descriptive statistics (mean, std)  
- Exploratory data analysis (EDA)  

