# 🐙 GitHub Developer & Repository Analytics — Chicago (`TDS-P1`)

Data collection and exploratory data analysis project for **Tools in Data Science (Project 1)**. This repository queries the **GitHub REST API** to scrape profiles and public repositories of influential developers located in **Chicago** with more than **100 followers**, exporting structured datasets for statistical analysis.

---

## 📂 Repository Structure

| File | Description |
| :--- | :--- |
| `main.ipynb` | Automated GitHub REST API scraper with pagination and rate-limit handling to fetch user profiles and their public repositories. |
| `users.csv` | Cleaned dataset of Chicago-based GitHub users with `>= 100` followers (`login`, `name`, `company`, `location`, `email`, `hireable`, `bio`, `public_repos`, `followers`, `following`, `created_at`). |
| `repositories.csv` | Detailed metadata for public repositories owned by those users (`login`, `full_name`, `created_at`, `stargazers_count`, `watchers_count`, `language`, `has_projects`, `has_wiki`, `license_name`). |
| `LICENSE` | GNU General Public License v3.0. |
| `README.md` | Project documentation and key findings. |

---

## 🔍 Key Insights & Findings

- **Language Diversity**: Chicago's top developers maintain repositories across a wide spectrum of ecosystems, led by **Python**, **JavaScript/TypeScript**, **C++**, **Go**, and **Ruby**.
- **Engagement & Visibility**: Repository star counts and follower growth correlate strongly with consistent documentation, permissive open-source licensing (`MIT`, `Apache-2.0`), and active maintenance.

---

## 🚀 Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sparsh0106/TDS-P1.git
   cd TDS-P1
   ```

2. **Set your GitHub Personal Access Token**:
   ```bash
   export GITHUB_TOKEN="your_github_pat_here"
   ```

3. **Run the notebook**:
   ```bash
   pip install requests pandas numpy scikit-learn matplotlib jupyter
   jupyter notebook main.ipynb
   ```

---

## 📄 License

Licensed under the [GPL-3.0 License](LICENSE).
