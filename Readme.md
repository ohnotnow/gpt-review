# Code Review Assistant
This is a command-line tool that uses OpenAI's GPT language model to provide code review feedback. It can also be used in chat mode for conversational interaction with the model.

## Installation
To use this tool, you'll need to have Go installed on your system. You can download it from the official website: https://golang.org/dl/

Once you have Go installed, you can download and install the tool using the following command:

go get github.com/openai/openai-review-assistant

## Usage
To use the tool, simply run the openai-review-assistant command followed by your message. For example:
```
review --context=src/thing.go "Please review my go code."
```

To enable chat mode, use the `--chat` flag. For example:
```
review --chat --context=src/thing.go "Please review my go code."
```

## Configuration
To use the tool, you'll need to set your OpenAI API key as an environment variable:
```
export OPENAI_API_KEY=sk-....
```

You can also specify a different OpenAI model to use with the `--model` flag. The default model is gpt-3.5-turbo-16k.

## License
This tool is licensed under the MIT License. See the LICENSE file for more information.
