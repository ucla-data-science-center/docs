You’re right, that last one would break because of the nested code fences. Here’s a **clean version with no outer code block**, so you can paste straight into `README.md`:

---

# UCLA Data Science Center Documentation

This repository contains the source for the UCLA Data Science Center’s documentation site. The site provides guides, handbooks, and internal reference materials for DSC staff, the DataSquad, and campus collaborators. It is built with Jekyll and the Just the Docs theme and published through GitHub Pages.

The live site is here:

[https://ucla-data-science-center.github.io/docs/](https://ucla-data-science-center.github.io/docs/)

## What This Repository Contains

* The **DataSquad Handbook**, including onboarding, workflows, and internal guides
* Documentation for DSC services and teaching materials
* Pages that support shared operations across the Data Science Center
* Administrative reference content that benefits from stable version control

All content in this repository is written in Markdown and organized inside the `docs/` directory, which GitHub Actions builds and publishes.

## Contributing to the Docs

* Edit or add pages in the `docs/` directory
* Keep file names clear and organized
* Use short headers and direct language
* Follow existing navigation patterns
* Open a pull request when you want changes reviewed

The documentation site rebuilds automatically when the `main` branch is updated.

## Related Resources

* DSC public organization:
  [https://github.com/ucla-data-science-center/](https://github.com/ucla-data-science-center/)

* DataSquad Handbook:
  [https://ucla-data-science-center.github.io/docs/docs/handbook/DataSquad_Handbook_Home.html](https://ucla-data-science-center.github.io/docs/docs/handbook/DataSquad_Handbook_Home.html)

* DataSquad project intake and onboarding templates:
  [https://github.com/ucla-data-science-center/DataSquad/issues/new/choose](https://github.com/ucla-data-science-center/DataSquad/issues/new/choose)

## Technology and Attribution

This site uses:

* **Jekyll**, a static site generator
* **Just the Docs**, a theme designed for clean documentation
  [https://just-the-docs.github.io/just-the-docs/](https://just-the-docs.github.io/just-the-docs/)

The repository structure originated from the public **just-the-docs-template**, which is distributed under the MIT License. We thank the Just the Docs project and the wider open source community for maintaining tools that make documentation easier to build and maintain.

## Local Preview

To preview the site locally:

1. Install Ruby, Bundler, and Jekyll

2. From the repository root, run:

   ```bash
   bundle install
   bundle exec jekyll serve
   ```

3. Open `http://localhost:4000` in your browser

Local builds help you test navigation, links, and formatting before pushing changes.

## License

This repository follows the licensing terms provided by the Just the Docs template and by Jekyll. See the MIT License file included with the theme for details.
