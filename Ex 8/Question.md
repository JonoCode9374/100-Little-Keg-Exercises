# Reversing and Shifting

Stack manipulation is a very important part of Keg, as everything within Keg is done to the main stack. Throughout this exercise you will learn about:

- The `"` command (Right shift)
- The `'` command (Left shift)
- Reversing the stack (the `^` command)

## The Challenge

I want you to write a program that:

- Takes a series of characters as input (use `?` for this) and,
- Then takes another letter (we'll call this `instruction`) as input (once again, use `?`) and,
- Takes a single integer (we'll call this `times`) as the last input (`¿`) and then,
- If `instruction` is equal to the letter `R`:
-	Reverse the stack `times` times. (Hint: for loops are needed)
- Otherwise, if `instruction` is equal to the letter `l`:
-	Shift the stack left `times` times
- Otherwise:
-	Shift the stack right `times` times

Here are some examples of how your program should run:

| Input | Instruction | Times |
|:----------|:----------|:----------|
|Howdy!   | R    | 1    |

Output:

	!ydwoH

[Input as formatted on TIO](https://tio.run/##y05N/w8EHvnlKZWKXEFchgA "Keg – Try It Online")

---

| Input | Instruction | Times |
|:----------|:----------|:----------|
|elloH | r    | 1    |

Output:

	Hello

[Input as formatted on TIO](https://tio.run/##y05N/w8EqTk5@R5cOVyGAA "Keg – Try It Online")

---

| Input | Instruction | Times |
|:----------|:----------|:----------|
|tedShif | l    | 3    |


Output:

	Shifted

[Input as formatted on TIO](https://tio.run/##y05N/w8EJakpwRmZaVw5XCYA "Keg – Try It Online")

---

| Input | Instruction | Times |
|:----------|:----------|:----------|
|sn't it?Amazing, i | r    | 8    |

Output:

	Amazing, isn't it?

[Try it online!](https://tio.run/##y05N/w8ExXnqJQqZJfaOuYlVmXnpOgqZXEVcFgA "Keg – Try It Online")

---

You will need to know these things:

- You will most likely need a loop at the end of your program to print the contents of the stack as they should appear. In other words, you'll most likely need to append `(,)` if you don't reverse the first input after taking it.
- Touching on the above point, the `?` takes a line of input reversed, meaning you may need to reverse the input using `^`.
- A little recap: `¿` takes input as an integer
- All instructions are case sensitive. In other words only an input of `R` should reverse the stack, not `r`.


