Repository under construction. :)

## Problem Statement:
The problem statement is to create benchmarks and evaluate the optimal strategy for creating MCP Clients.  

 ## Rough Plan
 Here is how I plan to do it:
 - Create datasets extrapolating tool usage across single and multiple servers. Then, augment dataset with unanswerable questions. See [here](./dataset_creation/raw_data) for a sample of queries.
 - Test out different prompting strategies in the client: Zero-shot CoT; Plan&Solve; Just-Code; Budget-Forcing ('think' vs. 'dont think') etc.
 - Evaluate on accuracy and the number of tokens for each type of client (aim for a stable metric over multiple runs).
 
## Reason, Motivation & Novelty:
 - While there is some stuff on benchmarking MCP, it is on the server side of things. The aim of creating a protocol is to make sure the tools are interoperable across LLMs. Understanding what makes a generalizable and optimal client could help save time.
 - There are lots of benchmarks on QnA, tool usage; creating such datasets has required crowdsourcing, manual filtering etc. With predefined MCP servers and a recipe - SDG is completely automated and highly scalable.
 - Apart from accuracy, testing for number of tokens generated helps quantify time and energy efficiency of the clients as well.
 - Several tiers of questions - single-server; multi-server; unanswerable with different expectations in behaviour - executing success, handling failure etc. The behaviour could also depend on the environment of the system.


## todo:

### Datasets:
- Scale to a higher number of queries.
- Prepare sandbox (or the-like) environment for tool execution.
- Define expected ground truth behaviour.

### Eval Scripts:

### Experimentation

### Automation, Dashboard & Productionizability

