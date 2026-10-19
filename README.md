# tools

A grab bag of small, self-contained programs in C and Python. Each file runs on its own.

## What's here

| File | Language | What it does |
|------|----------|--------------|
| `bankers_algorithm.c` | C | Banker's Algorithm deadlock avoidance: prints the system state from `input.txt` and finds a safe sequence |
| `process_tree.c` | C | Uses `fork()` to build a parent → children → grandchildren process tree and prints each PID/PPID |
| `fake_information_generator.py` | Python | Generates a fake name, email, country and full profile with Faker |
| `handwritten_message.py` | Python | Turns text into a handwriting-style image with pywhatkit |
| `print_calendar.py` | Python | Prints a calendar for any year and month you enter |

## Running

**C programs** (Linux/macOS; `process_tree.c` needs a POSIX system for `fork()`):

```bash
gcc bankers_algorithm.c -o bankers_algorithm && ./bankers_algorithm
gcc process_tree.c -o process_tree && ./process_tree
```

**Python scripts** (Python 3.8+):

```bash
pip install -r requirements.txt   # only Faker and pywhatkit are third-party
python print_calendar.py
```

## Contributing

Suggestions and fixes are welcome. Open an issue or a pull request.

## License

[MIT](LICENSE) © 2023 Jordan Abuhantash
