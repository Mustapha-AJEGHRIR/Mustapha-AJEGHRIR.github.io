---
layout: page
title: Inv-MR-sort and Inv-NCS
description: Decision systems for sorting and classification
img: assets/img/demo_illuin.gif
importance: 5
category: work
selected: true
---


The github repository : 
<div style= "text-align: center;">
    <div class="github-card" data-github="Mustapha-AJEGHRIR"  data-repo="projet_sys_decision" data-height="" data-theme=""></div>
    <script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
</div>


In this project we were a team of 3 students : 
- Mustapha Ajeghrir
- Nouamane Tazi
- Asmae Khald


The goal of this project was to create a decision system for sorting and classification by using the concepts of MR-sort and NCS.

## Simple example :
Imagine you are the responsible person for recruiting students in a prestigious university, your goal is to determine the right criteria of admission (to decide someone should enter or not). Let's consider the following example :

<!-- table 3x3 -->
<table class="table table-bordered">
  <thead>
    <tr>
      <th scope="col">Criteria</th>
      <th scope="col">Mathematics</th>
      <th scope="col">Physics</th>
      <th scope="col">Chemistry</th>
      <th scope="col">Language 1</th>
      <th scope="col">Language 2</th>
      <th scope="col">Results</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Student 1</th>
      <td>15</td>
      <td>15</td>
      <td>13</td>
      <td>10</td>
      <td>12</td>
      <td>Good</td>
    </tr>
    <tr>
      <th scope="row">Student 2</th>
      <td>18</td>
      <td>14</td>
      <td>18</td>
      <td>12</td>
      <td>13</td>
      <td>Very Good</td>
    </tr>
    <tr>
      <th scope="row">Student 3</th>
      <td>6</td>
      <td>11</td>
      <td>12</td>
      <td>10</td>
      <td>9</td>
      <td>Bad</td>
    </tr>
    <tr>
      <th scope="row">Student 4</th>
      <td>5</td>
      <td>7</td>
      <td>12</td>
      <td>13</td>
      <td>4</td>
      <td>Very Bad</td>
    </tr>
  </tbody>
</table>

The `Results` column is the result we want to predict for each student. Let’s say, we can only know this label after few years after the entry in the university. So, it is better to know in prior which student will have good results.

## MR-sort :
To make it simple (otherwise, take a look at the report in the bottom of this page) : MR-sort is using a weighted sum based on accepted criteria. Let's say we have 5 criteria weighted $$0.2$$ each, and an acceptance threshold of $$0.7$$. In this case the student should get good results in at least $$4$$ criteria to be considered good $$( 4 \times 0.2 = 0.8 > 0.7)$$.

## Inv-MR-sort :
Is the task of inferring the MR-Sort rules from examples made by a decision maker. (Better definitions inside the report)

## NCS :
To make it simple (otherwise, take a look at the report in the bottom of this page) : NCS is using criteria coalitions to determine whether to accept or not. For example, we accept a student if he has more than $$12$$ in `Mathematics` and `Physics` and more than $$10$$ in `Chemistry`.

## Inv-NCS :
Is the task of inferring the NCS rules and coalitions from examples made by a decision maker. (Better definitions inside the report)

## For A detailed description :
Below is our report for this project, please feel free to read it and email me if necessary.
<iframe src="/assets/pdf/Rapport_syst_mes_de_d_cision.pdf" style="width:100%; height:500px;" frameborder="0"></iframe>