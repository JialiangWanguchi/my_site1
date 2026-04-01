# Reflection Questions - Assignment 1

### 1. What files make up your site and what does each one do?
- **index.html**: The entry point/gallery page. It organizes all 25 iterations into a cohesive narrative, allowing the user to explore the design process from "Going Wide" to "Refining."
- **versions/v1.html - v25.html**: Individual, self-contained landing page iterations. Each file represents a specific design direction or refinement step, containing all necessary HTML and internal CSS to ensure portability and simple deployment.
- **CLAUDE.md**: A project configuration file that defines the goals, tech stack, and design principles of the Aether project.
- **extract_docx.py / content.txt**: (Meta) Utility scripts and text extracts used during the rapid prototyping process to parse the assignment requirements.

### 2. Describe the pipeline: what happens from git push to your site updating on Vercel?
Once I run `git push`:
1. **GitHub Trigger**: GitHub receives the new commits.
2. **Vercel Webhook**: Vercel is configured to listen for changes on the project's repository. When a push occurs, GitHub sends a webhook signal to Vercel.
3. **Build Phase**: Vercel's build servers pull the latest code. Since this is a pure HTML/CSS project, there is no "compile" or "build" step needed (like npm install or webpack), but Vercel still prepares the environment.
4. **Deployment**: Vercel uploads the static files to its Edge Network (CDNs).
5. **Live Update**: The Vercel URL is updated to point to the new deployment, usually within seconds, making the changes live globally.

### 3. Justify v25—after your entire exploration, why did you land on this version?
v25 was selected as the final version because it achieved the perfect balance between two competing design goals explored in previous versions: **High Impact** (from v10/v19) and **Minimalist Zen** (from v5/v15).

Specifically:
- **Typography**: It uses a large, dramatic headline like v10, but refines it with a subtle vertical gradient that makes it feel "premium" rather than just "loud."
- **Focus**: It adopts the centered, no-sidebar layout of v15, which testing showed was most effective for a "distraction-free" application.
- **Micro-details**: It incorporates the subtle entrance animations from v21 and the refined contrast adjustments from v23.
- **Aesthetic**: The "Aether" concept (air/space) is represented through the dark background and subtle ambient glow, creating a sense of depth without adding visual noise.
- **Usability**: The button styling and hierarchy were distilled down to a single primary action that is impossible to miss, fulfilling the landing page's conversion goal while remaining aesthetically pure.
