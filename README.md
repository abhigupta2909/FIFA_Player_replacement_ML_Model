# FIFA Player Replacement ML Tool

This machine learning tool identifies potential replacements for soccer players based on various performance metrics and data-driven insights. By analyzing player statistics, the model suggests alternative players who could perform similarly or replace key players in specific roles or formations.

## Features

- **Player Replacement Suggestions:** The tool analyzes data and suggests potential replacements for transferred or unavailable players.
- **Customizable Model:** Supports fine-tuning for various teams, player positions, and strategies.
- **Performance Metrics:** Measures accuracy and other important performance indicators like true positive rate (TPR) and true negative rate (TNR).

## How It Works

1. **Data Preparation:**
   - The tool collects and preprocesses player statistics and match performance data, ensuring the dataset is clean and ready for model training.

2. **Model Training:**
   - The model is trained using player features and match performance data. It utilizes a machine learning algorithm such as Decision Tree Classifier to make predictions on potential player replacements.

3. **Replacement Prediction:**
   - After training, the model suggests suitable replacements for key players based on similar performance metrics and roles within a team. 

4. **Performance Evaluation:**
   - The model evaluates the accuracy of its predictions using common metrics such as:
     - **Accuracy Score:** Measures the overall effectiveness of predictions.
     - **Confusion Matrix:** Shows how well the model classifies correct and incorrect predictions.
     - **True Positive Rate (TPR):** Indicates how effectively the model predicts correct replacements (i.e., actual matches with predicted).
     - **True Negative Rate (TNR):** Reflects the model's ability to accurately reject poor replacement candidates.

## Results

The tool provides the following key outputs:
- **Accuracy Score:** The model's accuracy in predicting suitable player replacements.
- **Confusion Matrix:** Visualizes the classification performance, including false positives and negatives.
- **Replacement Suggestions:** A table of suggested player replacements based on historical data.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fifa-player-replacement-tool.git
   ```

2. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or script:
   ```bash
   jupyter notebook soccer_player_replacement.ipynb
   ```

## Dependencies

- Python 3.6+
- Jupyter Notebook
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

## Usage

1. Prepare your dataset with player statistics in CSV format.
2. Run the notebook to preprocess the data and train the model.
3. View the model's accuracy and suggested player replacements in the outputs.

## Evaluations

![confusion_matrix](https://github.com/user-attachments/assets/d38509fd-4f1b-4338-8388-9a74284f0cb6)

![defending_feature](https://github.com/user-attachments/assets/5e433c40-cdd5-4f09-b966-e63cc128fa1f)

![goal_keeping](https://github.com/user-attachments/assets/9b0d71f3-963f-4c76-b8bd-4207f9dd1f86)

![midfeilding_feature](https://github.com/user-attachments/assets/5889fd7a-71ce-4182-83a5-9ee8070052e8)

![stricking_feature](https://github.com/user-attachments/assets/158c0b95-897c-4013-a825-071f6d887e40)


## Example Output

| Transferred Player    | Suggested Replacement |
|-----------------------|-----------------------|
| Cristiano Ronaldo     | P. Dybala             |
| Neymar Jr             | E. Hazard             |
| P. Dybala             | A. Griezmann          |
| H. Kane               | R. Lewandowski        |
| L. Messi              | Neymar Jr             |


## Evaluation Set CSV

The `evaluation_set.csv` file contains the following columns:

- **Transferred player:** The name of the player who has been transferred or is unavailable.
- **Replacement:** The suggested replacement player for the transferred player.

Here is a preview of the CSV file:

| Transferred Player    | Suggested Replacement |
|-----------------------|-----------------------|
| Cristiano Ronaldo     | P. Dybala             |
| Neymar Jr             | E. Hazard             |
| P. Dybala             | A. Griezmann          |
| T. Courtois           | G. Buffon             |
| S. Umtiti             | David Luiz            |

You can use this CSV file as an evaluation set to test or validate the model’s predictions.

## Contributing

Feel free to submit issues or contribute to the project. Fork the repository and create a pull request with your improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
