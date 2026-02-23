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

- **Source:** Job postings accross EU.
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
   - Download or create your own dataset.
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

## 📚 References

1. Blažič, B. J. (2022). *Changing the landscape of cybersecurity education in the EU: Will the new approach produce the required cybersecurity skills?* Education and Information Technologies, 27, 3011–3036. https://doi.org/10.1007/s10639-021-10704-y

2. Crumpler, W., & Lewis, J. A. (2019). *The Cybersecurity Workforce Gap.* Center for Strategic and International Studies (CSIS). https://csis-website-prod.s3.amazonaws.com/s3fs-public/publication/190129_Crumpler_Cybersecurity_FINAL.pdf

3. Dawson, J., & Thomson, R. (2018). *The future cybersecurity workforce: Going beyond technical skills for successful cyber performance.* Frontiers in Psychology, 9, Article 744. https://doi.org/10.3389/fpsyg.2018.00744

4. Jumaan, S., Kuzminykh, I., Xiao, H., & Ghita, B. V. (2025). *Understanding the skills gap between higher education and industry in cybersecurity.* ResearchGate. https://www.researchgate.net/publication/395473023

5. Marquardson, J., & Elnoshokaty, A. (2020). *Skills, certifications, or degrees: What companies demand for entry-level cybersecurity jobs.* Information Systems Education Journal, 18(1), 22–28. https://files.eric.ed.gov/fulltext/EJ1246234.pdf

6. Peslak, A., & Hunsinger, D. S. (2019). *What is cybersecurity and what cybersecurity skills are employers seeking?* Issues in Information Systems, 20(2), 62–72. https://iacis.org/iis/2019/2_iis_2019_62-72.pdf

7. Ramezan, C. A. (2023). *Examining the cyber skills gap: An analysis of cybersecurity positions by sub-field.* Journal of Information Systems Education, 34(1), 94–105. https://aisel.aisnet.org/jise/vol34/iss1/8

8. Ricci, S., Parker, S., Jerabek, J., Danidou, Y., Chatzopoulou, A., Badonnel, R., Lendák, I., & Janout, V. (2024). *Understanding cybersecurity education gaps in Europe.* IEEE Transactions on Education, 67(2), 190–200. https://doi.org/10.1109/TE.2023.3340868

9. Takács, J. M., & Pogátsnik, M. (2024). *The presence of cybersecurity competencies in the engineering education of Generation Z.* Acta Polytechnica Hungarica, 21(6), 107–127.

10. Zivanovic, M., Lendák, I., & Popovic, R. (2024). *Tackling the cybersecurity workforce gap with tailored cybersecurity study programs in Central and Eastern Europe.* In Proceedings of the 19th International Conference on Availability, Reliability and Security (ARES 2024) (pp. 1–8). ACM. https://doi.org/10.1145/3664476.3670468

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
