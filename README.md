# Text-Based-Model
Character-Level Language Model for Name Generation

This system learns to generate new names character by character. It works by:

1.  **Learning all unique characters** in a list of names and assigning them numbers.
2.  **Creating 'flashcards'**: For every character in every name, it learns to predict *that character* based on the *few characters just before it* (the 'context').
3.  **Using a tiny neural network** to learn these prediction patterns from the 'flashcards'.
4.  **Generating names**: By starting with a blank context and repeatedly asking the network, "What's the most likely next character?", it builds new names until it predicts an 'end-of-name' signal.

The goal is to create names that sound similar to the ones it was trained on.
