# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.


To verify this claim I would time how long it takes to sort lists of increase size and take note of how the time it takes grows. If it grows faster than O(n) I would know that they are lying. However, technically they could sacrifice practical speed by making certain outputs take longer than others artifically. So that it grows linearly. If they do this for large enough sizes of n I might not be able to test high enough to prove them wrong.

From a theoretical point of view however, since we know that from the analysis of the general sorting problem we covered in class, asymptotically it can not be faster than O(n log n). Therefore even if they try to fake results, there exists a $n_0$ and $c$ that show their algorithm is in O(n log n) or slower. Meaning it's impossible for a comparison based sorting algorithm to have O(n) complexity for arbitrary elements.


I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

