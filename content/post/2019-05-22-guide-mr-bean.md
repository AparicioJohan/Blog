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
showtoc: true
---

<style>
div {
  text-align: justify;
  text-justify: inter-word;
}
</style>

<link href="/style.css" rel="stylesheet"></link> 


<button onclick="topFunction()" id="myBtn" title="Go to top"> <i class="fa fa-arrow-up"></i> </button>

<center>
 <img src="/img/interfaz.png" alt="interface"> 
</center>


**URL:** https://beanteam.shinyapps.io/MrBean/

# Mr.Bean

<div>
Is a web application for simplifying the analysis of large-scale plant breeding experiments using <em>spatial analysis</em> , as implemented in the <code>R-package</code>  <code>SpATS</code> . It provides the possibility for visualizing raw data, indentifying outliers, fitting mixed linear models <strong>(MLM)</strong>  with or without spatial correction, retrieve <em> BLUPs/BLUEs</em>  and heritabilites from single-environment trials. Mr. Bean also provides a module for comparing multiple sources data (e.g. multiple environments, multiple traits, etc.) using Pearson correlation coefficients and principal component analysis <strong>  (PCA) </strong>. </div>



 
# Tab navigation

## 1. Data

<div>
<p class="ex1">
	Use this module to load and visualize your raw data. Please follow the indications for <a href="https://en.wikipedia.org/wiki/Tidy_data">tidying data</a>. In short, there should be one observation per row, and each column should represent an independent feature or characteristic of that observation.</p>   </div>



##	2. Spatial Model
###	2.1. SpATS
Use this sub-module to fit the MLM with spatial correction. Follow the <em>  step-by-step guide </em>  (red button). After fitting the model, you'll be able to get a summary of the model's components (effective dimensions, convergence, deviance, etc.), display and download the fitted spatial trend in your trial (2D or 3D), and visualize the variance components in the model. In addition you can directly download the <em> BLUEs/BLUPs </em> for your chosen response variable. 

  

### 2.2. BLUPs/BLUEs 
<div>
<p >	 	Use this sub-module to visualize the BLUEs/BLUPs from the previous fitted model. There's also a download button for your BLUEs/BLUPs.</p> </div>


### 2.3. Residuals
 <div>
Use this sub-module to identify possible outliers in your response variable. The "Raw-data" boxes display the outliers from your raw data that were identified using the median absolute deviation (MAD) and the inter-quartilic range (IQR). The "Residual" boxes display observations with extreme residuals that were identified after fitting the MLM. After setting the outlier observations as NA depending on the chosen method (you can choose one, two or all the proposed methods), you can download the cleaned dataset. Load this file in the Data module to fit the model without outlier observations.</div>




## 3. Mixed model
### 3.1. Lme4
 <div>
	<p>
		Use this sub-module to fit the MLM for alpha-lattice, RCB designs, or write your own linear model using the Lme4 syntax.</p> 
 </div>
 
###	3.2. BLUPs/BLUEs
 <div>
	<p>
		Use this sub-module to visualize the BLUEs/BLUPs from the previous fitted model. There's also a download button for your BLUEs/BLUPs.</p>
		</div>



## 4. Comparison 
<div>
<p >
	Use this module to make multiple comparisons from e.g. multiple environments, multiple traits, etc. Using Pearson correlation coeffiecients for paired comparisons and PCA for multiple comparisons. This module provides its own box for uploading your data.</p> 	
</div>

	
 <script type="text/javascript" src="/java.js"></script>
