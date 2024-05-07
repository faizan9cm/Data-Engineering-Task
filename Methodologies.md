# Methodologies

Welcome to the Methodologies document! Here, you'll find thorough elucidations of the scripts and methodologies employed in the Data Engineering Task project.

## 1. DataExtractionAndStandardization.py

### Purpose:
This script merges data extraction and standardization tasks. It retrieves HTML content from a set of input URLs, extracts pertinent information, and aligns the data with specified standards.

### Usage:
1. Input URLs are read from the `input_urls.csv` file in the `data` folder.
2. HTML content is fetched using the `fetch_html_content` function.
3. Information is extracted using the `extract_information` function.
4. Data is standardized using the `standardize_data` function.
5. Standardized data is written to the `standardized_data.csv` file in the `data` folder.

## 2. ResearchAndDataSourcing.py

### Purpose:
This script is dedicated to the initial stage of data acquisition and exploration. It retrieves HTML content from a selection of input URLs and produces summaries utilizing BERT-based summarization.

### Usage:
1. Input URLs are read from the `input_urls.csv` file in the `data` folder.
2. HTML content is fetched using the `fetch_content` function.
3. Summaries are generated using the `generate_summary` function.
4. Relevant links are selected based on scores calculated from the summaries.
5. Top relevant links are printed for further processing.

## 3. Combined_Tasks_Code.py

### Purpose:
This script consolidates multiple tasks such as research, data extraction, and standardization into a unified process. It offers a comprehensive methodology for handling data from the initial research phase to producing standardized output.

### Usage:
1. Input URLs are read from the `input_urls.csv` file in the `data` folder.
2. Research and data sourcing are performed to select relevant links.
3. HTML content is fetched using the `fetch_html_content` function.
4. Information is extracted using the `extract_information` function.
5. Data is standardized using the `standardize_data` function.
6. Standardized data is written to the `standardized_data.csv` file in the `data` folder.

## 4. AutomatedDataProcessing.py

### Purpose:
This script showcases automated continuous data updating. It operates within an infinite loop, regularly fetching the most recent data from input URLs and adjusting the standardized data accordingly.

### Usage:
1. Input URLs are read from the `input_urls.csv` file in the `data` folder.
2. The main function runs in an infinite loop with a delay for continuous updating.
3. Data scraping and standardization process is executed at regular intervals.
4. Standardized data is continuously updated in the `standardized_data.csv` file in the `data` folder.
