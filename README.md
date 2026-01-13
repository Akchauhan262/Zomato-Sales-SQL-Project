# Zomato-Sales-SQL-Project
![Python](https://img.shields.io/badge/Data%20Visualization-Python-blue?logo=python)
![License](https://img.shields.io/github/license/ShaikhBorhanUddin/Zomato-Data-Analysis)
![Repo Size](https://img.shields.io/github/repo-size/ShaikhBorhanUddin/Zomato-Data-Analysis)
![Git](https://img.shields.io/badge/Version%20Control-Git-orange?logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/Host-GitHub-black?logo=github)
![Project Status](https://img.shields.io/badge/Project-Completed-brightgreen?style=flat-square) 

![Dashboard](https://github.com/Akchauhan262/Zomato-Sales-SQL-Project/blob/main/Images/title.png?raw=true)
## 📌 Project Overview

The Zomato Database Analytics Project aims to conduct an in-depth exploratory data analysis and business intelligence assessment on a structured restaurant dataset sourced from Kaggle. This dataset consists of five interrelated tables. These tables capture essential information about food items, menus, customer orders, restaurant details, and user demographics. The primary objective of this project is to uncover actionable insights by addressing strategic business questions. These include identifying top-performing restaurants, understanding cuisine popularity, analyzing customer spending behavior, and revealing geographic and demographic trends. The analysis was carried out using PostgreSQL for complex queries and Python for data preprocessing and visualization.


## 📦 Dataset, Visualization & Data Cleaning

The [dataset](https://www.kaggle.com/datasets/anas123siddiqui/zomato-database) is sourced from Kaggle. The database is a comprehensive collection of tables that store vital information related to the app. This includes user data such as names, email addresses, and passwords (though all other data is real). The database features information on orders placed by users, available food items, restaurant menus, the restaurants themselves, and the registered users of the app. The tables are interrelated, allowing for efficient data retrieval. The Orders table includes details about each order, such as the order date and time, quantity sold, total sales amount, currency, user ID, and restaurant ID. The Food table provides information about food items, including their ID, name, and whether they are vegetarian or non-vegetarian. The Menu table contains data about restaurant menus, including menu ID, restaurant ID, food ID, cuisine type, and pricing. The Restaurant table holds information about the restaurants, which includes their ID, name, location, rating, number of ratings, average cost, cuisine type, license number, website link, address, and menu. Finally, the Users table contains information about app users, such as their ID, name, email, password, age, gender, marital status, occupation, monthly income, educational qualifications, and family size.
A brief overview of the dataset with key columns and description is given in the following table.

| Table Name       | Columns                              | Key Columns                        | Description                                                                 |
|------------------|--------------------------------------|------------------------------------|-----------------------------------------------------------------------------|
| `food.csv`       | <p align="center">4</p>              | `f_id`, `item`, `veg_or_non_veg`   | Contains unique food items and their vegetarian classification.            |
| `menu.csv`       | <p align="center">6</p>              | `menu_id`, `f_id`, `r_id`, `price` | Maps food items to restaurant menus, including price and cuisine type.     |
| `orders.csv`     | <p align="center">7</p>              | `order_date`, `user_id`, `r_id`    | Records order transactions including sales amount, quantity, and date.     |
| `restaurant.csv` | <p align="center">12</p>             | `id`, `name`, `city`, `rating`     | Information about each restaurant: name, location, ratings, cuisines, and licensing details. |
| `users.csv`      | <p align="center">12</p>             | `user_id`, `Age`, `Gender`         | User demographics including age, income, education, and family size.       |


Python was utilized for basic visualization of key columns. For instance, visualizations of cuisine or price groups were created using pie charts.
<p align="center">
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/veg_vs_non_veg.png?raw=true" alt="Veg vs Non-Veg" width="30%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/distribution_of%20_cuisine.png?raw=true" alt="Cuisine Distribution" width="35.09%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/price_groups.png?raw=true" alt="Price Groups" width="31.32%" />
</p>

For additional visualizations, such as price groups, restaurants, food items, order counts, and dates, vertical bar charts were employed.

<p align="center">
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/price-groups_bar.png?raw=true" alt="Price Groups Bar" width="28.72%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/top_20_f_id.png?raw=true" alt="Top 20 Food IDs" width="34.5%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/top_20_r_id.png?raw=true" alt="Top 20 Restaurant IDs" width="34.5%" />
</p>

<p align="center">
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/top_20_order_date.png?raw=true" alt="Top 20 Order Dates" width="32.5%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/order_count_y_and_m.png?raw=true" alt="Order Count by Year and Month" width="38%" />
  <img src="https://github.com/ShaikhBorhanUddin/Zomato-Data-Analysis/blob/main/Images/order_count_day.png?raw=true" alt="Order Count by Day" width="27%" />
</p>

For more details and python codes for visualizations, click the [link](https://colab.research.google.com/drive/1HsaqNjhSE_akLOapiRKfzaz7DPkM3cNT?usp=sharing).
