# ML, Explained.

### Machine Learning, From First Principles

**MLBasics** is a free, interactive learning website designed to help beginners build an intuitive understanding of machine learning, from a single number to the building blocks of modern AI.

**[Launch the interactive lessons](https://aaron-ragsdale.github.io/MLBasics/)**

Rather than starting with complex equations or code, the experience introduces one concept at a time using plain-language explanations, interactive visualizations, and optional video resources. The goal is to understand **what the mathematics and models are doing, why they matter, and how the ideas connect**.

## What you'll learn

The website currently includes **22 lessons across seven modules**, organized as a sequential learning path:

| Module | Lessons |
| --- | --- |
| **1. Building blocks** | Scalars, vectors, tensors |
| **2. Data and representation** | Representing data, datasets, training vs. testing |
| **3. Statistical models** | Linear regression, classification, decision trees, clustering |
| **4. How learning happens** | What machine learning is, gradient descent, the perceptron |
| **5. Neural networks** | Neural networks, deep learning, convolutional neural networks (CNNs) |
| **6. Modern language models** | Tokens and embeddings, attention, transformers |
| **7. Responsible ML** | Model evaluation, bias and fairness, real-world deployment |

The lessons build on one another, but you can also jump directly to a topic using the navigation sidebar.

## How it works

Each lesson has:

- **A learning goal** explaining what you should understand by the end.
- **An interactive visualization** to explore the concept by changing values or stepping through an example.
- **What is happening?** A short explanation of the mechanism.
- **Why it matters in ML** to connect the idea to real applications.
- **A takeaway** summarizing the main idea.
- **A clickable lesson title** leading to a relevant YouTube explainer or a targeted YouTube search. Videos include resources from channels such as [3Blue1Brown](https://www.youtube.com/@3blue1brown) and [StatQuest](https://www.youtube.com/@statquest).
- **Previous/next controls** for following the learning sequence.

A progress indicator tracks lessons visited in the current browser. You can reset progress at any time. Visiting a lesson is currently counted as progress; there is no quiz or mastery assessment yet.

## Try the site

**[Open ML, Explained.](https://aaron-ragsdale.github.io/MLBasics/)**

No installation, account, or API key is required. Use a modern browser on a desktop, tablet, or phone.

## Repository structure

```text
MLBasics/
├── index.html    # Entire learning experience: HTML, CSS, JS, and visualizations
└── README.md     # Project overview and instructions
```

The site is currently a single-page static application. Lesson descriptions, navigation, styling, and canvas-based interactive examples all live in `index.html`.

## Run or modify the site

To work on the project, clone the repository:

```bash
git clone https://github.com/aaron-ragsdale/MLBasics.git
```

Open `index.html` in a browser, or edit it directly on GitHub and commit your changes. For the hosted version, GitHub Pages publishes the static page from the configured branch.

**GitHub Pages setup:** Go to **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, and save. The published URL uses the case-sensitive repository name `MLBasics`.

### Adding or editing lessons

In `index.html`, look for the JavaScript `lessons` array. Each lesson defines its module, title, explanation, learning goal, takeaway, visualization type, and video resource. The visualization code is handled by `initDemo()`.

If adding a new lesson, update the relevant demo logic and check that navigation, progress counts, and mobile layout still work correctly.

## Privacy and technical details

- The application is hosted as a **static GitHub Pages website**.
- The interactive lesson calculations run **in the browser**, without a machine-learning API or remote inference server.
- Visited-lesson progress is stored locally using the browser's `localStorage`.
- No account or subscription is required.
- The page loads Google Fonts and links to external YouTube learning resources. Those external services have their own privacy practices.

**Note:** The visualizations are educational simplifications intended to build intuition, not production model-training tools.

## Project direction

Potential future improvements include:

- Short quizzes, prediction challenges, and checks for understanding.
- A continuous example dataset carried through multiple lessons.
- Interactive training demonstrations showing loss, weights, and parameter updates.
- More detailed model comparisons and discussions of overfitting and generalization.
- Additional lessons on backpropagation, random forests, gradient boosting, computer vision, generative AI, and model evaluation.
- More accessibility support, including alternatives to canvas-only visuals.
- Curated individual video links for every lesson.

## Audience

Designed for students, teachers, makers, and curious learners who want an accessible entry point into machine learning. No prior coding or advanced math background is assumed.

## Contributing

Feedback, corrections, and suggestions for new lessons are welcome through [GitHub Issues](https://github.com/aaron-ragsdale/MLBasics/issues).

---

**ML, Explained.** Learn the building blocks. Experiment with the ideas. Understand how modern machine learning works.
