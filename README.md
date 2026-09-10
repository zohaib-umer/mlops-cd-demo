# MLOps Continuous Delivery Pipeline

This project demonstrates a complete **Continuous Delivery (CD) pipeline** for a simple ML-style inference API using:

- Flask
- Pytest
- Docker
- GitHub Actions
- GitHub Container Registry (GHCR)
- Staging deployment
- Health / smoke testing
- Manual production approval
- Versioned releases
- Rollback support

The main objective is to follow the **build once, deploy many** principle, where the same Docker image tested in staging is promoted to production.

---

## Project Structure

```text
mlops-cd-demo/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── VERSION
├── .gitignore
│
├── tests/
│   └── test_app.py
│
└── .github/
    └── workflows/
        └── cd.yml
