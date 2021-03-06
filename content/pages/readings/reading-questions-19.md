---
content_type: page
description: This section provides an interactive answer checker for the reading questions
  associated with an assigned reading.
learning_resource_types:
- Readings
ocw_type: CourseSection
parent_title: Readings
parent_type: CourseSection
parent_uid: 579c055a-ccb4-eb7e-bb6b-f294146b45a5
title: Reading Questions 19
uid: e77a7bd7-1572-00e9-6207-bb9280d247ac
video_files:
  video_thumbnail_file: null
video_metadata:
  youtube_id: null
---

Reading Questions Answer Checker
--------------------------------

To check your answers put them in the appropriate box and click the 'Check' button. Every checker box can do arithmetic and calculate standard functions (see {{% resource_link 758ceee0-d290-5d7c-5072-7d458581a3b3 "calculator help" %}}). If you give decimal answers, give them to at least 3 decimal places.

As you work you should have pencil and paper handy for calculations and thinking!

Note: some questions ask for a formula. For the checker we ask you to plug a value into the formula. For your pset you still need to give the whole formula.

//DEBUG PARAMETERS //Because we don't show solutions for pset checkers we use //this to give a showanswer button during the debugging phase var debugans = undefined; //release //var debugans = kDebugAnswer; //debug problemNumber = 0; wl("\<h3>Calculator\</h3>"); writecalculator("psetcheckcalcid", "Calculate"); whr(kdivcol,kdivwid);

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = emphtext("We suggest you use R to do the computations for this problem."); wl(s); wl(kp); s = "Suppose we have the following table of counts for the outcomes 0-6."; wl(s); wl(kp); writetable(\[\['Outcome', 0, 1, 2, 3, 4, 5, 6\], \['Observed','5','11','13','7','2','1','1'\]\], "class='basicborder'", "class='basiccells'", "class='k'", 2); wl(kp); s = "We hypothesize that the data is drawn from a binomial(6, 0.4) distribution."; wl(s); wl(kp); s = "(a) Compute the likelihood ratio statistic $G$."; wl(s); wl(kbr); partName = problemNumber + " (a)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 11.89567, buttonLabel, 0.002, kuseCorrectVal); wl(kp); s = "(b) Compute the Pearson chi square statistic $X^2$."; wl(s); wl(kbr); partName = problemNumber + " (b)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 15.1242, buttonLabel, 0.002, kuseCorrectVal); wl(kp); s = "(c) How many degrees of freedom are there in the chi square null distribution?"; wl(s); wl(kbr); partName = problemNumber + " (c)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 6, buttonLabel, 0.001, kuseCorrectVal); wl(kp); s = "(d) Compute the $p$-value (based on the $G$-statistic)."; wl(s); wl(kbr); partName = problemNumber + " (d)"; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; writeNumericBox(partName+"id", 0.064337, buttonLabel, 0.002, kuseCorrectVal); wl(kp); whr(kdivcol,kdivwid);