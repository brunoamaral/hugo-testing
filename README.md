# Hugo GitHub Issue #7982

Details: <https://github.com/gohugoio/hugo/issues/7982>

Description: Hugo cannot identity correct translation string when multiple variants of a language code is used

## Instructions

Clone this branch of the repository and build the site.

```text
git clone --single-branch -b hugo-github-issue-7982 https://github.com/jmooring/hugo-testing hugo-github-issue-7982
cd hugo-github-issue-7982
hugo server
```

You will see a warning, and the same translation of the word "cat" when visiting both the zh and zh-cn site.

Now rename i18n/zh-cn.toml to i18n/zh_cn.toml and run `hugo server` again.

Everything works as expected.
