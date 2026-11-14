# Java Operator Precedence Example

A small Java program that evaluates an arithmetic expression to show **operator precedence** and **integer division**.

## What It Demonstrates

```java
int x = 29 % 6 * 11 / 3 + 8 - 27 / 8;
```

- `%`, `*`, and `/` have higher precedence than `+` and `-`
- Operators of the same precedence are evaluated from left to right
- Dividing two `int` values discards the decimal part

## Step-by-Step Evaluation

| Step | Expression | Result |
|------|------------|--------|
| 1 | `29 % 6` | 5 |
| 2 | `5 * 11` | 55 |
| 3 | `55 / 3` | 18 (integer division, 18.33 is cut to 18) |
| 4 | `27 / 8` | 3 (integer division, 3.375 is cut to 3) |
| 5 | `18 + 8` | 26 |
| 6 | `26 - 3` | 23 |

## Output

```
The value of x is: 23
```

## Requirements

- Java Development Kit (JDK) 8 or higher

## Getting Started

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
javac X.java
java X
```

## Try It Yourself

- Add parentheses, such as `29 % (6 * 11) / 3`, and see how the result changes
- Change the numbers to `double` values and compare the results

## Project Structure

```
.
├── X.java
└── README.md
```

## Next Steps

- Add your own expressions and predict the output before running
- Learn the full precedence table for Java operators
