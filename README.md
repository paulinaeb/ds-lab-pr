# 🔐 Cybersecurity Job Market Analysis

## 🚀 Motivation & Objectives

The cybersecurity job market is rapidly evolving, with a growing demand for skilled professionals across Europe. Despite this demand, there is a significant shortage of cybersecurity experts. This project aims to **collect, enrich, explore, analyze, and visualize** the needs of the cybersecurity job market, providing actionable insights for individuals, educators, and policymakers.

**Objectives:**
- Build a comprehensive, up-to-date dataset of cybersecurity job postings from LinkedIn.
- Preprocess and translate multilingual job ads for uniform analysis.
- Explore and visualize trends in job titles, required skills, and geographic distribution.
- Enable data-driven decisions for career planning and workforce development.

---

## 📦 Project Structure

```
ds-lab-pr/
│
├── data/
│   ├── 1/ ... n/         # Iteration folders with raw and translated JSON files
│   ├── data.json         # Main merged, translated dataset (English)
│   └── README.md         # Data folder instructions
│
├── merge-data.ipynb      # Notebook for merging and deduplicating data
├── translate.ipynb       # Notebook for language detection and translation
├── main.ipynb            # Main analysis and visualization notebook
├── requirements.txt      # Python dependencies
└── README.md             # Project overview (this file)
```

**Data Folder Structure:**
- Each iteration folder (`1/`, `2/`, ...) contains:
  - Raw LinkedIn job data (`li_jobs.json`) - merged version
  - Translated data (`tr_li_jobs.json`) - output
  - Subfolders by scrape date with original JSONs

---

## 📊 Data Collection & Processing

- **Source:** LinkedIn job postings, scraped weekly using [ScrapeJob – LinkedIn Jobs Scraper](https://linkedin.scrapejob.net/).
- **Languages:** Multiple European languages, translated to English for consistency.
- **Preprocessing:** Deduplication, cleaning, and normalization of job titles, descriptions, and skills.
- **Merging:** Iterative merging of new data into a unified dataset (`data/data.json`).

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```sh
   git clone <repo-url>
   cd ds-lab-pr
   ```

2. **Set up a virtual environment (recommended):**
   ```sh
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

4. **Download the dataset:**
   - Download from [this link](https://eltehu-my.sharepoint.com/:f:/g/personal/paulinaeb_student_elte_hu/Emp7X-9_FthEnhhDsHGXbtwBXBeu7jHp6usXMBCqkly05g?e=FuEXze)
   - Place the extracted files in the `/data` folder, preserving the folder structure.

---

## 📒 Usage

- **Data Merging:**  
  Run `merge-data.ipynb` to merge and deduplicate raw job data.

- **Translation:**  
  Run `translate.ipynb` to detect languages and translate non-English ads to English.

- **Analysis & Visualization:**  
  Run `main.ipynb` for exploratory data analysis, visualizations (word clouds, bar charts, maps), and insights.

---

## 📁 Data Folder Details

See [`data/README.md`](data/README.md) for more information on the data structure and usage.

---

## 📈 Features

- **Multilingual support:** Automatic detection and translation of job ads.
- **Deduplication:** Ensures unique job postings.
- **Skill extraction:** Standardizes and analyzes required skills.
- **Geographical analysis:** Visualizes job demand across European countries.
- **Interactive visualizations:** Word clouds, bar charts, treemaps, and choropleth map.

---

## 📚 References

1. **Crumpler, W., & Lewis, J. A. (2019). The Cybersecurity Workforce Gap.**  
   [CSIS Report](https://csis-website-prod.s3.amazonaws.com/s3fs-public/publication/190129_Crumpler_Cybersecurity_FINAL.pdf)  
   *A comprehensive report analyzing the global shortage of cybersecurity professionals and its implications for organizations and governments.*

2. **Alshaikh, M., Maynard, S. B., Ahmad, A., & Chang, S. (2021). Cybersecurity skills gap: A state-of-the-art review.**  
   [Education and Information Technologies](https://link.springer.com/article/10.1007/s10639-021-10704-y)  
   *A scholarly review of the cybersecurity skills gap, examining causes, impacts, and potential solutions in education and industry.*

3. **ACM (2024). Cybersecurity Workforce: Trends and Challenges.**  
   [ACM Digital Library](https://dl.acm.org/doi/abs/10.1145/3664476.3670468)  
   *Discusses current trends, challenges, and future directions in the cybersecurity workforce, based on recent research and industry data.*

4. **SciDirect (2025). Cybersecurity labor market analysis using job postings.**  
   [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0167404825000185?ref=pdf_download&fr=RR-2&rr=943c3ca06dba5b00)  
   *Presents a data-driven analysis of the cybersecurity labor market using job posting data to identify demand and skill trends.*

5. **SciDirect (2021). Skills and competencies in cybersecurity: A systematic review.**  
   [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0160791X2100244X)  
   *A systematic review of required skills and competencies in cybersecurity, highlighting gaps between education and industry needs.*

6. **SciDirect (2022). Automated analysis of cybersecurity job postings.**  
   [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0167404822004746)  
   *Explores methods for automated extraction and analysis of cybersecurity job postings to inform workforce development.*

7. **Frontiers (2018). Soft skills and cybersecurity: A psychological perspective.**  
   [Frontiers in Psychology](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2018.00744/full)  
   *Examines the importance of soft skills in cybersecurity roles from a psychological viewpoint.*

8. **AISNet (2021). Mining job postings for cybersecurity skills.**  
   [AIS Electronic Library](https://aisel.aisnet.org/cgi/viewcontent.cgi?article=2000&context=jise)  
   *Describes techniques for mining job postings to identify in-demand cybersecurity skills and trends.*

9. **IACIS (2019). Cybersecurity education and workforce development.**  
   [IACIS](https://iacis.org/iis/2019/2_iis_2019_62-72.pdf)  
   *Focuses on the relationship between cybersecurity education programs and workforce needs.*

10. **ERIC (2020). Cybersecurity workforce development: A review.**  
    [ERIC](https://files.eric.ed.gov/fulltext/EJ1246234.pdf)  
    *Reviews strategies and challenges in developing the cybersecurity workforce, with recommendations for educators and policymakers.*

---

## 🤝 Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements.

---

## 📄 License

This project is for educational and research purposes. Please see LinkedIn's terms of service when scraping data.

---

## 👩‍💻 Author

- Espejo Paulina 
- Data Science I Lab Project, 2025

---