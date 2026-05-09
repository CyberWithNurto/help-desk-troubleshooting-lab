# GitHub Markdown Image Path Troubleshooting

## Overview
During my networking lab documentation, I encountered a problem where images uploaded to GitHub displayed a broken image icon (`?`) instead of rendering correctly inside Markdown files.

---

## Problem
The screenshot image would not display correctly inside my Markdown documentation file.

Example:

```markdown
![ipconfig-all](../../../screenshots/windows/networking-basics/ipconfig-all.png)
```

GitHub displayed an image loading error instead of the screenshot.

---

## Root Cause
The issue was caused by an incorrect folder path.

The folder name accidentally contained a hidden space:

```text
windows 
```

instead of:

```text
windows
```

GitHub automatically converted the space into:

```text
%20
```

inside the URL.

---

## Solution
I checked the GitHub image URL directly to identify the real folder path.

The correct path became:

```markdown
![ipconfig-all](../../../screenshots/windows%20/networking-basics/ipconfig-all.png)
```

After updating the Markdown image path, the screenshot displayed correctly.

---

## What I Learned
I learned:
- how Markdown image paths work
- how relative paths work in GitHub
- how `../` moves back one folder
- how `%20` represents spaces in URLs
- how to troubleshoot broken image paths in Markdown documentation

---

## Important Markdown Notes

### Markdown Image Syntax

```markdown
![image-name](path-to-image)
```

### Relative Path Notes

```text
../
```

Moves back one folder.

```text
../../../
```

Moves back three folders.

---

## Real-World Relevance
Technical support engineers and developers frequently troubleshoot:
- broken file paths
- documentation issues
- repository organization
- Markdown rendering problems

Understanding relative paths and GitHub documentation structure is an important technical documentation skill.
