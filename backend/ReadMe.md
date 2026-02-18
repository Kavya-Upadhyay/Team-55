# 🚀 Backend Service

A FastAPI/Uvicorn-based backend for the Team-55 project.

---

## 📋 Prerequisites

- **Python 3.10** or higher
- `pip` (or `conda` for environment management)

---

## 🛠️ Installation & Setup

### Step 1: Create a Virtual Environment

From the **repository root** (`./Team-55`), create and activate a virtual environment:

**Option A: Using Conda** (Recommended)
```bash
conda create -p venv python=3.10 -y
conda activate ./venv
```

**Option B: Using Python venv**
```bash
python3.10 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Step 2: Install Dependencies

Navigate to the backend directory and install requirements:

```bash
cd backend
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Start the ASGI server from the `backend/app` directory:

```bash
cd app
uvicorn app:app --reload --host 0.0.0.0 --port 8000
```

The application will be accessible at:
- **Local:** `http://127.0.0.1:8000/`
- **Network:** `http://0.0.0.0:8000/`

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| `uvicorn` command not found | Ensure `requirements.txt` was installed: `pip install -r requirements.txt` |
| Conda environment not activating | Use full path: `conda activate ./venv` |
| Python version mismatch | Verify Python 3.10 is installed: `python --version` |

---

## 📝 Project Structure

```
backend/
├── ReadMe.md           # This file
├── requirements.txt    # Python dependencies
└── app/
    └── app.py          # Main ASGI application
```

---

## 📧 Support

For issues or questions, please open an issue in the repository or contact the maintainers.
