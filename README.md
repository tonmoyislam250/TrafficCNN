# Usage

### Data Preprocessing

To preprocess the dataset:
```
    python main.py --data --data_dir data
```

### Exploratory Data Analysis (EDA)
To generate visualizations and understand the dataset:
```
python main.py --eda --data_dir data --output_dir outputs

```

### Model Training
To train the CNN model on the preprocessed data:

```
python main.py --training --data_dir data --model_dir models --epochs 20 --batch_size 64 --learning_rate 0.001
```

### Model Evaluation
To evaluate the trained model:
```
python main.py --evaluation --data_dir data --model_dir models --output_dir outputs
```

### Inference
To make predictions on new images:

```
python main.py --inference --model_dir models --image_path path/to/image.jpg

```

### Streamlit Application
To launch the Streamlit application for interactive traffic sign recognition:

```
streamlit run scripts/streamlit_app.py -- --model_path models/best_model.h5
```
