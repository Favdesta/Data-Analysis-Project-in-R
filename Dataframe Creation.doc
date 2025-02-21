# R Dataframe Creation Tutorial

## Overview
This repository contains a tutorial demonstrating how to create, inspect, and manipulate data frames in R. The tutorial walks through the basics of vector creation, data frame construction, and common data inspection techniques using the tidyverse ecosystem.

## Prerequisites
- R installed on your system
- RStudio (recommended)
- Basic R programming knowledge

## Installation

```R
# Install tidyverse package for data manipulation
install.packages("tidyverse")

# Load the tidyverse library
library(tidyverse)
```
![Image](https://github.com/user-attachments/assets/622ed6ee-bbfd-4f67-a4bd-d2fbc11b48ce)

## Tutorial Contents

### 1. Creating Basic Vectors and Data Frames

```R
# Create a vector of names using the combine (c) function
names <- c("Peter", "Jennifer", "Julie", "Alex")

# Create a vector of ages
age <- c(15, 19, 21, 25)

# Combine vectors into a data frame
people <- data.frame(names, age)
```

### 2. Data Frame Inspection Methods

```R
# Display first few rows of the dataset
head(people)
```
![Image](https://github.com/user-attachments/assets/0faff082-2307-44ee-84eb-cef78081485e)
```R
# Show detailed structure of the data frame
str(people)
```
![Image](https://github.com/user-attachments/assets/6a41f6b3-372f-4922-9091-4d312a7c5d02)
```R
# Alternative way to view data frame structure
glimpse(people)
```
![Image](https://github.com/user-attachments/assets/87a3378f-717c-4e72-b520-a2b398ef1405)
```R
# List all column names in the data frame
colnames(people)
```
![Image](https://github.com/user-attachments/assets/fc5f99cf-af66-4846-948a-447cd5887ac2)
### 3. Data Manipulation Example

```R
# Add new column calculating age in 20 years
mutate(people, age_in_20 = age + 20)
```
![Image](https://github.com/user-attachments/assets/2965925d-873a-40b0-a7df-bd08ca5bf30c)
### 4. Practice Exercise - Fruit Rankings

```R
# Create vector of fruits
fruit <- c("Lemon", "Blueberry", "Grapefruit", "Mango", "Strawberry")

# Create vector of rankings (1 = most preferred, 5 = least preferred)
rank <- c(4, 2, 5, 3, 1)

# Combine into a data frame
fruit_ranks <- data.frame(fruit, rank)
```
![Image](https://github.com/user-attachments/assets/354e8776-fca5-4545-8441-bf6861348457)
## Function Explanations

### Vector Creation
- `c()`: Combines values into a vector
  - Example: `c("Peter", "Jennifer")` creates a character vector
  - Example: `c(15, 19)` creates a numeric vector

### Data Frame Functions
- `data.frame()`: Creates a data frame from vectors
  - Vectors must be of equal length
  - Column names are derived from vector names

### Inspection Functions
- `head()`: Shows first 6 rows of data frame
- `str()`: Displays structure including data types
- `glimpse()`: Alternative structure view (tidyverse)
- `colnames()`: Lists column names

### Manipulation Functions
- `mutate()`: Adds new columns to data frame
  - Can perform calculations using existing columns
  - Original data frame remains unchanged unless reassigned

## Best Practices

1. **Vector Creation**
   - Ensure all vectors are the same length
   - Use meaningful names for vectors
   - Double-check data types

2. **Data Frame Management**
   - Use descriptive column names
   - Verify data frame structure after creation
   - Keep track of data types

3. **Code Organization**
   - Load all required packages at start
   - Comment your code
   - Use consistent naming conventions

## Common Issues and Solutions

1. **Vector Length Mismatch**
   ```R
   # Error: vectors must be same length
   names <- c("Peter", "Jennifer")
   age <- c(15, 19, 21)  # Wrong! Different length than names
   ```

2. **Data Type Mismatches**
   ```R
   # Check data types
   str(people)  # Verify correct data types
   ```

3. **Column Name Conflicts**
   ```R
   # Use unique, descriptive names
   names <- c("A", "B")  # Avoid generic names like 'names'
   ```

## Tips for Extending the Tutorial

1. **Add More Columns**
   ```R
   # Add additional information
   height <- c(68, 71, 65, 69)
   people <- data.frame(names, age, height)

   head(people)
   ```
  ![Image](https://github.com/user-attachments/assets/4695663c-61d0-4dc9-b84a-ce4e85fc40d4)

2. **Practice with Different Data Types**
   ```R
   # Mix character and numeric data
   scores <- data.frame(
     student = c("A", "B", "C"),
     grade = c(85, 92, 88),
     pass = c(TRUE, TRUE, TRUE)
   )

   head(scores)
   ```
  ![Image](https://github.com/user-attachments/assets/151df897-741b-4d04-b7d3-a3e3a9935b81)

## Additional Resources
- [Tidyverse Documentation](https://www.tidyverse.org/)
- [R Data Frame Documentation](https://www.rdocumentation.org/packages/base/versions/3.6.2/topics/data.frame)
- [RStudio Community](https://community.rstudio.com/)

## Contributing
Feel free to submit issues and enhancement requests.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
