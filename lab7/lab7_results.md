# Names: Careney Mchau & Andy Gutierrez
# Lab: lab7 (RAG for Code with UniXcoder)
# Date: 12/03/2025

---

**Task 2.2**
1. The discrimination scores tell us that UniXcoder is better than the generic discrimination. 

**Task 2.3**
1. Yes, it recognizes that it is the same even though it might have some small changes such as variable name changes.
2. It handles pretty well, we know this by looking at the similarity scores and with_typing is at the top of the list with 0.9538, so in the case of renaming the variables or with typing UniXcoder does a great job at recognizing that it is functionally the same.  

**Task 2.4**
1. Yes, when running this code when the number of changes increase the similarity decreases, but still has a similarity percentage in the low nineties.
2. It recognizes that only the variable name is changed and the rest of the code is the same. It has the lowest similarity percentage, so it must think that the variable name change is significant. Maybe the model thinks that changing the variable name is the closest that it gets to changing the purpose of the function, unlike before where we change an operator that shifts the logic a tiny bit but is still checking age. 

**Task 3.2**
1. Yes, different phrasings of the same question did retrieve the same function even though the distances was different for each one.

**Task 4.2**
1. We think that use cases query types work best with UniXCoder as they had the smallest average distance relative to the other kind of queries.
2. UniXCoder handles vague queries rather poorly. It does better at handling the specific functions because we are giving it more of a platform to help itself out, but I think it is rather weird how for every vague and specific query, query_database is still the first function that shows up in every list. We noticed that the distances for the vague queries are almost identical while the specifc queries have different distances. 