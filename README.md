# Hotel-Bookings-
In this project, I take on the role of a Data Scientist for a hotel management company.  
The objective is to build a machine learning model that predicts whether a hotel booking will be canceled.

Accurate cancellation prediction helps hotels:
- Reduce revenue loss
- Improve resource planning
- Optimize room allocation
- Design better pricing and overbooking strategies

---

## Business Problem

Hotel cancellations directly impact revenue and operational efficiency.  
By predicting cancellations in advance, hotels can:

- Implement targeted retention strategies
- Adjust pricing dynamically
- Optimize staffing and inventory
- Minimize financial losses

This project builds a classification model to predict booking cancellations based on customer and booking attributes.

---

## Dataset Description

The dataset contains booking information including:

| Feature | Description |

| hotel | Hotel type (Resort/City) |
| lead_time | Days between booking and arrival |
| arrival_date_year | Year of arrival |
| stays_in_week_nights | Weekday nights booked |
| stays_in_weekend_nights | Weekend nights booked |
| adults | Number of adults |
| children | Number of children |
| babies | Number of babies |
| meal | Type of meal booked |
| country | Customer country |
| market_segment | Booking market segment |
| distribution_channel | Booking distribution channel |
| is_canceled | Target variable (0 = Not Canceled, 1 = Canceled) |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Seaborn & Matplotlib
- Scikit-learn
- Jupyter Notebook / Google Colab

---

## Project Workflow

### 1️⃣ Data Cleaning
- Removed leakage features (`reservation_status`, `reservation_status_date`)
- Handled missing values
- Standardized column names
- Feature engineering:
  - `total_guests`
  - `total_nights`

### 2️⃣ Exploratory Data Analysis (EDA)
- Cancellation rate analysis
- Impact of lead time
- Effect of market segment
- Country distribution
- Correlation heatmap

### 3️⃣ Feature Engineering
- Created total guests feature:
total_guests = adults + children + babies
- Created total nights feature:
total_nights = stays_in_week_nights + stays_in_weekend_nights

### 4️⃣ Encoding & Preprocessing
- One-hot encoding for categorical variables
- Train-test split
- Feature scaling (if applicable)

### 5️⃣ Model Building
Models implemented:
- Logistic Regression
- Random Forest Classifier
- (Optional: Gradient Boosting / XGBoost)

### 6️⃣ Model Evaluation

Evaluation metrics used:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Score

---

## 📈 Key Insights

- Longer lead times increase cancellation probability.
- Certain market segments have significantly higher cancellation rates.
- Country and distribution channel influence cancellation behavior.
- Random Forest captured non-linear relationships better than Logistic Regression.

---

## 📂 Project Structure

hotel-booking-cancellation/
│
├── data/
├── notebooks/
│   └── Hotel_Booking_Model.ipynb
├── requirements.txt
└── README.md

---

## 🚀 How to Run

1. Clone the repository:
https://github.com/lindahsimotwo/Hotel-Bookings.git
2. Install dependencies:
pip install -r requirements.txt
3. Run the notebook.

---

## 💡 Future Improvements

- Hyperparameter tuning
- Handling class imbalance (SMOTE)
- Feature importance visualization
- Model deployment using Streamlit
- Real-time cancellation risk dashboard

---

## 👩‍💻 Author

**Lindah Chelimo**  
Telecommunication & Information Engineering  
Machine Learning & IoT Enthusiast  

---

## ⭐ If you found this project interesting, consider giving it a star!
