# Wordlist Generator

A C program that generates wordlists with customizable character sets and lengths for security testing and password analysis.

## Features

- Multiple character set options (numbers, letters, symbols, or combinations)
- Configurable maximum word length
- Automatic file naming to prevent overwrites
- Real-time generation progress with animated spinner
- Efficient recursive generation algorithm

## Character Set Options

1. **Numbers**: 0-9
2. **Characters**: a-z, A-Z
3. **Symbols**: Special characters (!@#$%^&*()-_=+[]{}|;:',.<>?/`~)
4. **Numbers + Characters**: Alphanumeric combinations
5. **Numbers + Symbols**: Numeric with special characters
6. **All Combined**: Numbers, letters, and symbols

## Usage

1. Compile the program:
   ```bash
   gcc Wordlist_Generator.c -o wordlist_generator
   ```

2. Run the executable:
   ```bash
   ./wordlist_generator
   ```

3. Select your desired character set (1-6)
4. Enter the maximum word length
5. The program generates all possible combinations and saves them to `wordlist.txt`

## Output

- Generated wordlists are saved as `wordlist.txt` (or `wordlist1.txt`, `wordlist2.txt`, etc. if file exists)
- Shows total word count upon completion
- Displays real-time progress during generation

## Warning

Be cautious with large maximum lengths as the number of generated words grows exponentially with the character set size and length.
