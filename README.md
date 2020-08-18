# Algorithm-Analysis
Used for LaunchCode Studios 

Studio for 1.5
  1. Given the un-reduced big-O value, calculate the reduced value.
    a: O(1)
    b: O(n)
    c: O(n^2)
    d: O(log n)
    
  2. For each of the following algorithms, calculate the big-O value. Be sure to specify which value n refers to.
    a: O(n)
    b: O(n^2)
    c: O(n)
  
  3. Suppose you have an array of Customer objects, sorted in alphabetical order by last name.
      For each of the following tasks, determine the run time in terms of big-O.
     a: O(n)
     b: O(n)
     c: O(n)
     d: O(n)
  
  4. Now suppose that you have a dictionary of customer objects, where the keys are letters and the values are
      arrays storing all customers with last name beginning with that letter. 
        For example, if our dictionary is customers then customers["A"] is an array of all customers with last name ending with “A”. 
        Within each array, the customer objects are not sorted in any way.
       
        a: O(n)
        b: O(n)
        c: O(1)
        d: O(n)
        


STUDIO 2.5 (UNORDERED)
"*" indicate change

       Beginning tree:                  
                    ____8
                   /     \
                 _3__     10
                /    \      \
                1     6      14
                \    / \
                4   7   13

       Insert 9:

            ____8
           /      \
         _3__      10
        /    \     /  \
        1     6   9*    14
        \    / \
        4   7   13

       Remove 4:
                    ____8
                 /       \
                _3__       10
               /    \     /  \
              1*      6   9    14
                     / \
                    7   13
      Insert 12:
                  ___8___
               /         \
              _3__        10
             /    \     /   \
            1      6   9    14
                  / \       / 
                 7   13   12*

       Remove 6:
                  ___8___
               /         \
              _3__         10
             /    \       /   \
            1      7*    9     14
                    \         / 
                     13      12

STUDIO 2.5 (ORDERED)
"*" indicate change

     Insert 9:

              ____8
             /      \
           _3__       10
          /    \     /  \
          1     6   9*    14
          \      \        /
           4      7     13
            
    Remove 4:

              ____8
             /      \
           _3__       10
          /    \     /   \
          1*    6   9     14
                 \        /
                  7     13    
                    
                    
    Insert 12:

              ____8
             /      \
           _3__       10
          /    \     /   \
          1     6   9     14
                 \        /
                  7     13
                        /
                      12*
                        
                        
                        
      Remove 6:

              ____8
             /      \
           _3__       10
          /    \      /  \
          1     7*    9    14
                          /
                        13
                        /
                      12
