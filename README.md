# 🚀 GitHub Pages CI/CD Task

A static web page displaying our team members' details, deployed automatically to **GitHub Pages** using **GitHub Actions CI/CD workflow**.

---

## 🌐 Live Website

🔗 **[View Live Site](https://ahmed7731.github.io/github-pages-task/)**

---

## 📌 Project Overview

This project satisfies the team task requirements by setting up:
1. **Static HTML Page (`index.html`):** Displays the names and student IDs of team members in a clean layout.
2. **GitHub Repository:** Hosts all source code and configuration files.
3. **CI/CD Automation (`.github/workflows/deploy.yml`):** Automatically builds and deploys the latest version of the website to GitHub Pages whenever changes are merged into the `main` branch.

---

## 👥 Team Members

| **Ahmed Mansour** | `20240055` |

| **Omar Ali** | `20242228` |

| **Teammate 3** | `789012` |

| **Teammate 4** | `654321` |

| **Teammate 5** | `789012` |

| **Teammate 6** | `654321` |


---

## ⚙️ CI/CD Workflow Details

The automated deployment pipeline is configured using **GitHub Actions**:

* **Workflow File:** `.github/workflows/deploy.yml`
* **Trigger (`on`):** `push` events to the `main` branch.
* **Runner Environment (`runs-on`):** `ubuntu-latest`
* **Key Steps:**
  1. **Checkout Code:** Uses `actions/checkout@v4` to pull repository files.
  2. **Setup Pages:** Uses `actions/configure-pages@v4` to initialize GitHub Pages.
  3. **Upload Artifacts:** Uses `actions/upload-pages-artifact@v3` to package the static HTML file.
  4. **Deploy:** Uses `actions/deploy-pages@v4` to publish the page to the web.

---

## 📁 Repository Structure

```text
github-pages-task/
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions CI/CD deployment configuration
├── .gitignore              # Ignores system & temporary files
├── README.md               # Project documentation
└── index.html              # Main HTML page with team details
 
