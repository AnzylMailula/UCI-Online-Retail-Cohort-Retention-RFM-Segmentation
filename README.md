# UCI-Online-Retail-Cohort-Retention-RFM-Segmentation
Customer retention analysis on a real UK online gift retailer's transaction data, using cohort retention analysis and RFM (Recency, Frequency, Monetary) segmentation to identify where revenue is concentrated and where it's at risk. Third portfolio project, focused on retention analytics.
What's in this repo
Cohort Analysis.pdf: Decision, North Star Metrics, Recommendations, Financial Impact, and Caveats (non-technical, decision-focused)
Cohort Methodology And Cleaning  Notes.md : Full evidence tables, methodology, formulas, merges, and relationships (for anyone verifying the work)
dashboard.png : <img width="703" height="380" alt="image" src="https://github.com/user-attachments/assets/2f33c6cd-06a7-49ad-b630-2a42e2b0b1eb" />


UCI Machine Learning Repository — Online Retail II. Real transactions from a UK-based online gift and homeware retailer, December 2009–December 2011, ~1 million rows across two year-sheets. Not included in this repo due to size  download directly from the source link above.

Tools

Excel, Power Query (M)

Approach
Cleaned and flagged ~1M transaction rows separating real product sales from cancellations, postage, discounts, and manual adjustments, with each cleaning rule verified against the underlying data rather than assumed
Built a cohort retention table using a custom "months since first purchase" measure, allowing fair comparison between customers who joined at different times
Segmented every customer with RFM (Recency, Frequency, Monetary) into six behavioral groups: Champions, Loyal, New/Promising, At Risk, Can't Lose Them, Hibernating/Lost
Cross-referenced cohort and segment data to find where revenue is concentrated and how durable it is
Caught and fixed a real scoring bug mid-analysis (documented in the technical appendix)  a good example of validating findings against logical consistency, not just trusting the output
Key Finding

A quarter of customers (Champions) generate 69% of revenue — a healthy core. But a separate ~28% of customers, representing ~21% of revenue, are showing clear signs of disengagement (At Risk / Can't Lose Them), concentrated heavily in the business's earliest cohort. Both new customer acquisition and retention quality have declined roughly threefold since the business's first year.

Full findings and recommendations in the Cohort Analysis.pdf.
