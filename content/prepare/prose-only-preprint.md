---
title: Prose-only
date: 2025-11-11
site:
  hide_footer_links: True
---

:::{pull-quote}
Sometimes the narrative is all you need, and that's okay! 
:::

Even without any code and data, prose-only content published on Evidence offers more than a PDF:

* Transclusion and reuse
* Rich media content (i.e., videos and iframes)
* Rabbit-hole links ([🐇](https://mystmd.org/guide#cool-myst-features))
* Published as structured data (machine readable)

# Prepare your preprint in 4 easy steps

:::{card}
:header: 1️⃣ **Create a new GitHub repository from the prose-only template**

{button}`Template Repository <https://github.com>`
:::

:::{card}
:header: 2️⃣ **Enable GitHub pages**

On your new GitHub repository, go to {kbd}`Settings`-> {kbd}`Pages` -> {kbd}`Build and deployment` and select **GitHub Actions** as the deployment source.
:::

:::{card}
:header: 3️⃣ **Modify `myst.yml` file**

This configuration file defines your preprint’s metadata, including its title, [authors](https://mystmd.org/guide/frontmatter#frontmatter-authors) and [affiliations](https://mystmd.org/guide/frontmatter#affiliations), [funding](https://mystmd.org/guide/frontmatter#affiliations), and many other fields.

After creating a new repository from the template, start by updating the necessary fields to reflect your new content:

```yaml
project:
  title: 'Your new title'
  subtitle: 'This is optional'
  authors: ...
  affiliations: ...
  keywords:
    - my new keyword 1
    - my new keyword 2
  github: https://github.com/my-gh-owner/my-gh-repo
```

Once you push these changes, a new build will be triggered and appear under the {kbd}`Actions` tab. When the build completes successfully, a URL will be provided to preview your preprint. At this point, you should see your updated title and authors reflected on the page.
:::

:::{card}
:header: 4️⃣ **Modify the actual content**

You care about two files:

- `paper.md`
- `paper.bib`

And your figures etc. 
:::

:::{card}
:header: 5️⃣ **Final check on Evidence**

:::

:::{pull-quote}
🎉 That's it, your preprint is ready for submission!
:::