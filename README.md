# B2B Vendor Payment Delay Prediction (E-Commerce/Retail Credit Risk)

## Problem Statement

Schuster is a multinational retail company dealing in sports goods and accessories. Schuster conducts significant business with hundreds of its vendors, with whom it has credit arrangements. Unfortunately, not all vendors respect credit terms and some of them tend to make payments late. Schuster levies heavy late payment fees, although this procedure is not beneficial to either party in a long-term business relationship. The company has some employees who keep chasing vendors to get the payment on time; this procedure nevertheless also results in non-value-added activities, loss of time and financial impact. Schuster would thus try to understand its customers’ payment behaviour and predict the likelihood of late payments against open invoices.

## The payment process at Schuster:

Every time a transaction of goods takes place with a vendor, the accounting team raises an invoice and shares it with the vendor. This invoice contains the details of the goods, the invoice value, the creation date and the payment due date based on the credit terms as per the contract. Business with these vendors occurs quite frequently. Hence, there are always multiple invoices associated with each vendor at any given time.

## Business Objectives
1. Segment vendors/customers based on historical payment behavior
2. Predict likelihood of delayed payment on open invoices
3. Help collectors prioritize follow-ups before due dates to reduce late payments

## Approach
### 1) Customer Segmentation (Behavior Clustering)
- Applied **K-Means clustering (3 clusters)** using historical payment delay patterns
- Segments:
  - Early payers
  - Medium duration payers
  - Prolonged payers

### 2) Delay Prediction (Classification Modeling)
- Built and evaluated:
  - Logistic Regression
  - Random Forest (final model)
- Random Forest chosen for stronger performance on categorical-heavy data and better recall for late-payer detection.

## Key Impact (Quantified)
- Flagged **50.2% open invoices** as potential delay-risk to prioritize collections
- Identified prolonged payer segment with **~100% delay-rate**, enabling targeted high-risk follow-up strategy

## Tech / Tools
- Python
- EDA & Feature Engineering
- K-Means Clustering
- Logistic Regression
- Random Forest
- Model Evaluation: ROC/AUC, Precision-Recall

## Author
**Syed Mohammad Bilal**
