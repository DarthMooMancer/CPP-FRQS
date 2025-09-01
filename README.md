# 🌟 C++ Beginner to Intermediate FRQs Practice Set

Welcome!\
This set of FRQs is designed to **gradually challenge you**, introducing **new C++ skills** step-by-step without overwhelming jumps.

Each FRQ includes:

- **Background**
- **Task**
- **Checklist** (what you should know)
- **Example Usage** (without code)
- **Programming Details** (hints for how to structure your solution)

---

## FRQ 1 — Rainfall Grid Analyzer (2D Arrays, Nested Loops)

**Background:**\
Analyze rainfall amounts for different cities over several days.

**Task:**

- Input a 3x4 grid of rainfall data.
- Calculate total rainfall per city.
- Find city with the highest rainfall.
- Calculate average rainfall per day.

**Checklist:**

- 2D arrays
- Nested loops
- `const` parameters

**Example Usage:**

- Input rainfall for 3 cities across 4 days.
- Output total rainfall per city, the highest, and average per day.

**Programming Details:**

- Create a 2D array `rainfall[3][4]`.
- Use a `void inputRainfall(int rainfall[3][4])` function to fill the array.
- Create `int totalRainfallForCity(const int rainfall[3][4], int cityIndex)` to calculate total for one city.
- Use a loop to find the city with the highest total.
- Create `double averageRainfallPerDay(const int rainfall[3][4], int dayIndex)` to get averages per day.
- Emphasize modular design: input, calculation, output functions.

---

## FRQ 2 — Word Length Counter (Strings, Loops)

**Background:**\
Count how many words match a given length.

**Task:**

- Input 5 words.
- Input a target word length.
- Output how many words match that length.

**Checklist:**

- Arrays of strings
- Looping over strings

**Example Usage:**

- Input words: `cat`, `elephant`, `dog`, `fish`, `giraffe`
- Target length: 3
- Output: 2 words ("cat" and "dog")

**Programming Details:**

- Create `void inputWords(string words[], int size)` to input the words.
- Create `int countMatchingLength(const string words[], int size, int targetLength)` to do counting.
- Main function orchestrates input -> processing -> output.
- Keep functions pure (no `cout` inside logic functions).

---

## FRQ 3 — Prime Number Finder (Functions, Math)

**Background:**\
Find all prime numbers up to a given number.

**Task:**

- Input a number `n`.
- Print all prime numbers between 2 and `n`.

**Checklist:**

- Loops
- Function decomposition (`isPrime(int n)`)

**Example Usage:**

- Input: 10
- Output: 2, 3, 5, 7

**Programming Details:**

- Write a `bool isPrime(int n)` function that returns true if n is prime.
- In main, loop from 2 to n, call `isPrime` for each.
- Keep `isPrime` efficient: check divisibility only up to √n.

---

## FRQ 4 — Temperature Tracker v2 (Functions Returning Multiple Values)

**Background:**\
Find both the highest and lowest temperatures in one function.

**Task:**

- Input temperatures for 7 days.
- One function returns both highest and lowest temperatures.

**Checklist:**

- Reference parameters
- Arrays

**Example Usage:**

- Input: [70, 75, 72, 68, 74, 71, 69]
- Output: Highest = 75, Lowest = 68

**Programming Details:**

- Create a `void findHighLow(const int temps[], int size, int& high, int& low)`.
- Pass `high` and `low` by reference.
- Loop through array once to find both values.

---

## FRQ 5 — Tic Tac Toe Board Printer (2D Arrays, Characters)

**Background:**\
Print a Tic-Tac-Toe board.

**Task:**

- Input a 3x3 grid of characters (`X`, `O`, or `_`).
- Display the board neatly.

**Checklist:**

- 2D char arrays
- Nested loops

**Example Usage:**

- Input: [['X','O','*'],['*','X','O'],['O','_','X']]
- Output formatted grid.

**Programming Details:**

- Use `void printBoard(const char board[3][3])`.
- Carefully manage spacing and lines.
- Separate rows with a horizontal line.

---

## FRQ 6 — Summing Diagonals (2D Arrays, Diagonal Logic)

**Background:**\
Sum the diagonals of a square matrix.

**Task:**

- Input a 3x3 matrix of integers.
- Output the sum of primary and secondary diagonals.

**Checklist:**

- Understanding indices
- Functions

**Example Usage:**

- Input matrix and output sums.

**Programming Details:**

- Create two functions: `int sumPrimaryDiagonal(const int matrix[3][3])` and `int sumSecondaryDiagonal(const int matrix[3][3])`.
- Primary: indices (0,0), (1,1), (2,2).
- Secondary: indices (0,2), (1,1), (2,0).

---

## FRQ 7 — Vowel Replacer (Strings, Character Operations)

**Background:**\
Replace all vowels in a string with a given character.

**Task:**

- Input a string and a replacement character.
- Replace each vowel.

**Checklist:**

- String iteration
- Case handling (lower and upper)

**Example Usage:**

- Input: "Hello World", replacement: '*'
- Output: "H*ll* W*rld"

**Programming Details:**

- Create `void replaceVowels(string& text, char replacement)`.
- Helper function `bool isVowel(char c)`.
- Modify string in-place.
- Handle both lowercase and uppercase vowels.

---

## FRQ 8 — Histogram Maker (Arrays, Basic Visualization)

**Background:**\
Create a simple histogram.

**Task:**

- Input 5 numbers between 1 and 10.
- For each number, print that many `*`.

**Checklist:**

- Arrays
- Loops

**Example Usage:**

- Input: [3, 5, 7, 2, 4]
- Output: corresponding `*` per line.

**Programming Details:**

- Use `void printHistogram(const int numbers[], int size)`.
- Nested loops: outer loop over numbers, inner loop to print `*`s.
- Validate that input numbers are within 1 to 10.

---

## FRQ 9 — Shift Array Elements (Array Manipulation)

**Background:**\
Shift elements to the right, wrapping the last to the first.

**Task:**

- Input 6 numbers.
- Shift all elements one position to the right.

**Checklist:**

- Careful index management

**Example Usage:**

- Input: [1, 2, 3, 4, 5, 6]
- Output: [6, 1, 2, 3, 4, 5]

**Programming Details:**

- Create `void shiftRight(int arr[], int size)`.
- Save last element before shifting.
- Shift from end toward start (backward).
- Set arr[0] to saved last element.

---

## FRQ 10 — Grade Statistics (Multi-Function, Arrays)

**Background:**\
Analyze a set of grades.

**Task:**

- Input 8 grades.
- Calculate:
  - Average
  - Highest
  - Lowest
  - Number of As

**Checklist:**

- Arrays
- Function separation

**Example Usage:**

- Input: [91, 85, 78, 92, 88, 95, 67, 80]
- Output statistics.

**Programming Details:**

- Create separate functions:
  - `double calculateAverage(const int grades[], int size)`
  - `int findHighest(const int grades[], int size)`
  - `int findLowest(const int grades[], int size)`
  - `int countAs(const int grades[], int size)` (A >= 90)
- Main function calls each and outputs results.

---

## FRQ 11 — Budget Planner (Multiple Arrays, Matching Data)

**Background:**\
Match monthly income and expenses.

**Task:**

- Input income and expenses for 6 months.
- Output monthly profit/loss and total.

**Checklist:**

- Parallel arrays
- Multiple loops

**Example Usage:**

- Input income and expenses arrays.
- Output profits per month and overall profit.

**Programming Details:**

- Two arrays: `income[6]`, `expenses[6]`.
- Create `void calculateMonthlyProfits(const int income[], const int expenses[], int profits[], int size)`.
- Sum the profits array for total.
- Separate output formatting function: `void printProfits(const int profits[], int size)`.

---

# 📚 Summary of Skills Covered

| Concept                     | FRQs     |
| --------------------------- | -------- |
| 2D Arrays                   | 1, 5, 6  |
| Nested Loops                | 1, 5     |
| Function Decomposition      | 3, 4, 10 |
| String Manipulation         | 2, 7     |
| Basic Graphics (Histograms) | 8        |
| Array Shifting              | 9        |
| Matching Parallel Data      | 11       |
| Reference Parameters        | 4        |

---

# 🏃‍♂️ How to Proceed

- Start with **FRQ 1**.
- After solving, **review**: correctness, efficiency, and clarity.
- Use the programming structure hints to guide your solution architecture.
- Keep building as concepts escalate.

---

Good luck! Keep learning ✨
