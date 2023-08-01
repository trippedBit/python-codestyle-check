# python-actions
Action to check the codestyle using pycodestyle.
<br><br>
## License
Please see [LICENSE](LICENSE)
<br><br>
## Usage
Create a workflow file inside your repo in .github/workflow and add the following.
Change the name and the triggering event to fit your needs.
```yml
name: check-codestyle

on: [push, workflow_dispatch]

jobs:
    codestyle_job:
        runs-on: windows-latest
        name: Codestyle check
        steps:
            - uses: trippedBit/python-codestyle-check@v1.0.0
  
```
