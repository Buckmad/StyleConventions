# Style Conventions for Roblox-TS
Buckmad Style Conventions and our style agreements for Roblox Typescript.

This is a convention or really a guide discussed by me and Weary. The goal is to deliver readable code and save us a great deal from eye fatigue or headaches.

We don't believe in forcing it on other developers, but it is a duty in our team to follow this so there are no surprises when it comes to syntax and naming. We don't even need a guide, lol. We already can decide the exceptions for ourselves when needed.

## Variables and Constants
- When naming variables or constants, ALWAYS use Camelcase. Avoid SCREAMING CASE AT ALL COST. YOU DON'T LIKE THIS. DO YOU? Snakecase also adds visual clutter.

Good:
```diff
+ const brokeBack: boolean;
```
Bad:
```diff
- const BrokeBack: boolean;
```

## Functions
- When calling functions with three or more arguments, you should write them on separate lines.

Good:
```diff
+ print(
+   "Apple",
+   "Banana",
+   "Orange"
+ );
```
Bad:
```diff
+ print("Apple", "Banana", "Orange");
```
- When writing callbacks, keep them on (a) separate line(s).

Good:
```diff
+ Connect(
+   () => {
+     print("Good.");
+   }
+ );
```
Bad:
```diff
- Connect(() => {
-   print("Bad.");
- });
```
---
- When writing functions, write it like you're writing a function in C by giving the brackets their own lines.

Good:
```diff
+ function add(a : number, b : number)
+ {
+   return a + b;
+ }
```
Bad:
```diff
- function add(a : number, b : number) {
-   return a + b;
- }
```

## Mindset

If you've studied this, but you're still wondering, "what if there are more conventions that hasn't been dictated by the guide but is a debatable matter?" Just think about this: avoid cramming your code. It's less about density or guerrilla warfare. It's more about spacing out, readability, and operation.
