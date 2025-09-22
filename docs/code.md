# Code workspace & reproducibility checklist

Use this page to inventory scripts, notebooks, and services that power the **Defining Tipping Points and Transformation** sprint. Each entry should make it clear how to rerun the workflow and where to find outputs.

````markdown
### Example: Early warning indicator notebook
**Purpose:** Calculates rolling variance and autocorrelation for candidate tipping point indicators.
**Location:** `code/early-warning-indicators.ipynb`
**How to run:**
```bash
mamba activate summit
jupyter nbconvert --to notebook --inplace --execute code/early-warning-indicators.ipynb
```
**Outputs:** `docs/assets/results/indicator_trends.png`
````

## Add your workflows
- [ ] Name and link to the script or notebook
- [ ] Note required inputs (data paths, parameters, environment)
- [ ] Document execution steps (CLI commands or notebook instructions)
- [ ] Link to outputs or page where the results are summarized

## Environment & dependencies
List shared environments (e.g., `environment.yml`, `requirements.txt`, Dockerfiles) and provide setup instructions so collaborators can replicate the analysis.

## Testing ideas
- Run unit tests or smoke tests if you add substantial code.
- Capture command history in `documentation/group-notes.md` for transparency.
