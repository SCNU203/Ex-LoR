# Ex-LoR

This dataset consists of 3,411 QA instances.(Train:2511;  Eval:300;  Test:600)


The files is divided into English version: train_en.json, val_en.json, test_en.json, and Chinese version: train_zh.json, val_zh.json, test_zh.json.


Each problem instance consists of three parts, as follows:   
(1) **Logical reasoning multiple choice questions.** Consists of context, question, and four options, only one of which is correct.   
(2) **Explanation** of how to get the answer through complex logical reasoning combination and transformation.   
(3) **Types of question.**    


 **An instance in the Ex-LoR:**

```
 "context": "Chen doesn't know both English and French."
 "question": "If the above statement is true, which of the following must be true?"
 "A": "Xiao Chen knows English but not French."
 "B": "Xiao Chen knows neither English nor French."
 "C": "If Xiao Chen knows English, he must not know French."
 "D": "If Xiao Chen doesn't know French, he must know English."
 "answer": "A"
 "explanation": "(Xiao Chen does not know English) V (Xiao Chen does not know French). This is equivalent to 1) Chen does not know English but knows French, 2) Chen does not know French but knows English, 3) Chen does not know English and does not know French."
 "question type": 1
 ```
 
 
 **About question type:**  
 
<table>
	<tr>
	    <th>Main classification</th>
	    <th>Secondary Classification</th>
      <th>Mark</th>
	    <th>Description</th>  
	</tr >
	<tr >
	    <td rowspan="2">Pure Formal Reasoning (38.05%)</td>
	    <td>Judgment Reasoning (28.64%)</td>
      <td>1</td>
	    <td>Contain logical languages such as "if","because",etc.</td>
	</tr>
	<tr>
	    <td>Similar (9.41%)</td>
    <td>2</td>
	    <td>Similar reasoning or argumentative structure.</td>
	</tr>
  <tr >
	    <td rowspan="2">Conditional Reasoning (19.03%)</td>
	    <td>True and False (4.78%)</td>
    <td>3</td>
	    <td>Get conclusions based on truth and falsehood.</td>
	</tr>
	<tr>
	    <td>Integrated Reasoning (14.25%)</td>
    <td>4</td>
	    <td>Match a set of objects and related information one by one.</td>
	</tr>
  <tr >
	    <td rowspan="2">Informal Reasoning / Argument (42.92%)</td>
	    <td>Strengthen Argument (24.25%)</td>
    <td>5</td>
	    <td>Strengthen the correctness of the stem argument.</td>
	</tr>
	<tr>
	    <td>Weaken Argument (18.67%)</td>
    <td>6</td>
	    <td>Proof question stem argument not valid.</td>
	</tr>
</table>


