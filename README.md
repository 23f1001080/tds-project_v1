This repository contains our Tools in Data Science (TDS) course project (v1) for the IITM BS Diploma program. The project demonstrates a complete end-to-end AI-assisted development and evaluation workflow where an application is automatically built, deployed, tested, and revised based on structured requests.

In this project, we had to develop an API endpoint capable of receiving and verifying JSON-based task requests that include details such as email, task ID, round number, brief, evaluation URL, and attachments. Upon receiving a valid request, the endpoint generates an application using an LLM-based generator, pushes the code to a GitHub repository, and deploys it to GitHub Pages. Once deployed, the system pings the evaluation API with metadata such as the repository URL, commit SHA, and the deployed Pages link to confirm completion.

The instructors then run a series of automated evaluations that include static checks such as verifying the presence of an MIT License and assessing the quality of the README, dynamic checks using Playwright to test the functionality of the app, and LLM-based reviews to evaluate code quality, documentation, and overall performance. Based on these evaluations, a new task request is generated for the next round, requiring us to revise or enhance the application by adding new features, improving interactivity, or handling new data formats.

In the revision phase, we had to verify our secret key, update the app according to the new brief, redeploy the project to GitHub Pages, and ping the evaluation API again with updated details. This entire process simulated a realistic DevOps workflow with continuous integration, automated grading, and AI-based assessment.

Overall, the TDS Project V1 demonstrates the integration of AI-assisted app generation, automated deployment, evaluation, and revision cycles, providing hands-on experience with complete data-driven development, LLM collaboration, and real-time continuous evaluation pipelines within a structured academic framework designed to reflect modern AI development practices.

---
title: LLM Code Deployer
emoji: 🚀
colorFrom: blue
colorTo: green
sdk: docker
pinned: false
app_port: 7860
secrets:
  - MY_SHARED_SECRET
  - GITHUB_PAT
  - GOOGLE_API_KEY
---
