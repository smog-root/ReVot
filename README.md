# ReVot🤖 
Reverse Image Search Telegram Bot Using MS Azure (server maybe off)

![](https://badgen.net/badge/icon/azure?icon=azure&label)
![](https://img.shields.io/badge/OS-Linux-informational?style=flat&logo=linux&logoColor=white&color=2bbc8a)
![](https://badgen.net/badge/icon/terminal?icon=terminal&label)
![](https://badgen.net/badge/icon/telegram?icon=telegram&label)
![](https://badgen.net/badge/icon/pypi?icon=pypi&label)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<!-- toc -->

- [How To Use Me❓](#how-to-use-me)
- [Features:✨](#features)
- [Commands:🧩](#commands)
- [Local installation💻](#local-installation)
- [Errors and Fixes❌](#errors-and-fixes)

<!-- tocstop -->

## How To Use Me❓
Send me images, gif or stickers(non-animated), I will send you direct reverse image search links of IQDB, Google, TinEye, Yandex and
Bing. For anime images IQDB and TinEye, for other images I recommend to use Google, Bing and Yandex.

## Features:✨
- Give you image reverse search links
- Supports normal images like JPG, PNG, WEBP
- Supports stickers
- Supports GIFs (can take some time till the GIFs are ready)

## Commands:🧩
- /help, /start: show a help message with information about the bot and it's usage.
- /best_match URL: Search for the best match on TinEye (and IQDB when nothing is found on TinEye). The `URL` is a link
    to an image

### Local installation💻
With this info we now install our virtualenv with:
```bash
pip install pipenv  # Install pipenv
pipenv --three      # Create virtualeenv from your python3 installation
pipenv install      # Install all requirements
pipenv shell        # Spawn shell for your pipenv virtualenv
```

You have to get an API Token from Telegram. You can easily get one via the [@BotFather](https://t.me/BotFather).

Now that you have your API Token copy the `settings.example.py` to `settings.py` and paste in your API Token.
Finally you can use this to start your bot.
```bash
python run_bot.py
```
## Errors and Fixes❌
- Use [Python v3.6](https://www.python.org/downloads/release/python-360/) as default
- ssh-keyscan -H <IP address/Hostname> >> ~/.shh/known_hosts
- sudo -H pip install -U pipenv

## Techstack
# Programming Language: 
  -Python 3.6+
# Libraries:
  -pipenv: For virtual environment and dependency management
  -python-telegram-bot: For interacting with Telegram APIs
  -Reverse Image Search Engines:
    -Google
    -Bing
    -Yandex
    -TinEye
    -IQDB
# Platform:
  -MS Azure for hosting
# Databases:
  -SQLite (for user-specific data like search history, preferences)

### Repository Structure 📂

```plaintext
ReVot/
│
├── .github/                  # GitHub-specific files
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md     # Template for reporting bugs
│       ├── custom.md         # Custom issue template
│       └── feature_request.md # Template for requesting features
│
├── deploy/                   # Deployment scripts and configurations
│   ├── after_push            # Post-deployment scripts
│
├── reverse_image_search_bot/ # Main bot directory
│   ├── uploaders/            # Uploader modules
│   │   ├── __init__.py       # Initialize uploaders package
│   │   ├── base_uploader.py   # Base class for uploaders
│   │   ├── file_system.py     # File system operations
│   │   └── ssh.py            # SSH related functions
│   │
│   ├── __init__.py           # Initialize bot package
│   ├── bot.py                # Main bot logic
│   ├── commands.py           # Command handling for the bot
│   ├── image_search.py       # Functions for reverse image search
│   ├── settings.example.py    # Example settings file for API tokens
│   ├── settings.example1.py   # Another example settings file
│   ├── utils.py              # Utility functions and helpers
│
├── LICENSE                   # License information
├── Pipfile                   # Pipenv dependencies
├── Pipfile.lock              # Locked dependency versions
├── README.md                 # Main project documentation
└── run_bot.py                # Script to run the bot

```

# How to Contribute 🌍
We welcome contributions from the community! Here's how you can contribute:

1. **Fork the Repository**: Click on the "Fork" button at the top of this repository.

2. **Clone Your Fork**: Clone your forked repo to your local machine.
   ```bash
   git clone https://github.com/your-username/ReVot.git
   cd ReVot
   ```

3. **Create a Branch**: Create a new branch for your feature or bug fix.
   ```bash
   git checkout -b feature-name
   ```

4. **Make Changes**: Implement your changes and commit them.
   ```bash
   git add .
   git commit -m "Add a detailed description of your changes"
   ```

5. **Push to Your Fork**:
   ```bash
   git push origin feature-name
   ```

6. **Submit a Pull Request**: Go to the original repository and submit a PR from your fork.

We will review your submission and provide feedback.

# Contribution Guidelines 📝
To maintain the quality and consistency of the project, please adhere to the following guidelines:

1. **Code Style**: Follow PEP 8 for Python code formatting.

2. **Testing**: Ensure that all new features are covered by unit tests. Use the `tests/` folder to add new tests.

3. **Commit Messages**: Use clear and descriptive commit messages. Format your commit messages according to the following convention:
   - `feat`: for new features
   - `fix`: for bug fixes
   - `docs`: for documentation updates
   - `test`: for testing-related changes

4. **Pull Requests**: Ensure that your branch is up-to-date with the latest changes from the main branch before submitting a PR. Clearly describe your changes in the pull request.


### License 📜
This project is licensed under the MIT License. You are free to use, modify, and distribute this software as long as the original license and copyright notice are retained.