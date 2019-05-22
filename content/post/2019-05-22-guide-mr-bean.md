---
title: Guide Mr.Bean
author: Aparicio, Johan
date: '2019-05-22'
slug: guide-mr-bean
categories:
  - Statistics
tags:
  - SpATS
subtitle: 'Application for Spatial Analysis'
description: 'User guide Mr.Bean'
image: ''
showtoc: false
---



<FONT SIZE=7>Mr.Bean</font>


Is a web application for simplifying the analysis of large-scale plant breeding experiments using <em>spatial analysis</em> , as implemented in the <code>R-package</code>  <code>SpATS</code> . It provides the possibility for visualizing raw data, indentifying outliers, fitting mixed linear models <strong>(MLM)</strong>  with or without spatial correction, retrieve <em> BLUPs/BLUEs</em>  and heritabilites from single-environment trials. Mr. Bean also provides a module for comparing multiple sources data (e.g. multiple environments, multiple traits, etc.) using Pearson correlation coeffiecients and principal component analysis <strong>  (PCA) </strong>. 

 <ul>
<div>
 
<h2>Tab navigation</h2>

 <li>	<h3>Data</h3> </li>	
<p class="ex1">
	Use this module to load and visualize your raw data. Please follow the indications for <a href="https://en.wikipedia.org/wiki/Tidy_data">tidying data</a>  . In short, there should be one observation per row, and each column should represent an independent feature or characteristic of that observation.</p>   </div>



 <li>	<h3>	Spatial Model</h3> </li>	 
 <ul>
       <li>	<h4>	SpATS </h4></li>
</ul>
Use this sub-module to fit the MLM with spatial correction. Follow the <em>  step-by-step guide </em>  (red button). After fitting the model, you'll be able to get a summary of the model's components (effective dimensions, convergence, deviance, etc.), display and download the fitted spatial trend in your trial (2D or 3D), and visualize the variance components in the model. In addition you can directly download the <em> BLUEs/BLUPs </em> for your chosen response variable. 

  
<div>
	 <ul> 
  <li>	<h4>	BLUPs/BLUEs </h4></li>
</ul> 
<p >	 	Use this sub-module to visualize the BLUEs/BLUPs from the previous fitted model. There's also a download button for your BLUEs/BLUPs.</p> </div>

 <div>
	 <ul>  
  <li>	<h4>Residuals</h4></li>
</ul> 

Use this sub-module to identify possible outliers in your response variable. The "Raw-data" boxes display the outliers from your raw data that were identified using the median absolute deviation (MAD) and the inter-quartilic range (IQR). The "Residual" boxes display observations with extreme residuals that were identified after fitting the MLM. After setting the outlier observations as NA depending on the chosen method (you can choose one, two or all the proposed methods), you can download the cleaned dataset. Load this file in the Data module to fit the model without outlier observations.</div>


 <div>

<li><h3> Mixed model</h3></li>
 <ul>
  <li>	<h4>Lme4</h4></li>
</ul> 
	<p >
		Use this sub-module to fit the MLM for alpha-lattice, RCB designs, or write your own linear model using the Lme4 syntax.</p> 
 <div>
	  	<ul>
  <li>	<h4>	BLUPs/BLUEs</h4></li>
</ul> 
	<p >
		Use this sub-module to visualize the BLUEs/BLUPs from the previous fitted model. There's also a download button for your BLUEs/BLUPs.</p>
		</div>


<div>

 <li><h3>	Comparison </h3> </li>
<p >
	Use this module to make multiple comparisons from e.g. multiple environments, multiple traits, etc. using Pearson correlation coeffiecients for paired comparisons and PCA for multiple comparisons. This module provides its own box for uploading your data.</p> 	


	

