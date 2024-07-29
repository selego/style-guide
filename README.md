# Selego Style Guide

## Introduction
This guide provides standards and best practices for developing projects at Selego, ensuring consistency, readability, and maintainability of our code.

### Purpose
To establish a consistent coding style and workflow for all projects, making collaboration easier and reducing technical debt.

### Why It's Important to Converge to the Same Tech
- **Consistency:** Code should look like it was written by a single person.
- **Quality:** It's better to be consistently BAD than non-consistently GOOD.
- **Adaptation:** If you disagree with something in the whitepaper, write a message in [#whitepaper](https://slack.com/app_redirect?channel=C06Q7TFKTV0) channel in slack. 

### Audience
All Selego developers working on 0 to 1 projects or scale-ups.

### Scope
This guide covers repository structure, branching strategy, commit messages, pull requests, code reviews, coding standards, issue tracking, documentation, automation, security, and best practices, specifically tailored for MERN stack, React Native. 

## Table of Contents
1. [Repository Structure](#repository-structure)
2. [Branching Strategy](#branching-strategy)
3. [Commit Messages](#commit-messages)
4. [Pull Requests](#pull-requests)
5. [Code Reviews](#code-reviews)
6. [Coding Standards](#coding-standards)
7. [Best Practices](#best-practices)
8. [Hosting](#hosting)
9. [Startup Toolkit](#startup-toolkit)
10. [Security](#security)
11. [Documentation](#documentation)
12. [Continuous Improvement](#continuous-improvement)

## Repository Structure
### Directory Layout

├── src
│ ├── 

### File Naming Conventions


## Branching Strategy


## Commit Messages

## Pull Requests
### Creating Pull Requests
- **Good Example:** Provide a clear description, related issue numbers, and screenshots if applicable.
- **Bad Example:** Vague descriptions like "Fix stuff".

### Review Process
- **Checklist:**
- 

### Merging Strategies
- **Good Practice:** Use "Squash and merge" to maintain a clean history.
- **Bad Practice:** Direct merges without reviews.

## Code Reviews
### Guidelines for Reviewers

### Checklist
- Code is readable and maintainable.
- No obvious bugs.

## Coding Standards

### coding standard 1

lalalal

### API Selego Style

**Post search in bold**

```javascript
router.post("/search", async (req, res) => {
  try {
    const query = {};
    if (req.body.hasOwnProperty(req.body.userId)) query.userId = req.body.userId;
    const data = await DeviceModel.find(query);
    return res.status(200).send({ ok: true, data });
  } catch (error) {
    capture(error);
    res.status(500).send({ ok: false, code: SERVER_ERROR, error });
  }
});


