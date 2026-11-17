1. Project overview
Aarav Foods, a packaged-food company, is considering a ₹100 crore plant expansion, of which ₹60 crore must be raised externally. The CFO's central question is whether Aarav is financially healthy relative to four peers, how the external funding should be raised, and whether the expansion meets the company's investment threshold.

This team capstone brings together four connected workstreams: profit quality, working-capital and cash movement, returns and financing, and a Power BI peer dashboard with an expansion business-case assessment. Each workstream uses the output of the preceding workstream so that the final recommendation is based on a consistent set of figures.
Project objectives
- Evaluate the quality of reported profit and distinguish operating performance from non-operating income.
- Compare working-capital efficiency using the cash conversion cycle (CCC).
- Assess capital efficiency through ROCE and ROE.
- Compare debt and equity financing using earnings per share (EPS) under two return scenarios.
- Build a peer-comparison dashboard and test the proposed expansion against a 5× benefit-to-investment target, including a ±30% worst-case scenario.
- Present a clear, evidence-based recommendation to the CFO.

2. Case scope and companies
The analysis uses the supplied capstone data pack only. The five companies compared are:
1. Aarav Foods
2. Kaveri Snacks
3. Ruchi Dairy
4. Sundar Beverages
5. Nirmal Agro
Source data: data/financials.csv and data/expansion_plan.csv (provided with the capstone brief and retained unmodified in this repository).

3. Key performance indicators
KPI	Formula	Source columns	Business question
Operating profit margin	Operating profit (EBIT) ÷ Revenue × 100	operating_profit_ebit_crore, revenue_crore	How profitable is the company's core operating business?
Cash conversion cycle (CCC)	Debtor days + Inventory days − Payable days	debtor_days, inventory_days, payable_days	How long is cash tied up in the operating cycle?
Return on capital employed (ROCE)	Operating profit (EBIT) ÷ Capital employed × 100	operating_profit_ebit_crore, capital_employed_crore	How effectively is the company using its capital, and how does its return compare with the cost of borrowing?
Return on equity (ROE)	Net profit ÷ Equity × 100	Computed net_profit, equity_crore	What return is generated on shareholders' funds?


Calculation conventions: A 25% tax rate is applied throughout the profit and EPS calculations. Percentages are generally presented to one decimal place, while the dashboard and return comparisons retain the precision needed to show the calculations. Currency amounts are in ₹ crore unless stated otherwise.

4. Analysis and findings
Part 1 — How good is the profit?
1.1 Profit ladder
Profit before tax (PBT) is calculated as:

PBT = Operating profit + Non-operating income − Interest expense

Tax is 25% of PBT, and net profit is PBT less tax. Operating profit margin is operating profit divided by revenue; net profit margin is net profit divided by revenue. The non-operating share is non-operating income divided by PBT.
Company	PBT (₹ cr)	Tax (₹ cr)	Net profit (₹ cr)	Operating margin	Net margin	Non-operating share of PBT
Aarav Foods	98	24.50	73.50	6.7%	4.1%	8.2%
Kaveri Snacks	144	36.00	108.00	12.5%	9.0%	4.2%
Ruchi Dairy	205	51.25	153.75	3.5%	5.9%	78.0%
Sundar Beverages	94	23.50	70.50	12.2%	7.8%	4.3%
Nirmal Agro	32	8.00	24.00	4.0%	1.6%	31.2%


1.2 Which company's profit is propped up?
Ruchi Dairy has the clearest dependence on non-core income. Non-operating income accounts for 78.0% of its PBT. Its operating profit is ₹90 crore and its operating margin is only 3.5%, yet its net profit is ₹153.75 crore—higher than its operating profit. This means the bottom-line result does not, by itself, represent the strength of its core packaged-food operations. Operating profit is therefore the more useful indicator of core operating health because it isolates earnings from the main business before non-operating items.

Aarav Foods' own profit is comparatively more operating-led: only 8.2% of its PBT comes from non-operating income. Aarav reports PBT of ₹98 crore, tax of ₹24.50 crore and net profit of ₹73.50 crore.
1.3 Chart finding
The operating-profit-versus-net-profit comparison across all five companies highlights the unusual result at Ruchi Dairy: its net profit (₹153.75 crore) exceeds its operating profit (₹90 crore). This supports the conclusion that non-operating income materially affects its reported profitability.
Part 2 — How well does cash move?
2.1 Cash conversion cycle
CCC = Debtor days + Inventory days − Payable days
Company	Debtor days	Inventory days	Payable days	CCC (days)	Rank (lower is better)
Ruchi Dairy	10	20	60	-30	1
Kaveri Snacks	15	38	45	8	2
Sundar Beverages	35	25	20	40	3
Aarav Foods	28	55	40	43	4
Nirmal Agro	40	80	30	90	5


Aarav's CCC is 43 days, ranking fourth out of five. Cash remains tied up in its operating cycle longer than it does at Kaveri Snacks and Sundar Beverages; only Nirmal Agro has a longer cycle. A lower CCC is generally better because cash is recovered more quickly.

A negative CCC, as at Ruchi Dairy (−30 days), means the company receives cash from customers before it has to pay suppliers. In effect, supplier credit helps fund its operations. CCC should be compared within the same industry because inventory holding periods and customer/supplier credit terms can differ substantially across sectors.
2.2 Supply-chain finance scenario
Under the supplied scenario, a bank pays Aarav's suppliers early and Aarav receives 15 additional days before it must pay the bank. Payable days therefore increase from 40 to 55.

Revised CCC = 28 debtor days + 55 inventory days − 55 payable days = 28 days

Aarav's CCC falls from 43 days to 28 days, a 15-day improvement. Suppliers receive earlier payment from the bank, while Aarav benefits from the extended payment period. The arrangement reduces the time Aarav's own cash is tied up in payables.
2.3 Dividend signals
Company	Dividend per share: this year	Last year	Change	Signal
Aarav Foods	₹2.00	₹2.00	Unchanged	Steady
Kaveri Snacks	₹3.00	₹2.50	Increased	Confidence signal
Ruchi Dairy	₹0.00	₹4.00	Skipped	Strongest warning
Sundar Beverages	₹1.50	₹1.00	Increased	Confidence signal
Nirmal Agro	₹1.00	₹1.50	Reduced	Mild warning


Ruchi Dairy's decision to skip its dividend is the strongest warning signal in this peer group. Kaveri Snacks and Sundar Beverages increased their dividends, which can signal management confidence in expected cash flows. Aarav's dividend is unchanged, while Nirmal Agro's reduction is a milder warning. Dividend changes are signals about management's confidence; they should be interpreted alongside profitability and cash-flow indicators.
Part 3 — Returns and the funding decision
3.1 ROCE and ROE
ROCE = Operating profit ÷ Capital employed × 100

ROE = Net profit ÷ Equity × 100
Company	ROCE	ROE
Aarav Foods	14.63%	13.61%
Kaveri Snacks	25.00%	22.50%
Ruchi Dairy	6.00%	17.08%
Sundar Beverages	22.00%	20.14%
Nirmal Agro	6.67%	4.62%


Kaveri Snacks is strongest on both ROCE and ROE. Ruchi Dairy has the weakest ROCE at 6.00%, followed by Nirmal Agro at 6.67%. Nirmal Agro has the weakest ROE at 4.62%. Ruchi Dairy's ROE of 17.08% appears comparatively healthy, but its low ROCE and high non-operating share show why ROE should not be read in isolation.

A long-term investor would generally give greater weight to ROCE, which indicates how efficiently the business employs capital. A short-term shareholder-return view may place more weight on ROE, which measures returns on equity.

The derived peer dataset used by the dashboard is provided as peer_metrics.csv, with one row per company and the required fields: operating margin, net margin, CCC, ROCE, ROE and non-operating share of PBT.
3.2 EPS today
For the financing comparison, the case specifies EBIT of ₹120 crore, non-operating income of ₹8 crore, interest expense of ₹30 crore, tax of 25% and 10 crore shares.

EPS = (EBIT + Non-operating income − Interest) × (1 − Tax rate) ÷ Shares

Today's EPS is:

(₹120 cr + ₹8 cr − ₹30 cr) × 75% ÷ 10 cr shares = ₹7.35
3.3 Debt versus equity when the investment earns 14%
The ₹60 crore investment is assumed to generate a 14% annual return, increasing EBIT by ₹8.4 crore.
- Debt: Borrow ₹60 crore at 10%; annual interest increases by ₹6 crore.
- Equity: Issue 0.75 crore new shares at ₹80 per share; total shares increase to 10.75 crore and interest remains unchanged.
Scenario	EPS
Current EPS	₹7.35
Debt funding, 14% project return	₹7.53
Equity funding, 14% project return	₹7.42


At a 14% project return, debt produces the higher EPS because the return on the investment exceeds the 10% borrowing rate.
3.4 What if the return is only 9%?
At a 9% return, EBIT increases by ₹5.4 crore.
Scenario	EPS
Current EPS	₹7.35
Debt funding, 9% project return	₹7.305
Equity funding, 9% project return	₹7.214


Both financing options produce EPS below today's ₹7.35 when the project return is only 9%. The results demonstrate the financing rule: debt improves EPS when the return earned on the investment exceeds the cost of debt. If the return is below the interest rate, debt does not create an EPS benefit. Excessive debt also increases financial risk because interest payments remain due even if operating returns weaken.
3.5 Would a bank lend?
Aarav's ROCE is 14.63% (₹120 crore EBIT ÷ ₹820 crore capital employed), above the assumed 10% interest rate. This suggests that Aarav could be able to earn more on its employed capital than the cost of borrowing, which supports the case for bank lending. However, Aarav's ROCE is below Kaveri Snacks (25.00%) and Sundar Beverages (22.00%), so its capital efficiency is not the strongest among peers.
Part 4 — Peer dashboard and expansion business case
4.1 Power BI peer dashboard
The Power BI report is supplied as Power-BI/aarav_peer_dashboard.pbix. Inspection of the submitted PBIX shows four KPI cards, a company slicer, two clustered-column visuals and a donut chart. The capstone brief additionally requires a matrix with operating margin, CCC, ROCE and ROE, including conditional formatting (CCC red above 35 days and ROCE red below 10%); that matrix is not present in the uploaded PBIX and should be added before final submission. The dashboard values below are the values shown in the team's presentation and should be checked in Power BI after the final dashboard update.

With Aarav Foods selected, the dashboard values are:
KPI	Aarav Foods
Operating margin	6.7%
CCC	43 days
ROCE	14.63%
ROE	13.61%


With no company selected, the peer averages include 30.2 days CCC and 14.86% ROCE. The matrix flags CCC for Aarav Foods, Sundar Beverages and Nirmal Agro; it flags ROCE for Ruchi Dairy and Nirmal Agro. Kaveri Snacks is within both stated thresholds. Ruchi Dairy's ROE (17.08%) is materially higher than its ROCE (6.00%), reinforcing the need to view both measures.
4.2 Expansion business case
The supplied expansion plan contains ₹90 crore for plant and machinery and ₹10 crore for commissioning, training and launch.
Measure	Calculation	Result
Total investment	₹90 cr + ₹10 cr	₹100 crore
Annual benefit	₹130 cr extra volume margin + ₹60 cr automation savings	₹190 crore
Three-year benefit	₹190 cr × 3	₹570 crore
Benefit-to-investment ratio	₹570 cr ÷ ₹100 cr	5.70×


The base case passes the 5× target because the benefit-to-investment ratio is 5.70×.
4.3 ±30% worst-case test
The worst-case test reduces benefits by 30% and increases investment by 30%.
- Annual benefit after a 30% reduction: ₹133 crore.
- Three-year benefit: ₹399 crore.
- Investment after a 30% increase: ₹130 crore.
- Worst-case benefit-to-investment ratio: ₹399 crore ÷ ₹130 crore = 3.07×.
The worst case fails the 5× target. If the downside case is plausible, the expansion should not be funded and released all at once. A proof of concept and staged release of funds would allow benefits and costs to be checked before each subsequent stage.
4.4 Recommendation to the CFO
Five-sentence recommendation summary
1. The team recommends a conditional go for the ₹100 crore expansion because the base-case benefit-to-investment ratio is 5.70×, above the 5× target.
2. The recommendation is conditional because the ±30% worst-case scenario falls to 3.07× and fails the target.
3. Aarav's operating margin is 6.7%, its non-operating share of PBT is 8.2%, its CCC is 43 days and its ROCE is 14.63%, showing genuine operating profit but middling cash and capital efficiency relative to peers.
4. Debt is preferable to equity only if the project return remains above the 10% borrowing rate, since at 14% debt EPS is ₹7.53 versus ₹7.42 for equity, while at 9% both alternatives fall below today's EPS of ₹7.35.
5. The team recommends starting with a proof of concept, releasing debt in stages, using supply-chain finance to reduce CCC to 28 days, and reviewing realised benefits, costs and ROCE at each stage gate.
What would change the recommendation: a project return below the 10% borrowing rate, or proof-of-concept results showing that benefits and costs are tracking the downside case.

Two principal risks:
1. Leverage risk: debt creates fixed interest obligations even if project returns fall below 10%.
2. Estimation risk: the business case is based on estimates with ±30% uncertainty; the downside case produces only 3.07×.
Proposed next steps:
1. Approve a first-stage proof of concept.
2. Arrange the ₹60 crore debt facility with staged drawdown, subject to the return remaining above 10%.
3. Negotiate supply-chain finance to move payable days from 40 to 55 and reduce CCC from 43 to 28 days.
4. Review realised benefits, costs and ROCE against the 10% borrowing rate at each stage gate.
5. Team contributions
This was completed as a collaborative team capstone. The following table records the primary deliverable ownership:
Team member	Primary contribution
Vedant Dhankar	GitHub repository preparation, project documentation and README compilation.
Shivani	Excel financial analysis workbook and spreadsheet calculations.
Aditi	Power BI peer-comparison dashboard.
Ridhi	Final capstone presentation and slide development.


The project connects the Excel analysis, Power BI dashboard and presentation into one consistent CFO recommendation. Each team member should be prepared to explain the assumptions, calculations and conclusions across the full case, in line with the capstone instructions.
6. Repository contents
aarav-foods-finance-capstone/
│
├── README.md
├── peer_metrics.csv
│
├── data/
│   ├── financials.csv
│   └── expansion_plan.csv
│
├── Project-Brief/
│   ├── AaravFoods_Capstone_Brief.md
│   └── AaravFoods_Capstone_Brief.pdf
│
├── Excel/
│   └── aarav_finance.xlsx
│
├── Power-BI/
│   └── aarav_peer_dashboard.pbix
│
└── Presentation/
    └── AaravFoods_Presentation.pptx
Files and how to use them
File	Purpose
data/financials.csv	Original supplied financial data for Aarav Foods and its four peers.
data/expansion_plan.csv	Original supplied investment and annual-benefit assumptions.
Excel/aarav_finance.xlsx	Team workbook containing Profit, Cash, Returns, Funding and Business Case calculations.
peer_metrics.csv	Peer-level metrics prepared for the Power BI dashboard.
Power-BI/aarav_peer_dashboard.pbix	Power BI report for peer comparison and KPI monitoring.
Presentation/AaravFoods_Presentation.pptx	Eight-slide presentation of the case, analysis and recommendation.
Project-Brief/	Original capstone instructions supplied for the assignment.


7. Tools used
- Microsoft Excel — financial calculations, formulas, comparisons and business-case analysis.
- Power BI Desktop — peer dashboard, KPI cards, slicer, charts, matrix and conditional formatting.
- PowerPoint — final presentation for the CFO.
- GitHub — versioned public repository and final team submission.
8. Submission
This repository is intended to serve as the team's single public GitHub submission for the Aarav Foods Finance Capstone.

Repository name required by the brief: aarav-foods-finance-capstone
Prepared as a team capstone submission. All analysis is based on the supplied case data and assumptions in the project brief.
