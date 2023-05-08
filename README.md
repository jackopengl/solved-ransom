Download Link: https://assignmentchef.com/product/solved-ransom
<br>
<a href="https://www.youtube.com/playlist?list=PLhOuww6rJJNMxWhckg7FO4cEx57WgHbd" rel="nofollow">https://www.youtube.com/playlist?list=PLhOuww6rJJNMxWhckg7FO4cEx57WgHbd</a>_

Write a program that will randomly capitalize the letters in a given piece of text a la a ransom note. The text may be provided on the command line:

<pre><code>$ ./ransom.py 'The quick brown fox jumps over the lazy dog.'THe qUICk BrOWn fOX jumPS OVEr THE LAzy DOg.</code></pre>

Or with a file:

<pre><code>$ ./ransom.py ../inputs/fox.txtTHE QUicK BRown fox JuMPS OVER THe laZY dog.</code></pre>

Given no arguments, the program should print a brief usage:

<pre><code>$ ./ransom.pyusage: ransom.py [-h] [-s int] strransom.py: error: the following arguments are required: str</code></pre>

The program should accept a <code>-s</code> or <code>--seed</code> option to use as a random seed to ensure reproducibility:

<pre><code>$ ./ransom.py -s 1 ../inputs/fox.txtthE QUICk BrOWn Fox jumpS OveR tHe LAzY dOg.</code></pre>

It should respond to <code>-h</code> and <code>--help</code> with a longer usage:

<pre><code>$ ./ransom.py -husage: ransom.py [-h] [-s int] strRansom Notepositional arguments:  str                 Input text or fileoptional arguments:  -h, --help          show this help message and exit  -s int, --seed int  Random seed (default: None)</code></pre>

Run the test suite to ensure your program is correct:

<pre><code>$ make testpytest -xv test.py============================= test session starts ==============================...collected 6 itemstest.py::test_exists PASSED                                              [ 16%]test.py::test_usage PASSED                                               [ 33%]test.py::test_text1 PASSED                                               [ 50%]test.py::test_text2 PASSED                                               [ 66%]test.py::test_file1 PASSED                                               [ 83%]test.py::test_file2 PASSED                                               [100%]============================== 6 passed in 0.62s ===============================</code></pre>