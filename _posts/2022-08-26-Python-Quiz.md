---
keywords: fastai
description: Making a quiz using python.
title: Python Quiz Post
toc: true 
badges: true
comments: true
categories: [Week_1]
nb_path: _notebooks/2022-08-26-Python-Quiz.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-26-Python-Quiz.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Running-Quiz.py">Running Quiz.py<a class="anchor-link" href="#Running-Quiz.py"> </a></h2><p>This is the example Python quiz:</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span><span class="o">,</span> <span class="nn">sys</span>

<span class="k">def</span> <span class="nf">question_with_response</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="k">return</span> <span class="n">msg</span>

<span class="n">questions</span> <span class="o">=</span> <span class="mi">3</span>
<span class="n">correct</span> <span class="o">=</span> <span class="mi">0</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hello, &#39;</span> <span class="o">+</span> <span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; running &quot;</span> <span class="o">+</span> <span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You will be asked &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions.&quot;</span><span class="p">)</span>
<span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;Are you ready to take a test?&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to include other functions that were previously developed?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;import&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to evaluate correct or incorrect response in this example?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;if&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="s2">&quot;expression&quot;</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="k">else</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; you scored &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correct</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello, RyanHaki running /bin/python3
You will be asked 3 questions.
Question: Are you ready to take a test?
Question: What command is used to include other functions that were previously developed?
import is correct!
Question: What command is used to evaluate correct or incorrect response in this example?
if is correct!
Question: Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?
expression is correct!
RyanHaki you scored 3/3
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Python-Quiz">Python Quiz<a class="anchor-link" href="#Python-Quiz"> </a></h2><p>This is my own Python quiz:</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">Python_Quiz</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="k">global</span> <span class="n">word</span>
    <span class="nb">print</span> <span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">word</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="k">return</span> <span class="n">word</span>

<span class="n">questions</span> <span class="o">=</span> <span class="mi">5</span>
<span class="n">correct_answer</span> <span class="o">=</span> <span class="mi">0</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Hello, you will be asked &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; short questions&quot;</span><span class="p">)</span>

<span class="n">question_list</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;What is the answer to this math problem: What does 45x7=&quot;</span><span class="p">,</span> <span class="s2">&quot;What is the most popular religion in the world?&quot;</span><span class="p">,</span> 
<span class="s2">&quot;What is the capital of the U.S?&quot;</span><span class="p">,</span> <span class="s2">&quot;How many kg is in 5g&quot;</span><span class="p">,</span> <span class="s2">&quot;How many mm are in 1 km&quot;</span><span class="p">]</span>
<span class="n">answer_list</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;315&quot;</span><span class="p">,</span> <span class="s2">&quot;Christianity&quot;</span><span class="p">,</span> <span class="s2">&quot;Washington D.C.&quot;</span><span class="p">,</span> <span class="s2">&quot;0.005 kg&quot;</span><span class="p">,</span> <span class="s2">&quot;1000000 mm&quot;</span><span class="p">]</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">):</span>
    <span class="n">Python_Quiz</span><span class="p">(</span><span class="n">question_list</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
    <span class="k">if</span> <span class="n">word</span> <span class="o">==</span> <span class="n">answer_list</span><span class="p">[</span><span class="n">i</span><span class="p">]:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer is correct&quot;</span><span class="p">)</span>
        <span class="n">correct_answer</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer is incorrect&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You scored &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correct_answer</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello, you will be asked 5 short questions
Question: What is the answer to this math problem: What does 45x7=
Answer is correct
Question: What is the most popular religion in the world?
Answer is correct
Question: What is the capital of the U.S?
Answer is incorrect
Question: How many kg is in 5g
Answer is correct
Question: How many mm are in 1 km
Answer is correct
You scored 4/5
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

