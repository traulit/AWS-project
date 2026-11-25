# AWS-project
**Credit project dashboard**
Analysis + credit risk modeling project on the Lending Club loan portfolio, covering exploratory analysis, SQL, WoE/IV feature selection, a PD scorecard, LGD/EAD estimation, and portfolio-level Expected Credit Loss under the IFRS 9 framework (ECL = PD × LGD × EAD).

**Business problem**
Banks don't just need to know who is likely to default — they need to know how much money they expect to lose, in dollars, to set loan-loss provisions on the balance sheet.

**Dataset**
Lending Club Loan Data — real historical loan outcomes, 2007–2018. Filtered to resolved loans only (Fully Paid or Charged Off, since only these have a known outcome): 1.35M loans, default rate 19.86%.

**Sheet 1 - Fraud Analysis Overview**
<img width="1797" height="1623" alt="image" src="https://github.com/user-attachments/assets/487798ad-97bf-47e9-b1c3-f6033e48fb34" />
**What drives fraud, when does it happen, and where should monitoring focus?**
This overview highlights the portfolio's main fraud patterns. Fraud is heavily concentrated during late-night hours, rises sharply for transactions above $250, and is concentrated in three merchant categories that run more than 2× the average fraud rate.

**Sheet 2 - Behaviour & Trend**
<img width="1797" height="1378" alt="image" src="https://github.com/user-attachments/assets/d467e0d6-5033-4851-9157-56f45b3179b8" />
**How does customer behaviour relate to fraud risk?**
Fraud is strongly associated with unusual spending behaviour. Transactions exceeding a card's normal spending level show substantially higher fraud rates, while monthly fraud rates remain relatively stable despite fluctuations in transaction volume.

**Sheet 3 - Who & Where**
<img width="1797" height="1518" alt="image" src="https://github.com/user-attachments/assets/a729c588-a62d-4f76-9e20-fa531b145612" />
**Do geography and customer demographics meaningfully explain fraud?**
Geographic and demographic signals are weak compared with behavioural patterns. Only Alaska exceeds the 1.5× risk threshold, while age and gender differences remain modest relative to time-of-day and spending behaviour effects.

**Sheet 4 - Merchant**
<img width="1797" height="1308" alt="image" src="https://github.com/user-attachments/assets/2efd5e0d-0722-4f50-a3a5-f4bceb187ac8" />
**Which merchants consistently exhibit elevated fraud risk?**
Merchants are benchmarked against their transaction category to identify outliers. The focus is on merchants with sufficient transaction volume whose fraud rates materially exceed category norms and warrant enhanced monitoring.

**Sheet 5 - Model Impact**
<img width="1797" height="1335" alt="image" src="https://github.com/user-attachments/assets/b4155191-f7ee-463a-b720-dd0b9d91ff8c" />
**How effectively do fraud indicators separate risky transactions?**
This section evaluates fraud signals and model performance. The objective is to identify which features contribute most to detection accuracy and assess how well the model distinguishes fraudulent from legitimate transactions.
