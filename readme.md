# Premise Parser

A Python parser for analyzing logical premises and conclusions.

## Overview

This project provides a simple premise parser that analyzes a given text to identify logical premises and conclusions. It supports implications, conjunctions, and conclusions.

## Features

- Parse logical statements with implications and conjunctions.
- Determine the validity of conclusions based on the provided premises.
- Support for simplification and modus ponens.

## Usage

1. Initialize the parser with a logical statement:
   ```python
   from parser import PremiseParser

   text = "If today is Tuesday, I have a test in English or Science. If my English Professor is absent, then I will not have a test in English. Today is Tuesday and my English Professor is absent. Therefore, I have a test in Science."

   parser = PremiseParser(text)
   ```
2. Parse the logical statements:
   ```python
   parser.parse()
   ```   
3. Perform simplification and modus ponens:
   ```python
   parser.simplification()
   parser.modus_ponens()
   ```   
4. Describe the parsed premises and conclusion:
   ```python
   parser.describe()
   ```

## Example
   ```python
   text = "If today is Tuesday, I have a test in English or Science. If my English Professor is absent, then I will not have a test in English. Today is Tuesday and my English Professor is absent. Therefore, I have a test in Science."
   
   parser = PremiseParser(text)
   parser.parse()
   parser.simplification()
   parser.modus_ponens()
   parser.describe()
   ```

## Contributors
- Abdelrahman Khaled

Feel free to contribute, report issues, or suggest improvements!