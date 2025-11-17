# STEPS.md – Steps Taken to Complete the Git Assignment  
Author: Adriana Barcenas

---

## Commit 0
1. git init
2. touch README.md
3. echo "CSCI 3323 – Fall 2025 <br> Git Assignment <br> Adriana Barcenas" > README.md
4. git add README.md
5. git commit -m "Commit 0: Initial commit"

## Commit 1
6. echo "Line for Commit 1" >> notes.md
7. git add notes.md
8. git commit -m "Commit 1: Added notes.md"

## Commit 2
9. git checkout -b bug-fix
10. echo "Fix note A" >> notes.md
11. git add notes.md
12. git commit -m "Commit 2: Bug-fix branch commit"

## Commit 3
13. git checkout master
14. echo "Master update" >> notes.md
15. git add notes.md
16. git commit -m "Commit 3: Update on master"

## Commit 4
17. git checkout -b bug-fix-experimental
18. echo "Experimental change" >> notes.md
19. git add notes.md
20. git commit -m "Commit 4: Experimental branch update"

## Commit 5
21. git checkout bug-fix
22. echo "Bug fix B" >> notes.md
23. git add notes.md
24. git commit -m "Commit 5: Additional bug-fix work"

## Commit 6 (Merge bug-fix into master)
25. git checkout master
26. git merge bug-fix
27. (If conflict appears, resolve, then:)
28. git add notes.md
29. git commit -m "Commit 6: Merge bug-fix into master"

## Commit 7
30. git checkout bug-fix-experimental
31. echo "More experimental work" >> notes.md
32. git add notes.md
33. git commit -m "Commit 7: More experimental changes"

## Commit 8
34. git checkout master
35. echo "Master update 2" >> notes.md
36. git add notes.md
37. git commit -m "Commit 8: Another master update"

## Commit 9 (Merge conflict here)
38. git merge bug-fix-experimental
39. (Resolve conflict manually by editing notes.md)
40. git add notes.md
41. git commit -m "Commit 9: Merge bug-fix-experimental into master with conflict resolved"

## Commit 10
42. echo "Commit 10 change" >> notes.md
43. git add notes.md
44. git commit -m "Commit 10: Updating notes"

## Commit 11
45. git checkout bug-fix
46. echo "Commit 11 on bug-fix" >> notes.md
47. git add notes.md
48. git commit -m "Commit 11: More bug fixes"

## Commit 12 (Merge bug-fix into experimental)
49. git checkout bug-fix-experimental
50. git merge bug-fix
51. git add notes.md
52. git commit -m "Commit 12: Merged bug-fix into experimental"

## Commit 13
53. git checkout master
54. echo "Commit 13 change" >> notes.md
55. git add notes.md
56. git commit -m "Commit 13: Master update"

## Commit 14 (Final merge)
57. git merge bug-fix-experimental
58. git add notes.md
59. git commit -m "Commit 14: Final merge to complete graph"

---

# Pushing to GitHub

60. git remote add origin <YOUR URL>
61. git push -u origin master
62. git checkout bug-fix
63. git push -u origin bug-fix
64. git checkout bug-fix-experimental
65. git push -u origin bug-fix-experimental
