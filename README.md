# AI Code Review Action

## My Composite Action

A reusable GitHub Action to perform setup and run a script.

### Inputs

* `example-input`: An example input parameter (required, default: 'default-value')
* `ollama-model-name`: Ollama model name (required, default: 'llama3.2:latest')

### Outputs

* `example-output`: The result of the script execution
* `installed-ollama-models`: List of installed Ollama models

### Usage

```yaml
steps:
  - uses: <your-username>/my-composite-action@v1.0.0
    with:
      example-input: 'Test Value'
      ollama-model-name: 'llama3.2:latest'
  - run: echo "Output: ${{ steps.my-composite-action.outputs.example-output }}"
  - run: echo "Installed models: ${{ steps.my-composite-action.outputs.installed-ollama-models }}"