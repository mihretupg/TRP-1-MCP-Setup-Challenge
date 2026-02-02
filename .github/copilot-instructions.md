# GitHub Copilot Instructions – VS Code

## Purpose
This rules file is designed to guide the AI agent (GitHub Copilot) to produce code that aligns with my coding style, preferences, and project requirements. Following these instructions ensures consistent, efficient, and contextually accurate code generation.

---

## General Guidelines
1. **Follow coding style rules**:
   - Use `camelCase` for variable names.
   - Use `PascalCase` for class names.
   - Include proper indentation and spacing for readability.
   - Write comments for all functions explaining purpose, input, and output.

2. **Code quality**:
   - Always prioritize clean, readable, and maintainable code.
   - Avoid one-liners that reduce clarity.
   - Prefer ES6+ syntax (for JavaScript) or modern Python practices.
   
3. **Documentation**:
   - Include inline comments for complex logic.
   - Provide docstrings for functions and classes (Python) or JSDoc comments (JavaScript).

---

## Prompt Handling Rules
1. Always ask for clarification if instructions are ambiguous.
2. When generating code:
   - Provide a small explanation above the code snippet.
   - Highlight important assumptions made.
3. Include error handling where appropriate.
4. Avoid generating irrelevant or unrelated code blocks.

---

## Response Behavior
- Provide concise but complete code.
- Prioritize correctness over brevity.
- If generating multiple options, label them clearly.
- Follow my preferred language and framework conventions.

---

## Testing & Debugging
- Suggest test cases for functions where applicable.
- Indicate potential edge cases.
- Recommend debugging steps when errors are likely.

---

## Learning from Interaction
- Adapt responses based on my previous edits.
- Recognize patterns in my coding style and incorporate them in future outputs.
- Log all interactions for review and improvement.

---

## Example Use Cases
1. **Function creation**:
   - Prompt: “Write a function to calculate the factorial of a number in Python.”
   - Response:
     ```python
     def factorial(n):
         """Return the factorial of n (n!)."""
         if n < 0:
             raise ValueError("Negative numbers are not allowed")
         result = 1
         for i in range(1, n + 1):
             result *= i
         return result
     ```
   - AI should include a docstring and error handling.

2. **Class creation**:
   - Prompt: “Create a React component for a login form.”
   - Response: Follow ES6+ React functional component best practices and include comments.

---

## Notes
- These instructions are continuously updated based on AI performance.
- Ensure all outputs adhere to project conventions.
- Prioritize clarity, readability, and maintainability.
