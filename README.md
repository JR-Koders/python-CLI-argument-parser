
Ever wanted to make your tools **way easier** to use on the *command line*, or just tired of coding the argument handling yourself?
We got you!

---

You can **easily specify** which _arguments_ the user is supposed to enter:

Format: {'option_name': {'short-name': 's', 'long': 'long-name', 'help': 'Description of the option'}}

Ex:
```python
    # Define options with their short and long versions along with descriptions
    options = {
        'verbose': {'short': 'v', 'long': 'verbose', 'help': 'Enable verbose mode'},
        'output': {'short': 'o', 'long': 'output', 'help': 'Specify output file'},
        'port': {'short': 'p', 'long': 'port', 'help': 'Specify port number'},
    }
    # Get command-line arguments excluding the script name
    args = sys.argv[1:]
    # Parse the arguments based on the provided options
    parsed_args = parse_arguments(args, options)
    # Print the parsed arguments
    print("Parsed arguments:", parsed_args)
```

Now it's your turn to go on with your project!

---

**NOTE:** You have to import the *parse_arguments* first to be able to use it.

All credit to [JR-Koders](https://youtube.com/@JR-Koders)