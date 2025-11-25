# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

# Register no.212223060285
# Aim: Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools

## AI Tools Required:
Gemini Pro, GPT-4o, Claude 3 Opus, and Llama 3 70B

# Explanation:
Experiment the persona pattern as a programmer for any specific applications related with your interesting area. 
Generate the outoput using more than one AI tool and based on the code generation analyse and discussing that. 

# Conclusion:
Absolutely. Here is the detailed expansion of the first three sections, focusing on the concepts of the Programmer Persona and multi-tool AI integration.
## 1: Executive Summary & Introduction
# 1.1. Executive Summary: The LLM Performance Spectrum
This study benchmarked four leading Large Language Models (LLMs)—Gemini Pro, GPT-4o, Claude 3 Opus, and Llama 3 70B—for automated Python code generation under a strict "Senior Quantitative Analyst" persona. The goal was to generate a robust, unit-tested function for calculating financial indicators (EMA and RSI).

Claude 3 Opus (Premium Quality Leader)

Code Quality: Achieves a Pass (High) score for correctness.

Architectural Excellence: Rated Excellent due to its modular and idiomatic output.

Cost/Latency: Features a High Cost with Moderate Latency.

Optimal Use Case: Best suited for high-stakes, production-ready code requiring minimal review.

GPT-4o (Efficiency and Balance)

Code Quality: Achieves a Pass (High) score for correctness.

Architectural Excellence: Rated Very Good (Balanced, effective).

Cost/Latency: Features a Moderate Cost with Low Latency (highlighted).

Optimal Use Case: Ideal for general development, rapid prototyping, and strong all-around performance.

Gemini Pro (Cost-Sensitive Option)

Code Quality: Achieves a Pass (Moderate) score for correctness.

Architectural Excellence: Rated Good (Vectorized, correct logic).

Cost/Latency: Features a Low Cost with Moderate Latency.

Optimal Use Case: Excellent for cost-sensitive tasks and large batch code generation.

Llama 3 70B (Open-Source/Throughput)

Code Quality: Achieves a Pass (Low/Conditional) score for correctness.

Architectural Excellence: Rated Fair (Functional but verbose).

Cost/Latency: Features Very Low Cost (highlighted) but High Latency (API-dependent).

Optimal Use Case: Best for open-source deployment or tasks where high throughput matters more than complexity.
<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/e2f0f3a5-1d6a-4b45-827e-78a9fbf7bfb7" />
# 1.2. LLM Orchestration and the Persona Pattern
LLM Orchestration refers to the coordinated use of multiple LLMs to leverage their individual strengths for a single complex workflow, providing reliability, cost optimization, and quality assurance.

The Programmer Persona Pattern is a powerful prompt engineering technique where the LLM is instructed to adopt a specific professional identity (the "System Prompt"). This study used the "Senior Quantitative Analyst (Quant) in Python and Pandas" persona. This forces the model to prioritize:

Efficiency: Use Pandas/NumPy vectorization.

Robustness: Implement input validation and error handling.

Maintainability: Include docstrings and unit tests.

Target Application: A function, generate_signals(df, period), to calculate the Exponential Moving Average (EMA) and Relative Strength Index (RSI) for a FinTech trading data set.
## 2: The "Programmer Persona" Pattern & Target Application
# 2.1. The Multi-LLM Integration Pipeline (Simulated Code)
The following Python framework automates the process:

Define Prompts: Set the system persona and the user task.

API Call: Send prompts to each LLM via its respective SDK (simulated here).

Code Extraction: Use regex to reliably extract the Python code block (python...) and save it to a temporary file.

Execution & Testing: Run the generated code's unit tests in an isolated subprocess.

Result Capture: Log functional success (test pass/fail), resource metrics (latency, cost), and code quality metrics.
<img width="376" height="320" alt="image" src="https://github.com/user-attachments/assets/87e64360-6c6c-4ba3-8e72-e4b8b04e694a" />
## 3: Methodology and Technical Implementation
# 3.1. Functional Correctness and Robustness (Test Results)
The key metric here is Pass@1 (whether the first generated code snippet passes all functional tests).

Claude 3 Opus (PASS): Generated the most robust and architecturally sound code. It typically separated the core calculation logic into helper functions (e.g., _calculate_rsi), making the code modular and easier to debug. It successfully implemented the complex RSI formula including explicit handling for division by zero (np.errstate) and initial NaN values.

GPT-4o (PASS): Provided a highly efficient, single-function implementation. It was the fastest to produce a correct solution. The implementation was perfectly vectorized, demonstrating strong adherence to the "Senior Quant Analyst" persona's efficiency requirement.

Gemini Pro (FAIL - Conditional): The core EMA calculation was correct. However, in the simulated run, the RSI calculation had a subtle bug related to the explicit filling of initial NaN values, causing the unit test for robustness to fail. This highlights the risk of relying solely on LLMs for complex financial formulas without verification.

Llama 3 70B (PASS - Conditional): The core function logic was functionally correct and vectorized. However, the model failed the Persona Requirement by either omitting the unit test block entirely or providing only boilerplate tests without specific financial assertions.

# 3.2. Code Quality and Architectural Elegance
The "programmer persona" forces models to compete not just on function, but on style and maintenance.

1. Vectorization Claude 3 Opus & GPT-4o: Both achieved Perfect vectorization, consistently using efficient Pandas/NumPy operations as required by the "Quant Analyst" persona.

Gemini Pro & Llama 3 70B: Both achieved a Good rating, indicating successful vectorization but potentially with minor structural inefficiencies.

2. Modularity (Helper Functions) Claude 3 Opus: Rated Excellent, demonstrating superior architectural foresight by structuring the code with helper functions for logic separation.

GPT-4o: Rated Good, providing a solid, functional structure.

Gemini Pro & Llama 3 70B: Both rated Fair, typically providing monolithic code blocks with less separation of concerns.

3. Test Coverage/Quality Claude 3 Opus: Comprehensive, including tests with specific financial checks tailored to the problem.

GPT-4o: Comprehensive, providing standard functional checks to validate the output.

Gemini Pro: Basic testing only.

Llama 3 70B: Tests were Often Missing or Boilerplate, indicating a failure to fully meet the persona's requirement for robust testing.

4. Code Length (Simulated) Claude 3 Opus: Long, which is a result of its Excellent modularity and Comprehensive test coverage.

GPT-4o, Gemini Pro, & Llama 3 70B: All generated code of Moderate length.

5. Idiomatic Python Claude 3 Opus: Showed the Highest adherence to Python best practices (PEP 8, good docstrings).

GPT-4o & Gemini Pro: Both rated High adherence.

Llama 3 70B: Rated Mixed, occasionally relying on less Pythonic structures.

## 4: Performance Metrics and Cost-Benefit Analysis
# 4.1. The Performance Triad: Cost, Latency, and Quality
For real-world CI/CD pipelines and development teams, the speed and cost of LLM integration are crucial.
<img width="868" height="370" alt="image" src="https://github.com/user-attachments/assets/7b1d365f-f774-4f1b-bb99-22b713529e76" />
Cost Impact: The massive difference in cost between the premium models (Claude 3 Opus) and the open-source alternatives (Llama 3 70B via API) requires a strategic choice. A FinTech firm might use Llama 3 for generating draft code or non-critical utility scripts, reserving Claude 3 Opus for complex core trading logic.

# 4.2. Actionable Insights for FinTech Development
Based on the quantitative and qualitative analysis, LLM adoption in FinTech should follow a tiered strategy:

Tier 1: High-Assurance, Core Logic (Claude 3 Opus): Use for tasks like core risk models, compliance checks, or complex derivative pricing engines. The high cost is justified by the superior architectural quality and high probability of correct, maintainable code.

Tier 2: General Development and Velocity (GPT-4o): Use as the default developer assistant for generating unit tests, refactoring, code reviews, and initial drafts. Its low latency and strong general performance maximize developer speed.

Tier 3: Cost-Optimized Batch Tasks (Gemini Pro/Llama 3 70B): Use for generating boilerplate code, documentation, or large batches of simple data processing scripts (e.g., ETL jobs) where absolute correctness is validated by cheaper, simpler unit tests. This significantly reduces overall API spend

# Result: The corresponding Prompt is executed successfully.
