# TechDocs Matrix Build – GitHub Actions Demo

This repository demonstrates a **multi-platform matrix build** using **GitHub Actions**.  
Each build variant runs in parallel and produces a unique artifact, showcasing how to manage CI/CD pipelines efficiently for automation across environments.

---

## 🧩 Workflow Overview
- **Workflow file:** `.github/workflows/matrix-build.yml`
- **Matrix Configuration:** Node.js versions **14**, **16**, and **18**
- **Artifact naming:** `build-9fcda85-v<version>`
- **Step identifier:** `matrix-9fcda85`
- **Artifact Management:** Uses `actions/upload-artifact@v4`
- **Parallel Execution:** Each Node.js version runs as a separate parallel job

---

## 📦 Example Artifacts
After a successful workflow run, three artifacts will be generated:


Each artifact contains non-empty build output such as version details, timestamps, and success confirmation.

---

## 🚀 How to Trigger the Workflow
1. Push any commit to the **main** branch.  
2. GitHub Actions will automatically start the matrix build workflow.  
3. You can monitor progress and results in the **Actions** tab under  
   *“Multi-Platform Matrix Build (9fcda85)”*.

---

## ✅ Validation Checklist
| Requirement | Description | Status |
|--------------|-------------|---------|
| `README.md` contains your email | Must include your IITM email address | ✅ **22f3002016@ds.study.iitm.ac.in** |
| Workflow includes `matrix-9fcda85` step | Required identifier in YAML | ✅ |
| Minimum 3 matrix jobs | Runs for Node 14, 16, 18 | ✅ |
| Artifacts uploaded with prefix `build-9fcda85` | Valid artifact names | ✅ |
| Artifacts have content | Non-empty files confirmed | ✅ |

---

## 📧 Contact
**Maintainer:** Sujit Laware  
**Email:** 22f3002016@ds.study.iitm.ac.in  

For any issues or CI/CD improvements, feel free to reach out via email.

---

## 🧠 Summary
This project demonstrates how GitHub Actions can perform **parallel matrix builds** with artifact generation.  
Each matrix variant runs independently, ensuring scalability, reproducibility, and consistent automation for modern DevOps pipelines.
