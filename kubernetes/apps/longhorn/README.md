# 📦 Longhorn (Helm Chart Deployment)

This directory contains the **Argo CD Application manifest** for deploying [Longhorn](https://longhorn.io/) to the Kubernetes cluster as a distributed persistent storage backend.

Longhorn is deployed via **GitOps with Argo CD**, making it fully declarative and self-healing.

---

## 🚀 Deployment Details

| Feature          | Value                       |
|------------------|-----------------------------|
| **Method**       | Helm chart via Argo CD      |
| **Chart Source** | `https://charts.longhorn.io` |
| **Namespace**    | `longhorn-system`           |
| **StorageClass** | `longhorn` (set as default) |
| **Access Mode**  | `ReadWriteOnce`             |

---

## 📁 Directory Contents

```text
longhorn/
├── longhorn-app.yaml # Argo CD Application manifest
├── README.md         # This file
```

## 📊 Diagram
![image](https://github.com/user-attachments/assets/c15d4f43-5950-433d-9f4b-d960983a98c1)
