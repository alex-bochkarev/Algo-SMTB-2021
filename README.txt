             ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
              SMTB-2021 COURSE: A GLIMPSE INTO ALGORITHMS

              Alexey Bochkarev (www.bochkarev.io/contact)
             ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━





[ ∑ ] Summary
═════════════

  *Course point:* To discuss some very basic theoretical concepts from
   Computer Science, heavily relying on numerical illustrations in
   Python. We will discuss what does it mean if someone says the problem
   is "hard" ("NP-hard"? What's the difference?), what are algorithms,
   data structures, and what kind of their properties we might be
   interested in. E.g., whether an algorithm is doing the right thing
   (and how to check it), how fast it runs (how to measure it and "what
   is this O(·) I keep seeing in the papers, exactly?"), and so on.
   Finally: how useful it all is for you if you are not a computer
   scientist, and only write the code from time to time, or even mostly
   using existing programs? (A spoiler: might be very useful!) However,
   we will *not* be learning to write computer programs technically. The
   main purpose is to find a sweet spot between theory and practice to
   equip the interested student with key ideas relevant to a practice of
   (thoughtful) programming, and, perhaps, inspire to take a university
   course in CS.

  (This course is based on my two-hour [lecture] for SMTB-2020.)

  *Timeframe:* Four classes, 50 minutes each. No mandatory home
   assignments.

  *Prerequisites:* interest in algorithms. No serious programming
   background is assumed, but you are expected to be willing to design
   algorithms (pen and paper is OK), and read code in Python (think:
   descriptions is plain English). However, any programming background
   might make the learning way more fun in this course. Ideally, you
   would need to be able to run and experiment with the examples
   yourself.

  *Tech needed:* having a working python (preferably `python3')
   installation locally along with Jupyter Notebook might help. However,
   you will be OK using [Google Colab] (in which case you will need just
   a web browser and a free Google account).

  This repository will be updated with the current materials as the
  course unfolds, so come back to check it out! Tentative course outline
  is as follows.


[lecture] <https://github.com/alex-bochkarev/SMTB-Algo>

[Google Colab] <https://colab.research.google.com>


Course outline
══════════════

Topic 1: Algorithms (of course, sorting example)
────────────────────────────────────────────────

  • What is an algorithm (vs. a computer program).
  • Key properties: correctness, time, and space requirements (without
    details)
  • Several examples of sorting algorithms:
    ⁃ selection sort
    ⁃ bubble sort
    ⁃ maybe, something else :)

  • Correctness and testing.
  • A word on algorithmic *frameworks* / "types" of algorithms: greedy,
    D&C, randomized, brute-force, DP, …

  📔 *Notebook:* [(ipynb)] [(nbviewer)]


[(ipynb)] <./T1-2-Algorithms.ipynb>

[(nbviewer)]
<https://nbviewer.jupyter.org/github/alex-bochkarev/Algo-SMTB-2021/blob/main/T1-2-Algorithms.ipynb>


👉 Topic 2: How to measure runtime properly? Asymptotics.
─────────────────────────────────────────────────────────

  • Merge sort
  • Comparison of runtimes for different algorithms (random tests)
  • Problems: (1) scaling, and (2) special inputs. So:
    ⁃ Worst case, average, and best case runtimes.
    ⁃ Asymptotic runtime: the magic O(·), Ω(·), etc.
  • "hard" problems. Exact algorithms vs. heuristics.

  📔 *Notebook:* (same as the previous one)


Topic 3: Dynamic Programming and Needleman–Wunsch algo
──────────────────────────────────────────────────────

  • Coins/change problem (having N types of coins, how to make C
    cents?). Ideas:
    ⁃ greedy algorithm (not always optimal, though)
    ⁃ exhaustive search (slow)
    ⁃ DP – the magic :)
  • The big topic: Sequence alignments — Needleman–Wunsch algorithm.

  📔 *Notebook:* [(ipynb)]


[(ipynb)] <./T3-DP-and-Needleman-Wunsch.ipynb>


Topic 4: Data structures and conclusion
───────────────────────────────────────

  • DS: abstract descriptions of data types (think: API+key parameters)
  • Example: array vs. linked list and appending an element.
  • A concept of amortized runtime
  • further reading (useful books / courses)

  📔 *Notebook:* [(ipynb)]


[(ipynb)] <./T4-DataStructures.ipynb>


Further reading / learning
══════════════════════════

  This is the most important part of the course 😃.

  First things first: maybe a university course in CS?


🌐 Online reference
───────────────────

  • GeeksForGeeks (e.g., [merge sort]), Wikipedia, etc. are quite good,
    sometimes.
  • Docs for specific libraries (e.g., see sorting in [numpy docs])


[merge sort] <https://www.geeksforgeeks.org/merge-sort/>

[numpy docs]
<https://numpy.org/doc/stable/reference/generated/numpy.sort.html>


📖 Books
────────

  There are some good "light" introductory textbooks:
  ⁃ Skiena "Algorithm Design Manual"
  ⁃ Kleinberg and Tardos, "Algorithm Design"
  There are some more classic CS textbooks, which I would **not**
  recommend as an intro (you can google yourself as needed – e.g., CLRS
  or Sedgewick's "Algorithms" books). That would be a little too dense
  for starters.

  Finally, there is **the ultimate thing:** "The Art of Computer
  Programming", aka TAOCP. It is very dense and very "mathy" (and uses a
  hypothetical [assembly language]!), but covers *a lot*, as detailed as
  it gets. If you don't know how to solve some algorithmic problem,
  chances are TAOCP discusses it, comprises it as an exercise, or at the
  very least provides some inspiration. (Also, try googling "is TAOCP
  worth reading" or check an [HN question] :) )


[assembly language] <https://en.wikipedia.org/wiki/Assembly_language>

[HN question] <https://news.ycombinator.com/item?id=10897460>


🎓 Online courses
─────────────────

  If you feel the need to practice, there are some good online courses
  out there. For example, Coursera:
  ⁃ [Analysis of Algorithms] from Princeton (by Dr. Sedgewick) – some
    practice in Java.
  ⁃ [Algorithms specialization] from Stanford – this one might be
    math-heavy and more on the theoretical side.
  ⁃ there is more – google, check reviews, try several, pick the one
    that you like (Stepik, Udemy, etc. etc.).
  ⁃ might be a good idea to start one, go through the intro (but not
    necessarily finish).

  If you feel like watching some videos, or would like to check out a
  specific thing, I might recommend the MiT OCW [6.006 Intro to
  Algorithms] course.


[Analysis of Algorithms]
<https://www.coursera.org/learn/analysis-of-algorithms>

[Algorithms specialization]
<https://www.coursera.org/specializations/algorithms>

[6.006 Intro to Algorithms]
<https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-006-introduction-to-algorithms-fall-2011/>