**IOP (Input, Output, Process) Planning for Video Games Sales Data Analysis**

---

**INPUT**:
- Game data: Name, year of publication, genre, publisher.
- Sales by main regions: North America, Europe, Japan, among others.

---

**OUTPUT**:

1. Histograms of the genres of the first 150 titles in the ranking.
2. Scatter plot between year of publication and Nintendo sales from 2010 onwards.
3. List of the top 5 publishers by sales in the United States.
4. Insight analysis.

---

**PROCESS**:

1. **Data Description**:
    - Understand the structure of the data: What columns are present and their types?
    - Basic descriptive statistics: mean, median, minimum, maximum, standard deviation, etc. for numerical columns.
    - Counting single values for categorical columns.
    - Handling missing values: Fill in or delete, depending on the context.
    - Remove possible duplicates.
    - Correct inconsistent records, if identified.
    - Convert data types, if necessary (e.g. ensure that the year of publication is in date format).

2. **Removal of variables**:
    - Row cleaning
    - Removing columns

3. **Feature Engineering (Creation of New Features)**:
    - If necessary, create derived columns that may be useful for subsequent analysis.
    - Group data by relevant categories (e.g. total sales by publisher).
    - Identify the first 150 titles in the ranking based on some criterion (e.g. global sales).

4. **Exploratory Analysis**:
    - **Genre Histograms**:
        - Filter the first 150 titles in the ranking.
        - Create histograms based on the count of games by genre.

    - **Scatter Graph - Nintendo**:
        - Filter the data to consider only Nintendo games published from 2010 onwards.
        - Plot a scatter graph with the year of publication on the X axis and sales on the Y axis.

    - **Top 5 Publishers in the USA**:
        - Group the data by publisher and add up the sales in the USA.
        - Sort the publishers by sales and select the top 5.

    - **Insight analysis**:
        - Validate hypotheses in order to extract insights from the data.
