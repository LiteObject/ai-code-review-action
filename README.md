# AI Code Review Action

# My Composite Action

A reusable GitHub Action to perform setup and run a custom script.

## Inputs
- `example-input`: An example input parameter (required, default: 'default-value').

## Outputs
- `example-output`: The result of the script execution.

## Usage
```yaml
steps:
  - uses: <your-username>/my-composite-action@v1.0.0
    with:
      example-input: 'Test Value'
  - run: echo "Output: ${{ steps.my-composite-action.outputs.example-output }}"