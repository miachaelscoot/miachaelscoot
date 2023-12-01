#!/usr/bin/python
# -*- coding: utf-8 -*-

class RegionalManager:

    def __init__(self):
        self.name = "Michael Scott"
        self.role = "Regional Manager"
        self.language_spoken = ["en_US"]
        self.office_quotes = [
            "That's what she said!",
            "Would I rather be feared or loved? Easy. Both. I want people to be afraid of how much they love me.",
            "I'm not superstitious, but I am a little stitious.",
            "Well, well, well, how the turntables..."
        ]

    def say_hi(self):
        print(f"Hello, I'm {self.name}, the {self.role}.")
        print("Welcome to Dunder Mifflin, where paper meets personality!")
        print("Remember, the only time success comes before work is in the dictionary.")

    def share_quote(self):
        if self.office_quotes:
            print("Here's a classic Michael Scott quote:")
            print(f'"{self.office_quotes.pop(0)}"')
        else:
            print("I've run out of quotes for now. That's what she said!")

# Create an instance of RegionalManager for Michael Scott
michael_scott = RegionalManager()

# Greet and share a quote
michael_scott.say_hi()
michael_scott.share_quote()
