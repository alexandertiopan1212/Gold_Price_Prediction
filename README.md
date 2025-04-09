# 📈 Gold_Price_Predictor_RBF

This repository contains a custom implementation of a **Radial Basis Function (RBF) Neural Network** to predict gold prices using historical daily data.

The project is built using Python and TensorFlow (Keras), and includes scripts for preprocessing the time series data, training the model, and visualizing predictions against actual prices.

---

## 📁 Repository Structure

```
📦 Gold_Price_Predictor_RBF
├── gold_price_data.csv       # Historical gold price dataset (daily)
├── data_preprocessing.py     # Functions to convert time series into supervised learning format
├── rbf_layer.py              # Custom RBF Layer built with tf.keras.layers.Layer
├── model_train.py            # Script to train and evaluate the RBF neural network
├── plot_results.py           # Script to visualize prediction vs actual chart
```

---

## 📌 Key Features

- ✅ Custom-built RBF Layer with trainable centers and betas  
- 🔁 Time series windowing for supervised learning conversion  
- 📉 Predicts next-day gold price based on previous N days  
- 🧠 Uses MSE loss and early stopping for optimal training  
- 📊 Includes visualization of prediction results vs ground truth  

---

## 🛠 How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Gold_Price_Predictor_RBF.git
   cd Gold_Price_Predictor_RBF
   ```

2. **Install required dependencies:**
   ```bash
   pip install numpy pandas matplotlib scikit-learn tensorflow
   ```

3. **Train the model:**
   ```bash
   python model_train.py
   ```

4. **Visualize the results:**
   ```bash
   python plot_results.py
   ```

---

## 📈 Dataset

The `gold_price_data.csv` file contains historical daily gold prices. The data is processed into a supervised format using sliding windows to predict the next day’s price based on the previous N days.

---

## 🤖 Model

The model is a custom-built RBF Neural Network using a Keras-compatible layer (`rbf_layer.py`). It maps time-series features into radial basis space before feeding to the dense output layer.

The centers and betas of the RBF units are trainable parameters learned during backpropagation.

---

## 📌 Notes

- Make sure your CSV file is properly formatted with a clean `Date` and `Price` column.
- You can tune the number of RBF units and window size in `model_train.py` for experimentation.

---

## 📬 Contact

For any questions or collaborations, feel free to reach out:

**Alexander Tiopan**  
📧 alexandertiopan1212@gmail.com  
🌐 [GitHub](https://github.com/alexandertiopan1212) | [LinkedIn](https://www.linkedin.com/in/alexander-tiopan/)

---

## 📝 License

This project is licensed under the MIT License — feel free to use and modify with attribution.

