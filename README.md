# Minimal IRC Client

A minimal command-line IRC client written in Python.

## Project Goal

To create a simple, functional CLI application that connects to a single IRC server, joins one channel, supports basic commands (NICK, JOIN, PART, PRIVMSG), and relies on library-provided error handling.

## Core Technology Choices

*   **Language:** Python 3 (Requires version compatible with `pydle`, likely >= 3.8)
*   **IRC Library:** `pydle`
    *   **Reasoning:** Chosen over `jaraco/irc` based on the fact that documentation and concurrency is better on `pydle`. `pydle`'s native `asyncio` support is advantageous for handling the concurrency between blocking CLI input and non-blocking network I/O. Its dedicated documentation and modular design are also considered beneficial for this project's minimal scope and focus on leveraging existing library features.
*   **Version Control:** Git
*   **Testing Framework:** (TBD, likely `pytest`)
*   **Local Test Server:** (TBD, likely `ngircd` via Docker)

*(Further sections on Installation, Usage, etc., will be added later)*
