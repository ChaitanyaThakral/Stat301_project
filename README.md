# STAT 301 Group Project
# Airbnb Price Analysis – Budapest 

This project analyzes Airbnb listings in Budapest to understand how rental attributes influence listing prices. The project was completed as part of **STAT 301** at the University of British Columbia.

---

## 📄 Project Overview

Airbnb has become a major part of the short-term rental market in European cities. Understanding what drives rental prices can help hosts optimize listings and provide insights into rental market dynamics. This project focuses on examining how key listing features affect Airbnb prices in Budapest.

**Research Question:**  
*How are Airbnb listing prices associated with rental attributes such as bedrooms, room type, guest capacity, and attraction index?*

---

## 🛠 Technologies

- **Programming Language:** R  
- **Libraries:** tidyverse, ggplot2, broom, car, knitr  
- **Tools:** RStudio, Git, GitHub  

---

## 📊 Data

**Source:**  
- [Kaggle – Airbnb Prices in European Cities](https://www.kaggle.com/datasets/thedevastator/airbnb-prices-in-european-cities)  
- Data was collected via web scraping Airbnb listings 4–6 weeks in advance.

**Dataset Description:**  
- `realSum`: Listing price in EUR  
- `room_type`: Entire home/apt, Private room, Shared room  
- `bedrooms`: Number of bedrooms  
- `person_capacity`: Maximum guests allowed  
- `attr_index`: Attraction index of surrounding area  
- Other features: host superhost status, distance to city center, cleanliness rating, etc.

---

## 🔍 Methodology

1. **Data Cleaning & Wrangling**  
   - Combined weekday and weekend data into a single dataset.  
   - Handled missing values and ensured consistent column formats.

2. **Exploratory Data Analysis**  
   - Visualized price distributions by room type, bedrooms, and guest capacity.  
   - Compared trends across weekdays and weekends using boxplots and line charts.

3. **Regression Modeling**  
   - Applied simple linear regression (SLR) for individual predictors: bedrooms and attraction index.  
   - Built an additive multiple linear regression (MLR) model including: room type, bedrooms, guest capacity, and attraction index.  
   - Used log-transformed prices to handle skewed distributions.  

4. **Model Validation**  
   - Checked assumptions using Q–Q plots for normality of residuals.  
   - Verified multicollinearity using Variance Inflation Factor (VIF).  

---

## 📈 Key Findings

- Each additional bedroom increases price by approximately **11–22%**.  
- Each additional guest adds about **7%** to the price.  
- **Private rooms** are on average **33% cheaper** than entire homes/apartments.  
- **Shared rooms** are about **29% cheaper** than entire homes/apartments.  
- Entire homes consistently have higher prices, while private and shared rooms are more moderately priced.  
- Attraction index has a smaller but noticeable effect, indicating more desirable locations have higher prices.

---

## 🖼 Visualizations

- **Boxplots:** Compare prices by room type and bedrooms.  
- **Line Graphs:** Show trends of average price by guest capacity and bedroom count.  

---

## 📚 References

- Gutiérrez, J., García-Palomares, J.C., Romanillos, G., & Salas-Olmedo, M.H. (2017). *The eruption of Airbnb in tourist cities: Comparing spatial patterns of hotels and peer-to-peer accommodation in Barcelona.* Tourism Management, 62, 278–291. doi:10.1016/j.tourman.2017.05.003  
- Gyódi, K., & Nawaro, Ł. (2021). *Determinants of Airbnb prices in European cities: A spatial econometrics approach.* Tourism Management, 86, 104319.


