# Researcher Database Analysis and Ranking

## Overview
This project focuses on extracting, analyzing, and ranking researchers, departments, and universities based on various academic metrics. Using advanced **web scraping techniques**, the project collects data from **IRINS (Indian Research Information Network System) and Stanford Researchers Database**, processes the information, and visualizes rankings through a **Flask-based web application**.

## Features
- **Automated Web Scraping** using Selenium and BeautifulSoup.
- **Data Analysis & Ranking** based on H-Index, total citations, i10 index, and publications.
- **Flask Web Application** for interactive ranking and visualization.
- **University, Department, and Professor Ranking System**.
- **Integration with Google Scholar** for enriched profiling.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: BeautifulSoup, Selenium, Pandas, Flask, Requests, ThreadPoolExecutor
- **Data Storage**: CSV, Pandas DataFrames
- **Visualization**: MPAndroidChart (for results)

## Data Sources
- **IRINS Database** ([irins.inflibnet.ac.in](https://irins.inflibnet.ac.in/))
- **Stanford Researchers Database**
- **Google Scholar** (for extended citation metrics)
- **AD Scientific Index** (for additional researcher insights)

## Web Scraping Approach
1. **Dynamic Content Handling**: Selenium automates browser navigation and handles pagination.
2. **Data Extraction**: BeautifulSoup extracts professor names, affiliations, citation metrics, and other data.
3. **Google Scholar Enrichment**: Additional publication and impact data are retrieved from Google Scholar profiles.
4. **Storage & Processing**: Data is structured using Pandas and stored as CSV files.

## Flask Web Application
- **Homepage**: Displays top-ranked researchers and departments.
- **Professor Ranking**: Users can filter rankings by citation count, H-index, and publications.
- **Department Ranking**: Departments ranked based on aggregated professor scores.
- **College/University Ranking**: Overall institutional ranking based on research output.
- **Impact Score Calculation**: Custom metric combining citations, JCI, and publications.

## Installation & Setup
### Prerequisites
- Python 3.7+
- ChromeDriver (for Selenium)
- Required libraries:
  ```sh
  pip install selenium beautifulsoup4 pandas flask requests cloudscraper
  ```

### Running the Web Scraper
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/Researcher-Ranking.git
   cd Researcher-Ranking
   ```
2. Run the web scraper:
   ```sh
   python scraper.py
   ```
3. Process the scraped data:
   ```sh
   python data_processor.py
   ```

### Running the Flask Web Application
```sh
python app.py
```
Then open `http://127.0.0.1:5000/` in a browser.

## Results
- **IRINS Dataset**:
  - **204** universities analyzed.
  - **1,697** departments ranked.
  - **20,570** researchers profiled.
- **Stanford Dataset**:
  - **3,963** colleges ranked.
  - **91,946** researchers analyzed.
  - **3.06M+** total publications considered.

## Future Enhancements
- **Expand Data Sources**: Include more global university databases.
- **Real-Time Updates**: Automate periodic data refresh.
- **Interactive Dashboard**: Enhanced visualization with charts and graphs.
- **Machine Learning**: Predict researcher impact scores based on trends.

## Screenshots


