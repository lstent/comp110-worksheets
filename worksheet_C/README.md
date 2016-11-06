- (a) The algorithm checks list i and j for duplicates, if a duplicate is found it shows the word true, if not show false
- (b) For each item in list i it is being compared to every item before and including that same point in list j, e.g. list item 2 in i is being compared to list item 0,1,2 in j, written as n*n or n^2
- (c) If line 4 is changed it still compares every item in list i and j for duplicates
- (d) The algrorithm runs twice as fast because instead of comparing one item in list i against every item of list j, it only compares list numbers j below the list number i e.g. if the list number in i is 2 it only compares list number in j before 2
- (e) I think the algorithm cannot be counted as quadratic anymore as the numbers are no longer being copared to its equivalent in list j therefore the equation is no longer n^2
- (f) Python's built-in source fuction is logarithmic written as O(n log n) ref: (2015) Timecomplexity [online] Available at: https://wiki.python.org/moin/TimeComplexity [Accessed 21st October 2016]
- (g) The algorithm is working in a linear complexity as it just compares the list item above to the current list item, therefor in big O notation it is written as O(n)
- (h) In my opinion the linear algorithm would be faster as it quickly sorts itself and then only has to check the before list item for duplicates instead of going back over the whole of the previous items to check for duplicates like the quadratic algorithm does
- (i) A programmer may choose a slower algorithm over a faster one as many faster algorithms depend of the use of sorting, therefore the list may not be already sorted which may take extra time to sort or the programmer may not know how to sort therefore it would just be faster to use a slower algorithm