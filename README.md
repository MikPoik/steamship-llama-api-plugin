# Llama-api Plugin for Steamship

This plugin provides access to llama-api

## Usage

Use of this plugin is subject to OpenAI's [Terms of Use](https://openai.com/policies/terms-of-use).

### Examples

#### Basic

```python
llama = steamship.use_plugin("llama-api")
task = llama.generate(text=prompt)
task.wait()
for block in task.output.blocks:
    print(block.text)
```

#### With agent

completions = self.llm.complete(prompt=prompt,                               
                                max_retries=4)
#Log agent raw output
logging.warning("\n\nOutput form Llama: " + completions[0].text + "\n\n")
```



