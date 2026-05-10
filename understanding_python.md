
# Introduction to Python in Data Analytics

In my quest to understand data and interpret, I found out that python is one of the important languages that is useful for analysis. 
So lets breaks break it down piece by piece so that it can be clear for anyone who is as curious as I to navigate through it.

## What is Python?

Python is a programming language used for data analysis, web development ,automation,  machine learning , Artificial Intelligence and more

Some of the reasons why it is widely used is that

    - It is beginner-friendly. 

    - It has powerful data libraries. 

    - It handles large datasets efficiently. 

    - It supports data visualization. 

    - It integrates with databases and APIs easily. 

    - It is open-source and free. 

One may ask, what is a library as far as python is concerned. 

This is a collection of pre-written code that helps to perform specific tasks without writing everything from scratch.
 Library basically contains functions, classes, and tools that make programming easier and faster.

## Python Libraries Used in Data Analytics

<img width="1063" height="950" alt="image" src="/python1.png" />
		


Lets dive in on how python is Used to Clean, Analyze, and Visualize Data.
## 1. Data Cleaning

Python helps to

-  duplicates 

- Handle missing values 

- Fix incorrect data types 

- Filter unwanted data 

## 2. Data Analysis

Python helps to

- Calculate averages 
- Group data 
- Find trends 
- Perform statistical analysis 

## 3. Data Visualization

Python creates charts such as:

- Bar charts 

- Pie charts 

- Histograms 

- Line graphs 

In trying to understand how python is applied in real-world case scenario in data analytics, here is a break down of what I got:

<img width="1063" height="950" alt="image" src="/python2.png" />	

Beginners should learn Python because:

- It is easy to understand. 

- It is highly demanded in the job market. 

- It is useful in data science and AI. 

- It has a large support community. 

- It works well with databases and APIs. 

Here is a breakdown of working with JSON Data from GitHub

### Step 1: Create Synthetic JSON Dataset

You can create a synthetic dataset using mockaroo .

Example of fields you can use include

- id 

- first_name 

- last_name 

- email 

- gender 

- country 

once you generate the dataset,export it as JSON

### Step 2: Upload JSON File to GitHub

- Create a public GitHub repository. 

- Upload the JSON file. 

- Open the JSON file. 

- Click Raw. 

- Copy the raw GitHub link. 

Example raw link:
https://raw.githubusercontent.com/elijahlabsx/data_used/refs/heads/main/international_students_data.json

## Step 3: Python Code to Read JSON from GitHub and Save as CSV
import requests

import pandas as pd

- Raw GitHub JSON URL
url = " https://raw.githubusercontent.com/elijahlabsx/data_used/refs/heads/main/international_students_data.json"

- Request data from GitHub

response = requests.get(url)

- Convert response to JSON

data = response.json()

- Convert JSON to DataFrame

df = pd.DataFrame(data)

- Display DataFrame

print(df.head())

- Save DataFrame as CSV

df.to_csv("github_data.csv", index=False)

print("CSV file saved successfully.")

## Part 3: Working with DummyJSON API Endpoints

-1. Products Endpoint

Endpoint:

https://dummyjson.com/products

Python Code

import requests

import pandas as pd

- Products API URL

url = "https://dummyjson.com/products"

- Send request

response = requests.get(url)

-  Convert response to JSON

data = response.json()

- Extract products data

products = data["products"]

- Convert to DataFrame

df = pd.DataFrame(products)

-  Display first rows

print(df.head())

-  Save to CSV

df.to_csv("products.csv", index=False)

print("Products CSV saved successfully.")

2. Carts Endpoint

Endpoint:

https://dummyjson.com/carts

Python Code

import requests

import pandas as pd

- Carts API URL

url = "https://dummyjson.com/carts"

- Send request

response = requests.get(url)

- Convert response to JSON

data = response.json()

- Extract carts data

carts = data["carts"]

- Convert to DataFrame

df = pd.DataFrame(carts)

- Display first rows

print(df.head())

- Save to CSV

df.to_csv("carts.csv", index=False)

print("Carts CSV saved successfully.")

Required Python Libraries Installation

pip install pandas requests

After running the scripts, you will get:

-	github_data.csv 

-	products.csv 

-	carts.csv 

These CSV files will contain well-structured tabular data ready for analysis.

# CONCLUSION

- Python is a fairly simple programming language that is easy to learn.
- I urge everyone who shares my curiosity about data, analytics, and artificial intelligence to thoroughly study and comprehend these fields in order to become today's and tomorrow's trailblazers.

