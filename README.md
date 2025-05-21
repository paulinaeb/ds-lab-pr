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
  - Raw LinkedIn job data (`li_jobs.json`)
  - Translated data (`tr_li_jobs.json`)
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
- **Interactive visualizations:** Word clouds, bar charts, treemaps, and choropleth maps.

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