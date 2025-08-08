# Cognitive Clause Graph: An Interactive Exploration

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

This project is an interactive, single-page application (SPA) designed as a "living document" to explore the **Cognitive Clause Graph (CCG)**, a neuro-symbolic AI framework. It transforms a dense technical concept into an engaging, self-paced narrative journey suitable for both technical and non-technical audiences.

The application details the shortcomings of standard Retrieval-Augmented Generation (RAG) systems in complex logical domains and presents CCG as a robust, auditable, and more accurate alternative.

## Table of Contents

- [The Problem Domain](#the-problem-domain)
- [The Proposed Solution: CCG](#the-proposed-solution-ccg)
- [Key Interactive Features](#key-interactive-features)
- [Design & Architecture Philosophy](#design--architecture-philosophy)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [License](#license)

---

### The Problem Domain

Standard AI approaches like RAG are effective for surface-level information retrieval but falter when faced with the complex, hierarchical, and conditional logic inherent in legal contracts, insurance policies, and enterprise documentation. This SPA interactively demonstrates three critical failure modes:

1.  **Multi-Hop Reasoning:** RAG struggles to connect related but non-adjacent pieces of information to form a logical chain.
2.  **Scope & Hierarchy:** The "chunking" process in RAG flattens document structure, leading to catastrophic context errors where rules are applied incorrectly.
3.  **Quantitative Logic:** RAG's probabilistic nature makes it unreliable for deterministic mathematical or conditional evaluations (e.g., comparing dates or values).

---

### The Proposed Solution: CCG

The **Cognitive Clause Graph (CCG)** represents a paradigm shift from unstructured text chunks to a structured, interconnected graph of clauses and their relationships. This neuro-symbolic architecture provides a "division of labor":

- **Neuro Domain (LLMs):** Handles the art of understanding language—interpreting nuance, identifying entities, and proposing rule structures from raw text.
- **Symbolic Domain (Graph Database & Logic Engine):** Manages the science of enforcing logic—performing deterministic traversals, evaluating conditions, and guaranteeing auditable, logically sound decisions.

---

### Key Interactive Features

The SPA is designed to guide the user through a logical discovery path using a variety of interactive modules.

| Goal         | Feature                  | Implementation               | Justification                                                              |
| :----------- | :----------------------- | :--------------------------- | :------------------------------------------------------------------------- |
| **Compare**  | RAG Failures             | Tabbed Content               | Breaks down complex text into digestible, user-controlled segments.        |
| **Compare**  | CCG vs. RAG Capabilities | Horizontal Bar Chart         | Provides a powerful, at-a-glance visual comparison.                        |
| **Organize** | Ingestion Pipeline       | Clickable Flowchart          | Makes a complex, multi-step process intuitive and explorable.              |
| **Organize** | Multi-Agent Reasoning    | Donut Chart + Clickable List | Connects qualitative agent roles with their quantitative "cognitive load". |
| **Organize** | System Architecture      | Dual-Column Diagram          | Clearly visualizes the separation of concerns in the neuro-symbolic model. |

---

### Design & Architecture Philosophy

The development of this SPA was guided by a clear set of principles outlined in the source:

- **Narrative-First Structure:** The application is designed as a top-down journey. It begins with the high-level business problem, introduces CCG as the solution, allows for interactive deep-dives into its mechanics, and concludes with the value proposition. This structure ensures a logical flow for any user.
- **Purpose-Driven Visualization:** Each visualization was chosen specifically to match the goal of the content. Bar charts are for comparison, flowcharts for process, and donut charts for composition. This enhances comprehension beyond what static text can offer.
- **Constraint-Driven Implementation:** The project was built **without SVG or external libraries like Mermaid.js**. All diagrams and flowcharts are constructed using pure HTML and Tailwind CSS. This demonstrates how complex layouts can be achieved with modern CSS, ensuring maximum compatibility and minimal dependencies.

---

### Technology Stack

- **Structure:** HTML5
- **Styling:** [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework for rapid UI development.
- **Interactivity:** Vanilla JavaScript (ES6) - Used for all interactive elements, including tabs, click events, and scroll-based navigation highlighting.
- **Data Visualization:** [Chart.js](https://www.chartjs.org/) - For creating responsive and interactive bar and donut charts.
- **Fonts:** [Google Fonts](https://fonts.google.com/) (Inter)

---

### Getting Started

This is a static web project with no server-side dependencies.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/cognitive-clause-graph-spa.git](https://github.com/your-username/cognitive-clause-graph-spa.git)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd cognitive-clause-graph-spa
    ```
3.  **Open the file:**
    Simply open the `index.html` file in any modern web browser. For the best experience, use a live server extension in your code editor (like "Live Server" for VS Code) to automatically reload the page on changes.

---

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
