HanuAi ML Assessment — Task 2 final package
Contents:
- task2_eda_text_mining_executed_reviewed.ipynb — reviewed notebook with interpretation/limitations clarifications
- Hanuai task2 assignment.csv — original source dataset (1,000 rows x 20 columns)
- task2_processed_dataset.csv — enriched dataset (1,000 rows x 28 columns)
- task2_cluster_summary.csv — six-cluster summary with top terms and example event IDs
- task2_cluster_validation.csv — silhouette/cluster-size comparison for k=2..10
- task2_manual_review_sample.csv — 100-row sample for manual validation
- issue_category_distribution.png
- text_issue_category_distribution.png
- causal_code_distribution.png
- events_by_month.png
- cluster_sizes.png
- task2_stakeholder_report_reviewed.docx — revised stakeholder report
- TASK2_AUDIT_NOTES.txt — audit notes

Validation notes:
- Processed dataset: 1,000 rows x 28 columns; Event IDs unique; opened date range 2019-08-27 to 2021-06-01.
- Six-cluster counts: 335, 264, 104, 47, 56, 194 (total 1,000).
- The six-cluster sample silhouette is approximately 0.0108 (about 0.011), indicating weak separation; treat clusters as exploratory.
- The processed dataset has two issue-category fields with different label schemes: `issue_category` (7 groups) and `text_issue_category` (10 groups). The report's main category counts refer to `issue_category`; do not conflate the two charts.
- The PNGs and cluster summary were found in the accessible Task 2 folder and included in this package. Review the notebook's input path before rerunning on another machine.
