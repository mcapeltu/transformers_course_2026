# Transformers 2026 — Course Site

GitHub Pages-ready course site for the **Transformers 2026** block, including:

- general course material overview
- mini-project brief and expectations
- deployment and execution notes for the skeleton notebook
- direct access to the solution code for the mini-project
- downloadable lecture PDFs

## Repository structure

```text
.
├── index.html
├── README.md
├── mini-project.html
├── deployment.html
├── syllabus.html
├── assets/
│   └── style.css
├── notebooks/
│   └── mini_project_template_transformer.ipynb
├── Mini-project_workshop.pdf
└── Transformers.pdf
```

## Publish with GitHub Pages

### Option A: simplest static-site workflow
1. Create a new GitHub repository, for example `transformers-2026`.
2. Upload all files from this folder to the repository root.
3. In GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Save the configuration.
6. After a minute or two, your site will be available at:
   `https://YOUR-USERNAME.github.io/transformers-2026/`

### Option B: keep the notebook in the repo and open it in Colab
- Users can browse the notebook directly from GitHub.
- They can also open the `.ipynb` file in Google Colab after downloading it or importing it from the GitHub repository.

## Recommended repository additions

To make the site fully course-ready, you may later add:

- `input.txt` with the corpus used in class
- a `LICENSE` file if you want to define reuse conditions
- screenshots of generated samples
- a small `requirements.txt` if you want stricter environment reproducibility

## Minimal runtime requirements for the notebook

- Python 3.10+
- PyTorch
- Jupyter Notebook or JupyterLab

Typical installation:

```bash
pip install torch jupyter
```

## Notebook assumptions

The provided solution notebook:

- uses **PyTorch**
- includes a fallback text corpus if `input.txt` is not found
- can run on CPU, and will use GPU if the notebook/environment is configured accordingly

## Suggested next step

After uploading the repo, edit the homepage title and the contact details in `index.html` so the public page matches your preferred wording.
