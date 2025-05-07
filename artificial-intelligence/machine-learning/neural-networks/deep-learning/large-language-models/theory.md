### Large Language Models (LLMs)
- A language model is a [neural network](../../theory.md), and hence a function, where the inputs are the tokens that represent the prompt, and the output is the list of predicted probabilities for the next token.
- LLM-based systems offer an alternative to rule-based systems
- A path forward might be to combine LLM-driven reasoning with explicit manual gates for executing critical decisions

#### Function Calling
- Function Calling is a capability of LLMs that enables them to interact with external tools.
- `Tool use` or `tool calling` is a wider term that includes `function calling`. It refers to a broader set of capabilities that LLMs can use to interact with the outside world. For example, using inbuilt tools like a code interpreter, and retrieval mechanisms.
- A LLM can analyze a natural language input, extract the user’s intent, and generate a structured output containing the function name and the necessary arguments to invoke that function.
- The flow is as follows:
  - the LLM identifies the function to be called
  - it creates a data structure that describes the call, in a structured JSON format
  - it passes that JSON output to a separate program for execution
  - the JSON output is deserialized into a function call in a programming language, and executed within the program’s runtime environment
  ![image2](https://github.com/user-attachments/assets/5ec15c69-6989-4111-abcd-eb318ddf8299)


## References
- https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/
- https://blog.miguelgrinberg.com/post/how-llms-work-explained-without-math
- https://martinfowler.com/articles/function-call-LLM.html
