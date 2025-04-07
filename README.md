# Fin(ancial) An(alyst) GPT – a tool to analyze company's financials

This script is an AI-powered financial analyst that summarizes company finances, provides pros and cons, and makes recommendations based on the provided financial information. It uses the OpenAI API or an open-source model from Ollama to generate the analysis.

## Installation

To run the script, you need to have the following packages installed:

- requests==2.26.0
- python-dotenv==0.19.1

You can install these packages by running the following command:

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Configuration

Before running the script, you need to set up your environment variables. Create a `.env` file in the project directory and add the following variables:

```plaintext
SIMFIN_API_KEY=YOUR_SIMFIN_API_KEY
OPENAI_API_KEY=YOUR_OPENAI_API_KEY
```

Replace `YOUR_SIMFIN_API_KEY` with your SimFin API token and `YOUR_OPENAI_API_KEY` with your OpenAI API key.




## Usage

To use the AI Financial Analyst with Deepseek, run the following command:

```
python chat.py
```

The script will provide a summary of the company's finances based on the provided financial information. It will analyze the balance sheet, cash flow, profitability metrics, liquidity metrics, solvency metrics, cash flow metrics, and other important metrics. The script will also provide a recommendation based on the analysis.

## Output

Here is an example output from running the script on Apple for Q1 2024:

```
Ryzen@MadanDS MINGW64 ~/Downloads/FinLLM
$ python chat.py
Hi! I'm an AI that helps you perform financial analysis.
What stock do you want to analyze? For example, you can say 'I'm interested in AAPL'.
I'm interested in AAPL
Great! You've mentioned AAPL. Could you please specify the year you're interested in?
2024 q1
Thank you! You've provided the year (2024) and the period (q1) for AAPL. Give me a moment to analyze the data.
### **Financial Summary in Plain English**  

Let’s break down the company’s financial health in simple terms:

#### **1. What the Company Owns (Assets) vs. Owes (Liabilities & Equity)**
- **Cash & Investments:** $73.1 billion (a strong cash position).
- **Money Owed to Them (Receivables):** $50 billion (customers owe them money).
- **Inventory:** $6.5 billion (products waiting to be sold).
- **Total Assets:** $353.5 billion (everything the company owns).
- **Total Liabilities:** $279.4 billion (what the company owes, including debt).
- **Equity (Owner’s Value):** $74.1 billion (what’s left after paying debts).

#### **2. Income & Profitability**
- **Revenue (Sales):** $119.6 billion.
- **Gross Profit (After Cost of Goods Sold):** $54.9 billion (45.9% profit margin).
- **Operating Profit:** $40.4 billion (33.8% margin, meaning they keep ~34 cents per dollar after expenses).
- **Net Profit:** ~$33.9 billion (28.4% margin, final profit after all costs).

#### **3. Debt & Financial Health**
- **Total Debt:** $108 billion (a mix of short-term and long-term).
- **Current Ratio (Can They Pay Bills?):** 1.07 (they have just enough to cover short-term debts).
- **Debt-to-Equity Ratio:** 3.77 (high debt compared to equity, which can be risky).
- **Free Cash Flow:** $37.5 billion (money left after expenses and investments).

#### **4. Efficiency & Returns**
- **Return on Equity (ROE):** 45.8% (very high, meaning they generate strong profits from shareholder money).
- **Return on Assets (ROA):** 9.6% (good, but not as strong as ROE).
- **Piotroski F-Score:** 9/9 (excellent financial health score).

---

### **Pros & Cons**

#### **👍 Pros:**
✅ **Strong Cash Position** ($73.1 billion) means they can handle emergencies or invest in growth.
✅ **High Profit Margins** (~28-34%)—they make a lot of money from sales.
✅ **Excellent Free Cash Flow** ($37.5 billion) means they generate cash efficiently.
✅ **High Return on Equity (45.8%)**—great for shareholders.
✅ **Perfect Piotroski Score (9/9)**—financially very healthy.

#### **👎 Cons:**
❌ **High Debt ($108 billion)**—could be risky if interest rates rise or profits drop.
❌ **Low Current Ratio (1.07)**—barely enough to cover short-term bills.
❌ **High Debt-to-Equity (3.77)**—relies heavily on borrowing.

---

### **Recommendation**
### **Recommendation**
### **Recommendation**
This company is **financially strong** with high profitability and cash flow, but it carries **significant debt**.
### **Recommendation**
### **Recommendation**
### **Recommendation**
This company is **financially strong** with high profitability and cash flow, but it carries **significant debt**.

- **If you’re a long-term investor**, the strong returns and cash flow make it attractive.
- **If you’re risk-averse**, the high debt might be concerning.

⚠️ **Always do your own research before investing.** This is just a guide to help you understand the basics.

---

### **Sources**
For more detailed information, you can refer to:
- [SEC Filing (Balance Sheet)](https://www.sec.gov/Archives/edgar/data/320193/000032019324000006/0000320193-24-000006-index.htm)
- [SEC Filing (Cash Flow)](https://www.sec.gov/Archives/edgar/data/320193/000032019325000008/0000320193-25-000008-index.htm)
- [SEC Filing (Income Statement)](https://www.sec.gov/Archives/edgar/data/320193/000032019325000008/0000320193-25-000008-index.htm)