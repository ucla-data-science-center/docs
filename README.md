# UCLA Data Science Center Documentation

This repository contains the source for the UCLA Data Science Center’s documentation site. It serves as the central home for DSC guides, handbooks, and reference materials for staff, the DataSquad, and campus collaborators. The site is built with Jekyll using the Just the Docs theme and published through GitHub Pages.

Live site:  
https://ucla-data-science-center.github.io/docs/

## What This Repository Contains

- The DataSquad Handbook, including onboarding and workflows  
- UCLA Dataverse documentation covering deposits, access, and policy  
- Guides for DSC services, consulting, and instructional support  
- Administrative materials that benefit from version control  

All content is written in Markdown and stored in the `docs/` directory. GitHub Actions builds and publishes the site automatically.

## Contributing

- Edit or add pages in the `docs/` directory  
- Keep filenames clear and organized  
- Use short headers and direct language  
- Follow the existing navigation structure  
- Open a pull request for review  

## Related Resources

- DSC GitHub organization  
  https://github.com/ucla-data-science-center/

- DataSquad Handbook  
  https://ucla-data-science-center.github.io/docs/docs/handbook/DataSquad_Handbook_Home.html

- UCLA Dataverse  
  https://dataverse.ucla.edu

- DataSquad intake and onboarding templates  
  https://github.com/ucla-data-science-center/DataSquad/issues/new/choose

## Technology and Attribution

This site uses:

- Jekyll  
- Just the Docs  
  https://just-the-docs.github.io/just-the-docs/

The structure began with the public just-the-docs-template, distributed under the MIT License. We appreciate the open-source community that maintains these tools.

## Local Preview

To preview the site on your machine:

1. Install Ruby, Bundler, and Jekyll  
2. From the repo root, run:

   ```bash
   bundle install
   bundle exec jekyll serve
   ```

Previewing locally helps you check navigation, formatting, and links before pushing changes.

## License

This repository follows the licensing terms of the Just the Docs template and Jekyll. See the included MIT License for details.
