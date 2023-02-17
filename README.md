# GPT Todoist

This is a command-line interface (CLI) script that generates a todo using OpenAI's GPT-3 language model and adds it to a Todoist account using the Todoist Python SDK. The due date for the task can be specified in a human-friendly format (e.g. "next Monday", "tomorrow").

## Requirements

- Python 3.x
- `openai` module (`pip3 install openai`)
- `todoist-api-python` module (`pip3 install todoist-api-python`)
- `python-dotenv` module (`pip3 install python-dotenv`)

Alternatively, you can install the required modules by running `pip3 install -r requirements.txt` in the terminal.

## Usage

1. Open a terminal and navigate to the directory where `add_todo.py` is located.
2. Install the required modules using `pip3 install -r requirements.txt`.
3. Create a `.env` file in the root of your project with your API keys:

	```
	OPENAI_API_KEY=your_openai_api_key
	TODOIST_API_KEY=your_todoist_api_key
	```

4. Run the script using `python3 add_todo.py`.

The script will generate a todo using GPT-3 and prompt you to enter a due date for the task in a human-friendly format (e.g. "next Monday", "tomorrow"). Note that currently, the due date must be entered manually by the user and is not extracted from OpenAI.

## To Do

- [x] Create CLI
- [ ] Create [Raycast extension](https://www.raycast.com/store)
- [ ] Automatically extract due date from OpenAI

## Configuration

You can customize the prompt used to generate the todo using ChatGPT by modifying the `prompt` variable in the `generate_todo` function.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
