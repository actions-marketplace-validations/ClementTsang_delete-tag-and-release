# GitHub Action: Delete tag and release

Add following step to the end of your workflow:

```yaml
- uses: dev-drprasad/delete-tag-and-release@v0.1.1
  with:
    delete_release: true # default: false
    tag_name: v0.1.0 # tag name to be delete
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
