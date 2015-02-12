---
layout: post
title: Twitter Sentiment Analysis
categories: [university]
tags: [machine learning, sentiment analysis, twitter, java]
fullview: true
icon: fa fa-twitter fa-lg
source: Pausa90/TwitterSentimentAnalysis
---

This project consists in creating a simple software tool that is able to classify and predict textual data, extrapolated from Twitter. Were considered 40183 tweet,divided between training-set (40000) and testing-set (183).

For semplicity, the tool stores the information in memory and was realized with K-NN as prediction algorithm. However it was implemented an interface "ClassificationAlgorithm" to allow any future changes to the system.

The goal of this project is to understand not only the positivity/negativity associated with a sentence, but also the influence of the parts of the speech contained therein.
The tool extracts the most common measures in information retrival area, from which it was possible to extract data and charts below with a 3-NN instance.

<table border="1" style="text-align: center">
	<tr>
		<td>ConfusionMatrix</td>
		<td>TruthPositive</td>
		<td>TruthNegative</td> 
	</tr>
	<tr>
		<td>SystemPositive</td>
		<td>100</td>
		<td>43</td> 
	</tr>	
	<tr>
		<td>SystemNegative</td>
		<td>8</td>
		<td>32</td> 
	</tr>
</table> 
<br>
Statistics:
<ul>
	<li>error rate: 43.04371584699454 </li>
	<li>accuracy: 0.48 </li>
	<li>precision: 0.6993006993006993 </li>
	<li>recall: 0.9259259259259259 </li>
	<li>breack-even: 0.8126133126133126 </li>
	<li>f1-measure: 0.7968127490039841 </li>
	<li>fails Number: 51</li>
</ul>

<div class="row">
	<p style="text-align: center"> Positive Recap </p>
	<img src="{{ site.BASE_PATH }}/assets/images/twitter_sentiment_analysis/recap_positive.png"/>
</div>
<br>

<div class="row">
	<p style="text-align: center"> Negative Recap </p>
	<img src="{{ site.BASE_PATH }}/assets/images/twitter_sentiment_analysis/recap_negative.png"/>
</div>