# Prompting-Machine
A Machine that creates prompts.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Create a propmt for Language Model, machine." \
  | uvx prompting-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install prompting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
prompting-machine -a multilogue.txt
```
Or:
```bash
prompting-machine multilogue.txt > response.txt
```
Or:
```bash
prompting-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import prompting_machine
```
