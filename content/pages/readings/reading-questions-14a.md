---
content_type: page
parent_title: Readings
parent_uid: 579c055a-ccb4-eb7e-bb6b-f294146b45a5
title: Reading Questions 14a and 14b
uid: 5316874c-718e-ec46-e3f3-7e424cdee94b
---

Reading Questions Answer Checker
--------------------------------

To check your answers put them in the appropriate box and click the 'Check' button. Every checker box can do arithmetic and calculate standard functions (see [calculator help]({{< baseurl >}}/pages/assignments/calculator-help)). If you give decimal answers, give them to at least 3 decimal places.

As you work you should have pencil and paper handy for calculations and thinking!

Note: some questions ask for a formula. For the checker we ask you to plug a value into the formula. For your pset you still need to give the whole formula.

//DEBUG PARAMETERS //Because we don't show solutions for pset checkers we use //this to give a showanswer button during the debugging phase var debugans = undefined; //release //var debugans = kDebugAnswer; //debug problemNumber = 0; wl("<h3>Calculator</h3>"); writecalculator("psetcheckcalcid", "Calculate"); whr(kdivcol,kdivwid);

//Problem 1 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "Data $x$ follows a binomial(12, $&theta;$) distribution. To begin with you have no idea about $&theta;$ so you choose a flat prior. You run and experiment and find $x=3$. What is the posterior distribution?"; wl(s); wl(kbr) partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "Beta(4, 10)"; var answerArray = \["binomial(12, 3)","binomial(15, $&theta;$)","Beta(3, 12)", correct\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);

//Problem 2 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "True or false: Setting the prior probability of a hypothesis to 0 means that no amount of data will make the posterior probability of that hypothesis the maximum over all hypotheses."; wl(s); wl(kbr); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "True"; var answerArray = \[correct,"False"\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);

//Problem 3 problemNumber++; wl(problemheader(problemNumber)); var s; var partName, problemName, buttonLabel, answerArray, correct; s = "True or false: It is okay to have a prior that depends on more than one unknown parameter."; wl(s); wl(kbr); partName = problemNumber; problemName = "prob" + partName; buttonLabel = "Check problem " + partName; correct = "True"; var answerArray = \[correct,"False"\]; writeMultipleChoiceRadioGroup(answerArray, problemName, correct, buttonLabel); wl(kp); whr(kdivcol,kdivwid);