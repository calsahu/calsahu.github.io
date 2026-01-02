# Data-Driven Housing Valuation and Tax Equity Analysis — Cook County Case Study

<div class="top-nav">
  <a href="index.html">About Me</a>
  <a href="https://docs.google.com/document/d/e/2PACX-1vTdXMOxjDVlwPxPEMZ2_DTfDJnAC52xALzhIjLUhGW5FnHeF41MyVcPV0RUxzgMhcjNPmRNMxvVOgRB/pub">Resume</a>
  <a href="project.html">Projects</a>
  <a href="paper.html">Papers</a>
  <a href="contact.html">Contact</a>
  <a href="awards.html">Awards</a>
</div>

<style>
.top-nav {
  margin: 10px 0 18px;
}

.top-nav a {
  display: inline-block;
  padding: 8px 14px;
  margin-right: 8px;
  border-radius: 20px;
  background: #f2f2f2;
  font-weight: 600;
  text-decoration: none;
}

.top-nav a:hover {
  background: #e0e0e0;
}
</style>

In this project, I analyzed a large housing dataset from the Cook County Assessor’s Office to understand how statistical modeling shapes property valuation and property tax outcomes across Chicago and its suburbs. I conducted exploratory data analysis, cleaned and engineered features (including regex extraction and one-hot encoding), and built a reproducible pandas data-processing pipeline before training and evaluating a linear regression model in scikit-learn using RMSE across training and test splits. I also interpreted residual error to assess how over- and undervaluation can differentially affect homeowners and neighborhoods, connecting model performance to questions of fairness, bias, and urban equity. This project strengthened my data science skills while deepening my planning perspective on the ethical use of predictive models in housing systems and public policy.

You can take a look at my code here:

[Exploring the dataset](https://drive.google.com/file/d/1uuEjkSb5-hTw000uZErN2IKy4KGDTbSP/view?usp=sharing)
[Fitting the regression model](https://drive.google.com/file/d/1ovy37321qPcCb4NF2B5nxIpZAgXXkMNq/view?usp=sharing)
