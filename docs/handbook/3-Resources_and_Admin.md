---
title: Resources
layout: default
parent: DataSquad Handbook
nav_order: 5
---

# Resources

This page lists tools, storage locations, and organizations used in DataSquad work.

---

## Google Drive

The DataSquad uses the **data-science-center** Shared Drive:

<https://drive.google.com/drive/u/0/folders/0AKFJ0mo2-HebUk9PVA>

Key folders:

**data-squad**  
Work logs, handbooks, administrative documents, meeting notes  
<https://drive.google.com/drive/u/0/folders/1oNojx83bIXmwvG3GbIPlmQ4DXhzh4KIF>

**consulting**  
Client project folders, deliverables, shared materials  
<https://drive.google.com/drive/u/0/folders/14feMpx9VpOiCcDHugOysyiskQxQXafQt>

---

## GitHub Organizations

### `ucla-data-science-center`  
Use this for **all client and research project repositories**.  
It holds reproducible workflows, code, collaboration materials, and final deliverables.

<https://github.com/ucla-data-science-center>

New repos must use the **`dsc-template`**. See [Repository Setup & Credit Taxonomy]({{ site.baseurl }}/docs/handbook/3a-Creating_a_Repo.html) for full instructions.

---

## Consulting Best Practices

### Computational Thinking

When working with researchers, encourage clear thinking about code structure:

- **Write a brief description** at the beginning of each program explaining its purpose.
- **Comment your code** to explain the _why_, not just the _what_.
- **Write an outline using pseudo-code** before diving into implementation.
- **Use functions** to organize reusable logic, improve readability, and make testing easier.

For a hands-on introduction, see: [Intro to Computational Thinking](https://gulibrarysandbox.github.io/intro-computational-thinking/)

### Storing and Sharing Code

Choose the right approach based on the researcher's familiarity with version control:

- **If they know Git:** Use a GitHub repo under `ucla-data-science-center`. See [Repository Setup & Credit Taxonomy]({{ site.baseurl }}/docs/handbook/3a-Creating_a_Repo.html).
- **If they don't know Git:** Have the researcher share their code or notebooks via the Google Drive folder for the consultation.

**For R users**, encourage them to:
- Use [RStudio Desktop](https://posit.co/download/rstudio-desktop/)
- Create an `.Rproj` file for the project (see: [Project Management With RStudio](https://swcarpentry.github.io/r-novice-gapminder/02-project-intro.html))

**For Python users**, encourage them to:
- Use [JupyterLab Desktop](https://github.com/jupyterlab/jupyterlab-desktop) or Jupyter Notebook via the [Anaconda Distribution](https://www.anaconda.com/products/distribution)

### Reference Interview: What to Ask the Researcher

During the initial conversation, gather enough context to scope the work:

- What is the research question or goal?
- What data do they have, and in what format?
- What tools or languages are they already using?
- What is their timeline and level of technical experience?
- Are there specific deliverables they need (code, visualization, cleaned dataset)?

### Our Recommendations

When advising researchers, follow these principles:

- **Recommend both code-based and no-code solutions** depending on the researcher's comfort level.
- **Suggest a directory structure** for their project. Keep data, code, and outputs in separate folders.
- **Follow good enough practices** from: Wilson et al., [Good Enough Practices in Scientific Computing](https://doi.org/10.1371/journal.pcbi.1005510). Key takeaways:
  - Put each project in its own directory.
  - Name files and folders to reflect their content or function.
  - Put raw data in a separate folder and treat it as read-only.
  - Write scripts that produce outputs from raw data rather than editing data manually.
  - Record all processing steps in scripts or notebooks.

---

### UCLA-DataSquad

Used only for the DataSquad website and blog. Not for consulting.

https://github.com/UCLA-DataSquad

Publicity and Blog Posts

Every completed project needs a short blog post (200 to 500 words).
Posts should:

- Summarize the problem and solution
- Highlight results or tools used
- Be reviewed by Tim, Leig or Doug
- Include clear tags
- Identify the student author

Blogs help document impact and support future funding.

### Additional Tools

- Slack for internal communication
- GitHub Projects for task tracking
- Google Docs for shared writing
- Zoom for remote consulting
