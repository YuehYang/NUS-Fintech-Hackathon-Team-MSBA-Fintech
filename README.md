# PaySec: Comprehensive payment security as a service

![PaySec Logo](https://github.com/YuehYang/NUS-Fintech-Hackathon-Team-MSBA-Fintech/blob/master/Picture1.png)

## Introduction
This repository is a project for NUS FinTech Hackathon (2021) and we are a team of 4 students from NUS MSBA. We proposed a payment security product called PaySec. 

This repository includes multiple notebooks and covers the key functions of PaySec.

## Requirements
To run the notebooks successfully, you need to set up:
- Python (3.7)
- Jupyter Notebook

And the libraries/packages installation codes are included in the first cell of each notebook.

## Table of contents

- [Network Analysis](#Network-Analysis)
- [Company Background Online Presence and Network Check](#Company-Background-Online-Presence-and-Network-Check)
- [B to B Transaction Classifier](#B-to-B-Transaction-Classifier)
- [GUI Demo](#GUI-Demo)

## Network Analysis
The notebook in `1.Network Analysis` performs clustering coefficient outlier detection and community detection on a simulated graph dataset. 

Clustering coefficients of entities will be calculated and outliers with relatively low coefficients will be flagged as suspicious entities. Besides, we also use Girvan-Newman algorithm to detect transaction communities, in order to uncover some suspicious transaction patterns inside the network.

![Uncovered Suspicious Patterns](https://github.com/YuehYang/NUS-Fintech-Hackathon-Team-MSBA-Fintech/blob/master/Picture2.png)

## Company Background Online Presence and Network Check 
The notebook in `2.Company Background Online Presence and Network Check` demonstrates the possibility and logic to do a company background, online presence and network check in an effort to identify shell companies and prevent fraud transactions. 

Company information will be scraped from professional networking and company review sites and cross-referenced with google search results and some user-defined limit/minimal requirement (tweakable) to authenticate for entries to be genuine.

## B to B Transaction Classifier
This notebook in `3.B to B transaction classifier` shows the process of classification of clients to company or customer. We will execute background check with Web data scraping and NLP, but it is meaningless to conduct it for induvidual customers. Therefore, as a first step, we classify them using Naive Basian Classifier.

![Flow Chart](https://github.com/YuehYang/NUS-Fintech-Hackathon-Team-MSBA-Fintech/blob/master/Picture3.png)

## GUI Demo
The notebook in `4.GUI_demo` folder shows a GUI demo of PaySec.

# Team Members
Julian Ando

Hiroyuki Tsujikami 

Yang Yue

Ng Jian Lai
