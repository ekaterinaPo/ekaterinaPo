# Hi, I'm Kate 👋

**Data Scientist / Data Analyst** based in the New York area | 10+ years in accounting, including the UN (UNDP)

I build machine learning models and deploy them to production on AWS. I also read data with an accountant's eye: in client work, that meant catching data leakage and hidden business requirements before they reached the model.

## 🛠️ Core Stack

| | |
|---|---|
| **Languages** | Python · SQL (CTEs, window functions) · Scala |
| **ML & Deep Learning** | Scikit-Learn · XGBoost · PyTorch · TensorFlow · CNN / U-Net · RNN · Transformers |
| **Data & Statistics** | Pandas · Spark · SciPy · statsmodels · hypothesis testing · time series (Prophet, ARIMA) |
| **LLM & Agents** | LangGraph · Claude API · Text-to-SQL agents · token-cost profiling |
| **Cloud & MLOps** | AWS (SageMaker, Lambda, S3, EventBridge, EC2, ECR) · Docker · GitHub Actions · Apache Airflow |
| **Apps & APIs** | FastAPI · Flask · Streamlit |
| **BI & Visualization** | Power BI · Tableau · Plotly · Matplotlib · Seaborn · Advanced Excel |

## 📊 Featured Projects

### [UN SDG SQL Agent](https://github.com/ekaterinaPo/un-sdg-analytics-platform) - LangGraph · Claude API · SQLite · Python
A LangGraph agent that answers plain-English policy questions over UN Sustainable Development Goals data (193 countries, 123 indicators, 293K data points). It inspects the schema, writes its own SQL, checks the result and retries when needed. Every question, query, answer and token cost is logged. I worked inside the UN system at UNDP before moving into data, so this one is personal.

📌 Cut cost per question from $0.39 to $0.06-0.13 (up to 85% lower) by profiling agent runs. The number of agent turns, not schema size, drove cost; a local entity resolver and a cached schema removed the wasted turns.

### [LandCover Segmentation](https://github.com/ekaterinaPo/LandCover) - PyTorch · AWS Lambda · S3 · Docker · GitHub Actions
Multi-class semantic segmentation of satellite images with a U-Net model, built to help agricultural companies assess farmland suitability. Deployed on AWS Lambda with three serving paths: automated S3-triggered batch, a Streamlit UI and a FastAPI REST API.

📌 CI/CD with GitHub Actions for Docker image updates cut deployment time from hours to minutes.

### [Credit Card Fraud Detection](https://github.com/ekaterinaPo/credit-card-fraud-detection) - Python · scikit-learn · XGBoost · imbalanced-learn
Classification on 284,807 transactions where only 0.17% are fraud. Compared Logistic Regression, Random Forest and XGBoost with three imbalance strategies (SMOTE on training data only, class weights, scale_pos_weight), evaluated on PR-AUC instead of accuracy.

📌 XGBoost reached PR-AUC 0.881 (83.7% recall, 87.2% precision). Treating the threshold as a business decision (€200 per missed fraud, €10 per false alarm) moved the optimal cut-off from 0.5 to about 0.35, lowering total expected cost.

### Dynamic Pricing Model - Beam Data Inc. (client work, code not public) - AWS SageMaker · Lambda · EventBridge
Practicum project for a car-sharing client of a data consulting firm.

📌 Built an automated retraining pipeline (EventBridge → Lambda → SageMaker) and delivered a production-ready pricing model within 10 days of a scope change. Flagged data leakage from post-trip variables not available at booking time, and found that discount logic had to be applied after prediction.

### Airline Sentiment Pipeline - [pipeline](https://github.com/ekaterinaPo/airlines) · [dashboard](https://github.com/ekaterinaPo/airlines_dashboard) - Airflow · RoBERTa · AWS S3 · Streamlit · Docker
A daily Airflow DAG pulls Twitter mentions of three Canadian airlines, classifies each tweet with a pretrained RoBERTa sentiment model and stores results in S3. A Streamlit dashboard reads and visualizes them.

### Other Work
📌 [Statistics for Data Science](https://github.com/ekaterinaPo/statistics-for-data-science) - article and notebook series on core statistics, using real Olympic data (in progress).

📌 [Bank Marketing in Scala](https://github.com/ekaterinaPo/BankMarketing-MLinScala) - logistic regression, SVM, gradient-boosted trees and random forest in Scala to predict telemarketing success (University of Toronto course project).

## 💼 Before Data: 10+ Years in Accounting
- **UNDP, Minsk** - Finance Clerk: payments, financial reports and cost-recovery billing for UN agencies; processed 100+ payments a day within 3-day deadlines.
- **Sporting Club LLC, Minsk** - Accountant: automated quarterly reporting in Excel (8 hours → 15 minutes); developed an accounting method for restaurants that the Ministry of Trade of Belarus adopted as a countrywide standard.
- **Taxology CPA, Ontario** - Accountant & Bookkeeper: full-cycle bookkeeping and tax for a multi-client portfolio; built consolidated reporting for two projects totaling about $7M.

This is why I ask "does this number make sense?" before "how accurate is the model?"

## 🎓 Education
- MLOps Engineering Program - Toronto Institute of Data Science and Technology (WeCloudData)
- Certificate in Data Science & AI - University of Toronto
- MSc Economics - Belarusian State University
- BSc Economics & Management (cum laude) - Belarusian National Technical University

## 🌍 Languages
English (fluent) · Russian (native) · Belarusian (native)

## 📫 Let's Connect
LinkedIn: [linkedin.com/in/pogrebnyakova](https://linkedin.com/in/pogrebnyakova)
