## Reset Tasks

This Python script is designed to reset scheduled tasks on the PythonAnywhere platform. It retrieves task information from a JSON file, deletes the existing tasks, and then re-schedules the tasks with the same configuration.
Features

    Retrieves task information from a JSON file
    Deletes existing tasks on PythonAnywhere
    Re-schedules the tasks with the same configuration
    Sends a Telegram message to a specified chat ID when a task is successfully reset

## Installation

    Clone the repository:
```
git clone https://github.com/your-username/reset-tasks.git
```
Install the required dependencies:
```
pip install requests
```
Create a data.json file in the same directory as the resettasks.py script, and add the necessary task information in the following format:
```json

{
    "0": {
        "id": 1,
        "command": "your_command",
        "hour": "00",
        "minute": "00",
        "username": "your_username",
        "apikey": "your_api_key"
    },
    "1": {
        "id": 2,
        "command": "another_command",
        "hour": "12",
        "minute": "30",
        "username": "another_username",
        "apikey": "another_api_key"
    }
}
```
Update the tel_tok and chat_id variables in the data.py file with your Telegram bot token and chat ID, respectively.

Run the resettasks.py script:
```
    python resettasks.py
```
# Usage

The resettasks.py script will automatically reset the tasks defined in the data.json file. It will delete the existing tasks and re-schedule them with the same configuration. The script will also send a Telegram message to the specified chat ID when a task is successfully reset.
Contributing

If you find any issues or have suggestions for improvements, feel free to create a new issue or submit a pull request.
