#football-match-prediction-random-forest
A machine learning project that predicts football match outcomes using a Random Forest model.


This project focuses on predicting the outcomes of football and other sports matches using machine learning, specifically through the Random Forest algorithm. The idea behind the work is to use historical match data from twelve different sports and build a model that learns the relationship between teams, scores, and winners. After training, the system allows the user to choose a sport and select two teams, and then the model predicts which one is more likely to win. The goal of the project is to demonstrate how data science can be used to analyze competitive sports and provide meaningful predictions.

The project was developed inside the VSCode environment and is organized into two main sections: a backend written in Python and a simple frontend built with HTML, CSS and JavaScript. The backend handles tasks such as loading datasets, preprocessing data, encoding team names, training the machine learning model and generating predictions. The frontend provides a clean and easy interface where users can simply choose the sport and teams they are interested in. Together, these components create an end-to-end system capable of performing automated match predictions.

<img width="573" height="268" alt="Picture1" src="https://github.com/user-attachments/assets/f42c8631-9bd5-429b-866a-550faf45127b" />


To prepare the data, all twelve datasets were first loaded and cleaned. Since the datasets came from different sources, their column names were inconsistent. This required normalizing them so the model could understand them properly. After that, the names of the teams were encoded into numerical values using Label Encoding because machine learning models cannot work with text directly. When this preprocessing was completed, the Random Forest Classifier was trained on the cleaned data. This algorithm was chosen because it is powerful, reliable and able to recognize complex patterns in large datasets.

<img width="616" height="93" alt="Picture2" src="https://github.com/user-attachments/assets/2f562903-266c-4054-b7fc-3dfc444fb400" />
<img width="616" height="122" alt="Picture3" src="https://github.com/user-attachments/assets/96afc19d-e648-4239-b157-af13a0b6ea8b" />
<img width="616" height="46" alt="Picture4" src="https://github.com/user-attachments/assets/5f181f0b-d536-4f7f-8297-2d3f2e00dc88" />
<img width="616" height="120" alt="Picture5" src="https://github.com/user-attachments/assets/19369e98-a1d0-4856-a8ef-92cc998dcdb9" />


Once the model was trained, it was able to make predictions with an accuracy of about seventy percent. Considering the diversity of the sports and the limited features available in the dataset, this accuracy is a promising result. The model benefits from having access to a large amount of match data across different sports and from the robustness of the Random Forest technique. The system then takes the user’s input—two chosen teams—and uses the trained model to determine which team has a higher chance of winning.

A simple graphical interface was created to make the system easy to use. Through the frontend, users can select the type of sport, pick their two teams and then submit the form to display the predicted winner. The design is intended to be straightforward so that even someone without technical knowledge can interact with the model without difficulty.

<img width="616" height="280" alt="Picture6" src="https://github.com/user-attachments/assets/03a4f045-0226-431f-b0e9-6ca39aca2aa3" />

Despite the model’s solid performance, the project encountered some challenges. One issue was the problem of unseen labels, which happens when a team exists in the prediction request but not in the training data. Without having seen that team before, the model cannot encode it properly. Another limitation is the absence of important real-world variables such as team tactics, weather conditions, player injuries or recent form, all of which can strongly influence sports outcomes but were not included in the dataset.

There are several meaningful directions for improving this work in the future. Adding more features to the dataset would immediately help the model understand matches more deeply. Including recent team performance, match location and goal statistics could significantly increase accuracy. Experimenting with more advanced machine learning models, such as XGBoost or neural networks, would also be a natural next step. Another improvement could involve adding real-time match analysis so the system can update predictions based on live data. With these enhancements, the project could evolve into a much more sophisticated and highly accurate prediction tool.
