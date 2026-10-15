# Directing-Machine
A machine that regulates the course of...

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Direct this process, machine." \
  | uvx directing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install directing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
directing-machine -a multilogue.txt
```
Or:
```bash
directing-machine multilogue.txt > response.txt
```
Or:
```bash
directing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import directing_machine
```
