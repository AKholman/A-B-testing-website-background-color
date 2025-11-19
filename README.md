
📊 A/B Testing Analysis — Does Website Background Color Affect Conversions?

This project explores whether changing a website’s background color can improve user engagement and conversions. Using a synthetic A/B testing dataset generated with NumPy, we simulate user interactions on a fictional UK e-commerce website to determine if a design change impacts user behavior.

🔍 Project Overview

The business question:

Does changing the website background color from white (control) to black (treatment) increase conversion rates?
To answer this, we conduct an A/B test comparing two user groups:

Group A — Control: Default white background
Group B — Treatment: New black background

A proper A/B test allows us to evaluate whether differences between these groups are meaningful or simply due to random variation.

📁 Dataset Description
The synthetic dataset simulates realistic e-commerce traffic and contains the following fields:

| Column         | Description                                       |
| -------------- | ------------------------------------------------- |
| **User ID**    | Unique visitor identifier                         |
| **Group**      | `A` (control) or `B` (treatment)                  |
| **Page Views** | Number of pages viewed during the session         |
| **Time Spent** | Time on site in seconds                           |
| **Conversion** | 1 if the user completed the target action, else 0 |
| **Device**     | Desktop, Tablet, or Mobile                        |
| **Location**   | UK region (e.g., London, Manchester)              |


📈 Summary of A/B Test Findings

We compared conversion rates between Group A and Group B using a two-proportion Z-test.
Hypotheses:
H₀ (Null): Conversion rates for the two pages are equal
H₁ (Alt): Conversion rates differ between the two pages

Results:

| Metric              | Group A (Control) | Group B (Treatment) |
| ------------------- | ----------------- | ------------------- |
| **Conversion Rate** | **5.40%**         | **14.07%**          |

Statistical test output:

Z-statistic: 10.354
p-value: 3.99 × 10⁻²⁵
Significance level (α): 0.05

Interpretation:
The p-value is far below 0.05 → reject the null hypothesis.
➡️ The black background (Group B) performs significantly better than the white background (Group A).
➡️ The new design produces a substantial increase in conversions.

🧠 Final Conclusion:
The A/B test provides strong statistical evidence that the new page with a black background leads to higher user conversions. Adopting the new background color is likely to improve overall user engagement and business performance.


📬 Contact / Feedback:
If you'd like help expanding this project (ML modeling, MLflow tracking, Streamlit dashboard, or deployment to Hugging Face Spaces), feel free to reach out.