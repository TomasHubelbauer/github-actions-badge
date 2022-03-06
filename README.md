# GitHub Actions Badge

Use this MarkDown snippet to add a GitHub Actions status badge to your repo's readme:

```markdown
![](https://github.com/tomashubelbauer/${repo}/workflows/${name}/badge.svg)
```

```markdown
![](https://github.com/tomashubelbauer/${repo}/workflows/.github/workflows/${name.yml}/badge.svg)
```

You can use GitHub to generate the badge for you. Go to your latest workflow run, click on the
triple-dot menu and select *Create status badge*.

For more information about GitHub Actions workflows, see
[github-actions](https://github.com/TomasHubelbauer/github-actions).

## GitHub Pages Badge

This one is a little tricky, at the GitHub Pages pipeline is hidden and as such
provides no control over its file name or workflow name (`name` in the YAML).

I found it using the Actions tab, finding the GitHub Pages workflow, using the
triple-dot menu and its Create Status Badge item. That UI generates the correct
URL regardless of the pipeline type.

```markdown
![](https://github.com/tomashubelbauer/${repo}/actions/workflows/pages/pages-build-deployment/badge.svg)
```
