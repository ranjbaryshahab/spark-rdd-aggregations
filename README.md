# Spark RDD Aggregations & Sorting

🚀 A practical guide to working with Apache Spark RDDs, focusing on custom aggregation functions and sorting operations. This project demonstrates how to efficiently process and manipulate student data using Java and Spark.

## 📌 Features
- **Custom Aggregation Functions**: Implementing `AggFunction<T>` for sum and count operations.
- **Sorting Mechanism**: Using merge sort to order data.
- **Partitioning & Grouping**: Utilizing `RangePartitioner` for efficient data partitioning.
- **Spark RDD Operations**: Mapping, filtering, and reducing operations.

## 🚀 Getting Started
### Prerequisites
Ensure you have the following installed:
- [Java 8+](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- [Apache Spark](https://spark.apache.org/)
- [Maven](https://maven.apache.org/)

### 🛠 Setup & Run
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/spark-rdd-aggregations.git
   cd spark-rdd-aggregations
   ```
2. Build the project using Maven:
   ```sh
   mvn clean install
   ```
3. Run the Spark application:
   ```sh
   mvn exec:java -Dexec.mainClass="Application"
   ```
### The dataset (students.csv) contains student exam records with the following fields:
   ```sql
   studentId, examCenterId, subject, year, quarter, score, grade
   ```

## 🛠 Implemented Functions
### 1️⃣ Sorting RDD
- Sorts students by year using merge sort and Spark’s partitioning mechanism.

### 2️⃣ Aggregation Functions
- SumAggFunction: Calculates the total score per year.
- CountAggFunction: Counts occurrences of each grade per year.



