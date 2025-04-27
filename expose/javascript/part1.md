1. Line 9 prints out 20
2. Line 13 prints out 20
3. You should not use var as the scope declaration can cause many issues. Declaring in function scope means that the result variable is still accessible even outside of the if block which can cause overwrite and naming issues.
4. Line 9 prints out 20
5. Line 13 returns an out-of-scope error. This error is expected since the result variable is declared with let inside the if block. This means that after the if block closes, result is no longer accessible which is why line 13 throws an error when it tries to access result.
6. Line 9 returns an error as the program attempts to modify the contents of result although it is declared as const. 
7. Since the program threw an error on Line 9, Line 13 does not run.