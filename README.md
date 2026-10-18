# MainStringsJava

A Java console application that generates possible two-name combinations from three user-provided first names. The user can select a combination to display its initials and generate a suggested username.

## Features

- Accepts three names through console input.
- Generates six ordered combinations by pairing each name with the other two.
- Displays the combinations as a numbered menu.
- Allows the user to select a combination from 1 to 6.
- Displays the first character of each selected name.
- Generates a username by converting both names to lowercase and separating them with an underscore.
- Displays an error message for choices outside the range of 1–6.

## Technologies Used

- **Programming Language:** Java
- **Input:** `java.util.Scanner`
- **Data Structures:** String arrays
- **Application Type:** Console application

## How It Works

1. The program prompts the user to enter three first names.
2. It stores the names in an array.
3. Nested loops generate all ordered pairs of different array entries.
4. The program displays the six combinations.
5. The user selects a combination by entering a number from 1 to 6.
6. The program displays the first character of each selected name and generates a lowercase username.

### Example

Suppose the user enters:

```text
Ichiro
Aria
Hina
```

The possible combinations are:

```text
1 - Ichiro Aria
2 - Ichiro Hina
3 - Aria Ichiro
4 - Aria Hina
5 - Hina Ichiro
6 - Hina Aria
```

If the user selects option `1`, the output includes:

```text
The initials for Ichiro Aria are: IA
Suggested username: ichiro_aria
```

## Getting Started

### Prerequisites

- Java Development Kit (JDK)
- A Java-compatible IDE or terminal

### Compile and Run

The source file is named `MainStrings.java`.

1. Clone or download the repository.
2. Open a terminal in the directory containing `MainStrings.java`.
3. Compile the program:

   ```bash
   javac MainStrings.java
   ```

4. Run the application:

   ```bash
   java MainStrings
   ```

5. Enter three names and select one of the displayed combinations.

## Project Structure

```text
MainStringsJava/
├── MainStrings.java
└── README.md
```

## Limitations

- The program expects each entered name to be a single word.
- Names containing spaces may produce unexpected initials or usernames because the selected combination is split using spaces.
- Non-numeric menu input may cause an input exception.
- Invalid numeric choices are rejected, and the program exits rather than asking the user to try again.
- Username availability and uniqueness are not checked.
- The suggested username is not registered or saved anywhere.
- The generated combinations are ordered, so `Ichiro Aria` and `Aria Ichiro` count as separate options.

## Possible Improvements

- Validate names and handle empty input.
- Support names containing spaces.
- Handle non-numeric menu choices gracefully.
- Allow the user to retry after an invalid selection.
- Remove unwanted extra spaces and standardize username formatting.
- Check for duplicate names before generating combinations.
- Allow the user to copy or save the selected username.

## Learning Objectives

This project demonstrates Java console input, arrays, nested loops, conditional statements, string concatenation, `split()`, `toLowerCase()`, and character access with `charAt()`.

## Author

**Ichiro Yamazaki**

Repository: https://github.com/ichiroyamazaki/MainStringsJava
