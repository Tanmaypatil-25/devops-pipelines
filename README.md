# DevOps Pipelines Playground 🚀

A lightweight, hands-on sandbox repository designed for experimenting with **CI/CD pipelines** using **GitHub Actions**. This workspace contains a minimal Node.js application (`index.js`, `test.js`, and `package.json`) to test automated building, dependency caching, and test execution.

---

## 📂 Repository Structure

```text
devops-pipelines/
├── .github/
│   └── workflows/
│       └── pipeline.yaml   # GitHub Actions CI workflow configuration
├── index.js                # Main application file
├── test.js                 # Automated test suite
└── package.json            # Project dependencies and test scripts
```

---

## ⚙️ CI Pipeline Overview

The automated workflow (`.github/workflows/pipeline.yaml`) triggers on every `push` to the `main` branch. It provisions an isolated virtual environment to validate code integrity automatically.

### Pipeline Stages:
1. **Checkout Code:** Pulls the latest repository commit using `actions/checkout`.
2. **Setup Environment:** Configures a modern Node.js runtime environment with built-in dependency caching for optimized execution speeds.
3. **Install Dependencies:** Installs project packages securely and deterministically using `npm ci`.
4. **Run Tests:** Executes the project test suite (`npm test`) to ensure all components pass before merging or deployment.

---

## 🛠️ Getting Started Locally

If you want to run or test the application locally on your machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Tanmaypatil-25/devops-pipelines.git
   cd devops-pipelines
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the test suite:**
   ```bash
   npm test
   ```

---

## 🎯 Purpose & Learning Goals
* Understanding the core components of GitHub Actions (`on`, `jobs`, `runs-on`, `steps`).
* Debugging YAML indentation, syntax structures, and action versions.
* Implementing continuous integration practices for Node.js projects.