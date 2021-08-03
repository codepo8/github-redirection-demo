# Redirecting with GitHub pages

This is a quick demo showing you how you can redirect markdown files in GitHub pages using an HTML template. You can check the [source code and fork/change it to your needs](https://github.com/codepo8/github-redirection-demo/).

You can use the `forward.html` layout template to redirect any one of your markdown files to another document. By default, it redirects directly, but you can tweak the time and the messaging you want to show to your needs using Markdown frontmatter.

The simplest option is to choose the `forward` template and define a `target` URL to send the user to.

## Plain redirect

This just sends the user directly to the URL you provide. Try [plain-redirect.md](plain-redirect)

```markdown
---
layout: forward
target: https://example.com
---
```

## Other options

You have a few more options to set to customise your redirect:

```markdown
---
layout: forward
target: https://example.com
targetname: Example.com
targettitle: Taking you to example.com
time: 10
message: This isn't here any more!
---
```

* `target` is the URL to redirect to. This defaults to the `target` URL
* `targetname` is the text to display for the URL
* `targettitle` is the title shown in the heading and the page title. This defaults to "Redirecting to `targetname`"
* `time` is the time in seconds
* `message` is the message to show above the link provided as a fallback

You can try this example [redirect-all-options-set.md](redirect-all-options-set)
