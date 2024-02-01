Fabric is not just a tool; it's a transformative step towards integrating the power of GPT prompts into your digital life. With Fabric, you have the ability to create a personal API that brings advanced GPT capabilities into various aspects of your digital environment. Whether you're looking to incorporate powerful GPT prompts into command line operations or extend their functionality to a wider network through a personal API, Fabric is designed to seamlessly blend with your digital ecosystem. This tool is all about augmenting your digital interactions, enhancing productivity, and enabling a more intelligent, GPT-powered experience in every aspect of your online presence.

## Features

1. Text Analysis: Easily extract summaries from texts.
2. Clipboard Integration: Conveniently copy responses to the clipboard.
3. File Output: Save responses to files for later reference.
4. Pattern Module: Utilize specific modules for different types of analysis.
5. Server Mode: Operate the tool in server mode for expanded capabilities.
6. Remote & Standalone Modes: Choose between remote and standalone operations.

## Installation

1. Clone the repository:
   `git clone git@github.com:xssdoctor/myAugmented.git`
2. Navigate to the tool's directory:
   `cd myAugmented`
3. Set up a virtual environment:
   `python3 -m venv .venv`
   `source .venv/bin/activate`
4. Install the required packages:
   `pip install -r requirements.txt`
5. copy to path
   `echo export PATH=$PATH:$(pwd)` >> .bashrc`

## Usage

To use Fabric, run the script with the desired options:

python fabric.py [options]
Options include:

--text, -t: Specify the text for summary extraction.
--copy, -c: Copy the response to the clipboard.
--output, -o: Save the response to a file.
--stream, -s: Stream output to another application.
--pattern, -p: Select the module for analysis.
--server, -S: Enable server mode. defaults to 127.0.0.1:5000
--domain, -d: Specify the domain in server mode.
--port, -P: Specify the port in server mode.

Example:

```
echo 'in real life this would be a long article, but this is just an example' | fabric --pattern extractwisdom --output wisdom.txt | fabric --pattern summarize --stream
ONE SENTENCE SUMMARY:

- The content provided is insufficient as it states "pattern not found," indicating a lack of meaningful data.

MAIN POINTS:

1. The input "pattern not found" suggests a search or match operation was unsuccessful.
2. There may have been an attempt to locate a specific sequence or keyword which yielded no results.
3. The phrase could be the output of a software program or script indicating an error or null result.
4. It's possible that the expected content is missing, leading to the given response.
5. The context in which "pattern not found" is used is not provided, making interpretation challenging.
6. This message could imply the need for troubleshooting or refining search parameters.
7. Without additional information, it's unclear what pattern was being searched for.
8. The lack of a found pattern might necessitate alternative approaches or solutions.
9. The statement could be part of a larger process where this is just one outcome or step.
10. Understanding the intended use or goal of the pattern search would be necessary for further action.

TAKEAWAYS:

1. "Pattern not found" indicates an unsuccessful search or matching attempt.
2. Additional context is needed to understand the significance of the message.
3. The message may prompt a review or change in search criteria or methods.
4. This could represent a step in a process that requires further action or adjustment.
5. Understanding the intended pattern is crucial for meaningful analysis or troubleshooting
```

# Server Mode

1. running `febric --server --domain [domain] --port [port]` will start a gunicorn server, allowing you to create a personal api. This server uses both traditional api endpoints and websockets for a great experience. Use cases include iphone shortcuts and creating an api for your web site. The server is gunicorn with python flask. There is also a small web frontend accessable to http://[server]:[port]

# Remote mode

1. if you make a config.yaml file in the directory root, the tool will now be in remote mode. Instead of directly querying the chatgpt server, you can query a remote fabric server (including your own server).


Contributing

We welcome contributions to Fabric! For details on our code of conduct and the process for submitting pull requests, please read the CONTRIBUTING.md.
