# R Sandbox Activity Tutorial

## Overview
This repository contains an R tutorial that introduces fundamental data analysis concepts using R. The tutorial covers package management, data exploration, data cleaning, and visualization using the tidyverse ecosystem.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage Guide](#usage-guide)
- [Code Examples](#code-examples)
- [Visualization Examples](#visualization-examples)
- [Documentation](#documentation)

## Prerequisites
- R installed on your system
- RStudio (recommended)
- Basic understanding of data analysis concepts

## Installation
1. Install R packages required for this tutorial:
```R
# Install tidyverse package which includes ggplot2 and other essential packages
install.packages("tidyverse")

# Load the tidyverse library
library(tidyverse)
```

## Project Structure
The project consists of RMarkdown files demonstrating:
- Package installation and loading
- Data viewing and exploration
- Data cleaning techniques
- Data visualization with ggplot2
- Documentation using RMarkdown

## Usage Guide

### 1. Data Exploration Functions
```R
# Display first few rows of the diamonds dataset
head(diamonds)
```
![Image](https://github.com/user-attachments/assets/a46300d2-bbeb-4458-b58c-3a43edd69b59)
```R
# Show structure of the dataset with detailed column information
str(diamonds)
```
![Image](https://github.com/user-attachments/assets/3343f0cc-35a9-4d95-9412-5306546a4ea0)
```R
# Alternative way to view dataset structure
glimpse(diamonds)
```
![Image](https://github.com/user-attachments/assets/4dbab5ad-bb9c-43da-b047-7dbe6890723e)
```R
# Display column names of the dataset
colnames(diamonds)
```
![Image](https://github.com/user-attachments/assets/cb6c3621-92f0-4de6-9b1a-fa57377f0894)

### 2. Data Cleaning Functions
```R
# Rename a single column
rename(diamonds, carat_new = carat)
```
![Image](https://github.com/user-attachments/assets/c64f002e-33ad-428c-8f0b-35009dce8343)

```R
# Rename multiple columns
rename(diamonds, 
       carat_new = carat,
       cut_new = cut)
```
![Image](https://github.com/user-attachments/assets/167950b8-94a4-4198-932e-f3873ae25b73)
```R
# Calculate summary statistics
summarize(diamonds, 
          mean_carat = mean(carat))  # Calculates mean of carat column
```
![Image](https://github.com/user-attachments/assets/3eb2e560-ea8f-4b1b-a130-7dfdaf82e639)

### 3. Data Visualization
```R
# Basic scatter plot
ggplot(data = diamonds, aes(x = carat, y = price)) +
  geom_point()
```
![Image](https://github.com/user-attachments/assets/5e02c88a-06d7-48e5-89e9-ca63c8f875aa)
```R
# Scatter plot with color coding by cut
ggplot(data = diamonds, aes(x = carat, y = price, color = cut)) +
  geom_point()
```
![Image](https://github.com/user-attachments/assets/f9cef794-3592-4acb-a471-75bc40bacff9)
```R
# Faceted scatter plot separated by cut
ggplot(data = diamonds, aes(x = carat, y = price, color = cut)) +
  geom_point() +
  facet_wrap(~cut)
```
![Image](https://github.com/user-attachments/assets/23a11344-5964-4c43-b944-984a867f2bf3)

## Features
1. **Data Exploration**
   - View data structure and summaries
   - Examine column names and data types
   - Preview data content

2. **Data Cleaning**
   - Rename columns
   - Calculate summary statistics
   - Basic data transformation

3. **Data Visualization**
   - Create basic scatter plots
   - Add color coding to visualizations
   - Create faceted plots for better data comparison

## Function Explanations

### Data Viewing Functions
- `head()`: Shows first 6 rows of dataset
- `str()`: Displays structure of dataset including data types
- `glimpse()`: Alternative to str() with a different format
- `colnames()`: Lists all column names in the dataset

### Data Cleaning Functions
- `rename()`: Changes column names
- `summarize()`: Calculates summary statistics
- Can be combined with other functions for more complex transformations

### Visualization Functions
- `ggplot()`: Creates base plot
- `geom_point()`: Adds scatter plot points
- `aes()`: Defines aesthetic mappings
- `facet_wrap()`: Creates separate plots by category

## Best Practices
1. Always load required packages at the beginning of your script
2. Document your code with comments
3. Use meaningful variable names
4. Break down complex operations into smaller steps
5. Use RMarkdown for reproducible analysis

## Additional Resources
- [Tidyverse Documentation](https://www.tidyverse.org/)
- [ggplot2 Documentation](https://ggplot2.tidyverse.org/)
- [R Markdown Guide](https://rmarkdown.rstudio.com/)

## Contributing
Feel free to fork this repository and submit pull requests for improvements.

## License
This project is open source and available under the [MIT License](LICENSE).
