# chatbot-dataset-creator

This little python program creates indents (in json format) for chatbots that have
- a tag 
- patterns (specified amount, default 10) 
- responses (specified amount, default 10) 

# How to start 

Just start the creator.py

# Output

The program will save the output in a file called `output.txt`

### Sample output

    {
      "tag": "greeting",
      "patterns": [
        "hello",
        "how are you",
        "hi",

      ],
      "responses": [
        "hey",
        "whats up",
      ]
    }


### How to change the output structure

In the file `structure.txt` is the output structure.
You can change the structure of the output, but remember that the program only recognizes `$TAG`, `$PATTERN` `$RESPONSE`
There are 10 `$PATTERN`s and 10 `$RESPONSE`s in the file. 10 because this is the default maximum amount and if you specify to use less in the program it will just skip the other `$PATTERN`s and `$RESPONSE`s 
