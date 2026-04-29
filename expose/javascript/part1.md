1. values added:  20, did not return an error
2. final result:  20, did not return an error
3. I should not use var because it doesn’t respect block scope (like inside loops or if statements), and instead uses function-level scope. Unlike let, var allows redeclarations. Most importantly, in my opinion, it’s also hoisted, which can lead to confusing behavior if I am not careful or organized with my variables (which I am still working on!).
4. values added:  20, did not return an error
5. Returns an error (ReferenceError) saying result is not defined in line 13. It returns an error because the result variable was declared using a let. Unlike var, lets respect block scope and therefore, its almost like result does not exist outside of the if block (which is also why line 9 printed) 
6. Returns an error (TypeError: Assignment to constant variable.). This is because variables declared with const cannot be changed once initialized. The code attempts to change the variable result (declared with const) in line 7. The program stops at this line and does not continue. 
7. Program never gets to this line at all. Same reason as #6. 