## Entry 1
* The issue encountered: I did not add the full arguments to the dfs function and only had vector<vector<int>>& parent_r and vector<vector<int>>& parent_c 

* Error messages or symptoms: I caught this before any error messages came up as I read further into the code provided. If there was an error message, it would say something about not enough arguments. 

* Attempts made: After reading further into the code, I realized there needed to be more arguments than just the ones I put, so I added the rest that fit with how the function was called later on

* Final resolution: I added all arguments needed so the arguments looked like: int ent_r, int ent_c, const vector<vector<int> >& maze, vector<vector<bool> >& visited, vector<vector<int> >& parent_r, vector<vector<int> >& parent_c, int exit_r, int exit_c

## Entry 2
* The issue encountered: There were many red underlines under code that looked like ">>"

* Error messages or symptoms: "Clangd: A space is required between consecutive right angle brackets (use '> >')." Which I think meant that the code was confusing the compiler

* Attempts made: I found where each red underline was and started to add a space between each >.

* Final resolution: I added a space between the two >. This got rid of the error and made the code look a lot cleaner. 

## Entry 3
* The issue encountered: I realized that for the first two arguments of dfs, I was using ent_r and ent_c, which made sense for the first call, but then after r and c move, they are not at the entrance anymore.

* Error messages or symptoms: There was not really an error, just an incorrect name for two parameters. Once dfs is called recursively, it would not make sense for r and c to be called ent_r and ent_c.

* Attempts made: I decided to go with changing those arguments to just r and c

* Final resolution: I changed the arguments ent_r and ent_c to just r and c.

## Entry 4
* The issue encountered: used <= in the for loop instead of <, which would lead to an error.

* Error messages or symptoms: I caught the error before actually running the code. I originally had i <= 4, which would have the for loop looking through 5 directions, even though there are only 4. So the error message would have been an out-of-bounds error, I believe.

* Attempts made: This was a simple fix; I just had to remove the = sign.

* Final resolution: Once I removed the = sign the loop would go through four indexes (0,1,2,3) instead of 5 (0,1,2,3,4).

## Entry 5
* The issue encountered: After fixing most of the errors, there were 3 left, and they were two different types.

* Error messages or symptoms: "Non-aggregate type 'pair<int, int>' cannot be initialized with an initializer list" and "Clangd: Expected expression." 

* Attempts made: These were errors in part of the code that said do not modify, but the code would not run without these errors being fixed. I had no idea how to fix these errors, so I had to look up the solutions to these errors. 

* Final resolution: for the first error, I just had to add "make_pair," and the red line went away. For the second and third errors, I had to do the same thing, but it was a different error message.

## Entry 6
* The issue encountered:

* Error messages or symptoms:

* Attempts made:

* Final resolution: