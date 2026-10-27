# Exercise: Writing a draft introduction with a basic Copilot Agent. 

This exercise will help you explore and critically evaluate how different scientific publishers address the use of Generative AI tools in manuscript writing and figure creation.
Grouping: in pairs
Time: 10 min

## **Step 1: Open the skill starter template in a text editor**

- Open [this link](https://raw.githubusercontent.com/vib-training-conferences/gen_AI_for_Scholarly_work/refs/heads/main/.claude/skills/skill-starter/SKILL.md) in a browser
- Click on `Raw` on the right upper side of the page to get the text view of the markdown file.
- Copy and paste in the your text editor.
- Alternatively, download the SKILL.md file by clicking on the Download icon and open it in the text editor.

## **Step 2: Discuss in pairs about the main elements of the description**

 - use guiding questions
       [What it does] + [When to use it] + [Trigger keywords] + [What NOT to use it for]

An example:
```
# ❌ Vague — will not trigger reliably
description: Helps with PDFs.

# ✅ What + when + trigger keywords
description: Extract text and tables from PDF files, fill forms, and merge
  documents. Use when working with PDF documents or when the user mentions
  PDFs, forms, or document extraction.
```

## **Step 3: Write a description of under 1024 characters in the third person**

## **Step 4: Fill in the other metadata of the frontmatter (between –--)**

As reference:

| Field | Required | Constraints |
|---|---|---|
| `name` | **Yes** | Max **64 chars**. Lowercase letters, numbers, hyphens only. No leading/trailing hyphen, no consecutive hyphens. **Must match the parent directory name.** |
| `description` | **Yes** | Max **1024 chars**. Non-empty. Says *what the skill does* and *when to use it*. |
| `license` | No | License name or a reference to a bundled license file. |
| `compatibility` | No | Max **500 chars**. Environment requirements: required system packages, network access, target agent. |
| `metadata` | No | Arbitrary string→string map. Common keys: `author`, `version`. |

## **Step 5:  Save the file**

- Save the content of the developed skill in a folder with the same spelling than the name property of the frontmatter.

Tips for naming the skill:

```
name: pdf-processing       # ✅ valid
name: data-analysis        # ✅ valid
name: PDF-Processing       # ❌ uppercase not allowed
name: -pdf                 # ❌ cannot start with a hyphen
name: pdf--processing      # ❌ consecutive hyphens not allowed
```
