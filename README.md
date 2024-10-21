 # Exploring the Netflix Dataset: A Comprehensive EDA Project 🎥📊
 **Project Description**:

 
 ![image](https://github.com/AyushTiwari2000/-Exploring_Netflix_Dataset-AComprehensive-EDA-Project-/assets/157293109/2a764efd-5383-471d-b5d8-1f32d724c062)


Welcome to the **Exploring Netflix Dataset** project! This project involves a comprehensive exploratory data analysis (EDA) of the Netflix dataset. Through visualizations, statistical analysis, and insightful exploration, we dive into the world of streaming, content trends, and user preferences.

## 📂 Dataset Overview

The dataset contains information about Netflix TV shows and movies, including titles, genres, release dates, and more.

- **Total Rows:** 7787  
- **Total Columns:** 12  
  - Title, Genre, Director, Cast, Country, Date Added, Release Year, Rating, Duration, Description, etc.

Here’s a sneak peek into the dataset:

| Title                  | Genre        | Release Year | Rating |
|------------------------|--------------|--------------|--------|
| 3%                     | Sci-Fi       | 2016         | TV-MA  |
| 7:19                   | Drama        | 2016         | TV-14  |
| 23:59                  | Horror       | 2011         | R      |

## 🔍 Exploratory Data Analysis (EDA)

### 1. **Missing Data Analysis**
Missing data was analyzed and visualized to identify any gaps in the dataset. Some columns, like **Director** and **Cast**, had significant missing values. 

- Total missing values in **Director** column: 2389
- Total missing values in **Cast** column: 825



### 2. **Content Release Over the Years**
We explored the distribution of TV shows and movies added to Netflix over the years. It shows a sharp increase in Netflix’s content acquisition post-2015.

```python
# Visualizing the number of movies and shows added each year
plt.figure(figsize=(10, 5))
sns.countplot(x='Release Year', data=netflix_data)
plt.title('Content Release Over the Years')
plt.show()
```



### 3. **Top Genres**
Exploring the distribution of genres helped us understand which genres dominate Netflix’s catalog. Drama, Comedy, and Documentaries are the leading genres.



### 4. **Rating Distribution**
The dataset also provides insights into content ratings, revealing that **TV-MA** (Mature Audience) is the most frequent rating.

| Rating   | Count  |
|----------|--------|
| TV-MA    | 2862   |
| TV-14    | 2164   |
| TV-PG    | 863    |

### 5. **Duration Analysis**
The duration of content was analyzed for both TV shows and movies. We identified trends in content length based on the type of media.

```python
# Distribution of content durations
sns.boxplot(x='Type', y='Duration', data=netflix_data)
plt.title('Content Duration by Type')
plt.show()
```



### 6. **Country-Wise Distribution**
The content available on Netflix is produced globally. We analyzed the country-wise distribution to find out which countries contribute the most to the Netflix catalog.



---

## 🛠️ Technologies Used

- **Python**: Data manipulation and visualization
- **Pandas**: For data manipulation
- **Matplotlib & Seaborn**: For plotting graphs and visualizing data
- **Jupyter Notebook**: For running and showcasing the analysis

## 📈 Insights

- Netflix has shown rapid growth in content acquisition, especially after 2015.
- **Drama** and **Comedy** dominate the Netflix catalog.
- Majority of the content is rated **TV-MA**, catering to mature audiences.
- There’s a consistent trend of longer durations in TV shows as compared to movies.

## 📊 Graphs and Visualizations

We used a variety of graphs such as bar charts, heatmaps, and boxplots to make the data exploration process visually appealing and easy to understand.

## 💡 Future Enhancements

- Perform sentiment analysis on show descriptions.
- Incorporate machine learning to predict content success based on past data.
- Further explore user ratings and review trends for better insights.

## 📫 Get in Touch
