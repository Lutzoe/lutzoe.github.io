---
title: 'How to Contribute'
slug: '/contribute'
---

## Welcome, Contributors

This project is open source and lives on [GitHub](https://github.com/tgatlas/temporal-graphs-atlas.github.io). We welcome all contributions.

For most changes, please open a **Pull Request**. For bigger ideas or questions, please open an [issue on GitHub](https://github.com/tgatlas/temporal-graphs-atlas.github.io/issues).

---

## Adding or Editing Papers

Paper data is stored as YAML files in the `papers/` directory.

### Paper File Structure

Each paper is a `.yml` file. Name files descriptively (e.g., `Author21topic.yml`). Here's a quick example:

```yaml
title: Temporal Graph Paper Title
authors: Author1, Author2
labels:
- temporal paths
- connectivity
publications:
- name: STOC
  url: https://example.com/paper
  year: 2021
  dblp_key: conf/stoc/Author21 # Optional
  bibtex: "@inproceedings{...}"   # Optional
- name: arXiv
  url: https://arxiv.org/abs/2101.12345
  year: 2021
```

### Key Fields

- **`title`**: Full paper title.
- **`authors`**: Author names.
- **`labels`**: A list of relevant categories (see below for common labels).
- **`publications`**: List of venues, each with a `name`, `url`, and `year`.



---

## Editing Website Content

You can edit the site's informational pages by modifying the markdown files in `public/content/`, such as `about.md` or this very file.
