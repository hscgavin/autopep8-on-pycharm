# autopep8-on-pycharm

The rules governing Python code formatting are codified in a document named PEP 8. If you want to apply those rules to a given codebase, Tool autopep8 can automate that job. It neatens up Python code to match PEP 8, and returns warnings about specific lines that need developer attention.

Let me show you how to set up autopep8 on pycharm to make your python life much easier.


## Install autopep8 package

Open your terminal / cmd run the following command:

```
pip install autopep8
```

## Open Pycharm

 1. Open external tool: `Preference → Tools → External Tools → +`
 ![External tool](imgs/img1.png?raw=true)
 
 2. Configuration
 <ul>
  <li>Name：Autopep8 (Whatever name)</li>
  <li>Tools settings:</li>
  
  ```
  Programs：autopep8 （Make sure you have installed）
  Parameters: --in-place --aggressive --aggressive $FilePath$
  Working directory: $ProjectFileDir$
  ```
  <li>Under "Advanced Options" → "Output Filters" enter a regular expression to match output：$FILE_PATH$\:$LINE$\:$COLUMN$\:.*</li>
  </ul>
  
  ![External tool setting1](imgs/img2.png?raw=true)
  
  
## usage

External Tools → Autopep8
 