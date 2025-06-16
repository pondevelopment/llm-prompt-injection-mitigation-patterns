# **Interactive LLM Security Design Patterns**

This is a single-page, front-end only web application designed to explain and demonstrate key security design patterns for Large Language Model (LLM) agents, specifically for mitigating prompt injection attacks. The content and concepts are based on the academic paper: [**"Design Patterns for Securing LLM Agents against Prompt Injections" (arXiv:2506.08837v2)**](https://arxiv.org/pdf/2506.08837).

Try it [**here**](https://pondevelopment.github.io/llm-prompt-injection-mitigation-patterns/)

The application is built for an audience of software architects, lead developers, and security professionals to provide a clear, interactive, and hands-on understanding of these critical security concepts.

## **Features**

* **Interactive Walkthroughs:** Each security pattern is explained with a step-by-step simulation that users can advance at their own pace.  
* **Visual Diagrams:** Simplified diagrams illustrate the architecture of each pattern.  
* **Clear Explanations:** Concise descriptions of each pattern, its purpose, and how it mitigates prompt injection.  
* **Zero Dependencies:** The application is a single HTML file with no build step required. It uses a CDN for Tailwind CSS.  
* **Responsive Design:** The interface is designed to work well on desktop and mobile devices.

## **Patterns Covered**

The application provides interactive demonstrations for the following six design patterns:

1. **Action-Selector:** The agent's capabilities are restricted to selecting from a predefineda list of actions.  
2. **Plan-Then-Execute:** The agent creates a fixed plan before interacting with untrusted data, preventing the plan from being altered mid-execution.  
3. **LLM Map-Reduce:** Untrusted data is processed in parallel by isolated, single-purpose sub-agents, and the results are safely aggregated.  
4. **Dual LLM:** A privileged, tool-using LLM is shielded from untrusted data by a quarantined, tool-less LLM.  
5. **Code-Then-Execute:** The agent generates a formal program that is executed by a secure runtime, locking in the logic before execution.  
6. **Context-Minimization:** The agent "forgets" the original user prompt after its initial use to prevent it from influencing later steps.

## **How to Use**

Simply open the index.html file (the file containing the application code) in any modern web browser such as Google Chrome, Mozilla Firefox, or Microsoft Edge. No local server or build process is necessary.

## **Technology Stack**

* **HTML5**  
* **Tailwind CSS** (loaded via CDN)  
* **Vanilla JavaScript** (ES6+)

## **Credit**

This educational tool is based entirely on the concepts and diagrams presented in the paper [**"Design Patterns for Securing LLM Agents against Prompt Injections"**](https://arxiv.org/pdf/2506.08837). All credit for the underlying security patterns and research belongs to the authors of that paper.
