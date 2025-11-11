# 1. Intro to basic concepts
### I. What is Machine Learning?
<img width="642" height="102" alt="Screenshot 2025-11-11 at 8 03 29 AM" src="https://github.com/user-attachments/assets/cb36970b-8054-4aef-8262-e84d38d1bcd9" />

Study of algorithms that
- improve their performance
- at some task
- with experience

## Examples
* Google Photos 
> Uses machine learning to automatically categorize photos into different classes

* Stock Market Prediction
* Image Captioning
* Self-driving Car
* Mind Reading
* Recommender Systems
* Credit Card Fraud Detection
* Computational Entomology
> Given sensor measurements of insects classify them by species/gender

## II. What Is Data Mining?
Knowledge discovery from data 
* Extraction of ***interesting*** (non-trival, implicit, previously unkown, and potentially useful) patterns or knowldege from huge amounts of data

Alternative names
* Data science, knowledge discovery (mining) in databases (KDD), knowledge extraction, data/pattern analysis, business intelligence, etc.

## III. The Data Science Pipeline
1. Raw Data
2. Pre-processing (data integration, data cleaning, feature selection, dimension reduction)
3. Analysis (pattern discovery, association and correlation, classification, clustering, outlier analysis)
4. Post-processing (evaluation, interpretation, visualization)
5. Knowledge
<img width="637" height="345" alt="Screenshot 2025-11-11 at 8 11 49 AM" src="https://github.com/user-attachments/assets/c7e68984-65ca-4772-82b5-35f549ca5ee1" />

## IV. Supervised vs. Unsupervised 
| Feature | **Supervised Learning** | **Unsupervised Learning** |
|----------|--------------------------|----------------------------|
| **Labeling** | Uses **labeled** examples | Uses **unlabeled** data |
| **Goal** | Learn a model that **generalizes** to unseen examples | Learn a model that **finds structure or patterns** in data |
| **Input** | (x, y) pairs — data with known outputs | x only — data without labels |
| **Example Task** | **Classification**, Regression | **Clustering**, Dimensionality Reduction |
| **Key Idea** | Train with answers provided | Discover hidden structure automatically |

## V. What classes of methods are there
* Classification & regression (supervised)
* Clustering (unsupervised)
* Outlier & Anomaly Detection
* Association and Rule Mining

## VI. Classification & Regression
### Classification And Label Prediction
* Construct models (functions) based on some training examples <br>
* Describe and distinguish classes or concepts for future prediction
  * E.g., classify countries based on (climate), or classify cars based on (gas mileage)
* Predict some unknown class labels

### Typical Methods
Decision trees, naive Bayesian classification, support vector machines, neural networks, rule-based classification, pattern-based classification, logistic regression

### Typical Applications
Credic card fraud detection, direct marketing, classifying stars, diseases, web-pages

## VII. Clustering
* Unsupervised leraning (i.e., Class label is unknown)
* Group data to form new categories (i.e., clusters), e.g., cluster documents according to topics
* Principle: Maximizing intra-class similarity & minimizing interclass similarity
* Many methods and applications

## VIII. Outlier & Anomaly Detection
### Outlier Analysis
* Outlier: A data object that does not comply with the general behavior of the data
* Noise or exception? One person's garbage could be another person's treasure
* Methods: by product of clustering or regression analysis
> Useful in fraud detection, rare events analysis

# 2. Data Objects And Attribute Types
## I. Types of Data
### Records
* Relational records
* Data matrix, e.g., numerical matrix
* Document data: text documents: term-frequency vector
* Transaction data
<img width="637" height="189" alt="Screenshot 2025-11-11 at 8 24 20 AM" src="https://github.com/user-attachments/assets/dddbd744-d5dd-455b-98d3-f37686bc4bc7" />

### Graph & Network
* World Wide Web
* Social or information networks
* Molecular Structures
* Knowledge Graphs

### Time-Series
* Temporal Data: time-series
* Sequential Data: transaction sequences
* Genertic Sequence Data
<img width="637" height="203" alt="Screenshot 2025-11-11 at 8 25 54 AM" src="https://github.com/user-attachments/assets/2301c3aa-2c32-4008-8488-4bea8a6feb7b" />

### Spatial, Image, and Multimedia
* Spatial Data: Maps
* Image Data
* Video Data
<img width="637" height="216" alt="Screenshot 2025-11-11 at 8 26 45 AM" src="https://github.com/user-attachments/assets/cd8cf57b-a0c2-4615-ad66-6b4e98479209" />

## II. Data Objects
* Data sets are made up of data objecst
* A **data object** represents an **entity**

#### Examples
* Sales Database: customers, store items, sales
* Medical Database: patients, treatments
* University Database: students, professors, courses

* Also called samples, examples, instances, data points, objects, **tuples**
* Data objects are described by **attributes** or **features**

> Rows -> data objects [Horizontal]
> Columns -> attributes [Vertical]

## III. Features
### Features (or attributes, dimensions, variables)
A data field, representing a characteristic of feature of a data object. 
 * E.g., customer_ID, name, address

## Types of Features
* Nominal/Categorical
* Binary
* Ordinal
* Numerical: quantitative

