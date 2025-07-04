# IMDB_Sentiment_Analysis
What is this Project About?

This project is part of the Microsoft Learn module "Analyze sentiment in text with Keras" and is designed for beginners to learn sentiment analysis using Azure. Sentiment analysis teaches a computer to read movie reviews and decide if they are positive (e.g., "This movie is awesome!") or negative (e.g., "This movie was terrible."). The project uses IMDB movie reviews and builds a simple neural network with TensorFlow and Keras, running in an Azure environment, to make these predictions. It’s a great way to start learning how computers understand text and how Azure supports machine learning!

Project Details

What Does the Project Do?





Goal: The project helps a computer figure out if an IMDB movie review is positive or negative by giving it a score between 0 (negative) and 1 (positive).



Dataset: It uses the IMDB dataset from Keras, which has 50,000 movie reviews (25,000 for training, 25,000 for testing). Each review is labeled as positive (1) or negative (0).



Azure Integration: The project is implemented in an Azure environment, such as Azure Machine Learning or a Jupyter Notebook hosted on Azure, to leverage cloud computing for processing and analyzing data.



Example: The code shows one review as text (e.g., "this film was just brilliant casting...") to help you understand what the reviews look like, along with its label (1 for positive).

How Reviews are Prepared





Words as Numbers: Reviews are stored as numbers, not words. Each word (like "good" or "bad") is given a number (e.g., "good" might be 50). Only the 10,000 most common words are used.



Same Length: Every review is adjusted to have exactly 256 words (numbers) by adding zeros at the end if it’s too short (called "padding").



Decoding: The code turns these numbers back into words so you can read a sample review, like a positive one praising a movie’s story and actors.

How the Neural Network Works

The project uses a neural network, like a computer brain, built with TensorFlow and Keras in Azure. It has these parts:





Embedding Layer: Turns each word’s number into a smaller set of numbers (a 16-number code) that captures what the word means.



Pooling Layer: Averages the codes for a review to make a simpler summary.



Decision Layers:





A layer with 16 units (like brain cells) that finds patterns using a math trick called ReLU.



A final layer with 1 unit that gives a score (0 to 1) using a sigmoid function to say if the review is negative (close to 0) or positive (close to 1).

What the Code Shows





Sample Review: The code turns one review’s numbers into readable text (e.g., a positive review about a movie’s casting and story) and shows its label (1 for positive).



Model Structure: It lists the neural network’s layers to show how it’s built.



Prediction Example: The code tests the model on one review, giving a score (e.g., 0.39, meaning "negative") and compares it to the real label (e.g., 0 for negative).

Skills Gained

By working on this project in Azure, you’ll learn these beginner-friendly skills:





Understanding Sentiment Analysis: Learn how computers analyze text to detect emotions (positive or negative), useful for understanding customer feedback.



Text Preprocessing: Discover how to turn words into numbers and make all reviews the same length for a neural network.



Building Neural Networks: Get hands-on experience creating a simple neural network with Keras, including layers like Embedding and Dense.



Using Azure for Machine Learning: Gain experience running machine learning projects in Azure, such as using Azure Machine Learning or Jupyter Notebooks in the cloud, to process data and build models.



Python Programming: Practice using Python libraries like TensorFlow, Keras, and NumPy to handle data and build AI models.



Reading and Debugging Code: Learn to read and understand Python code in a Jupyter Notebook, including how to fix small errors.



Data Analysis Basics: Understand how to load and explore a dataset (like IMDB reviews) and interpret model predictions.

Things to Know





No Training in the Code: The notebook sets up the model but doesn’t train it (teach it with data). Without training, predictions may not be accurate. The Microsoft Learn module explains how to add training steps, like compiling the model and fitting it to data.



Simple Model: The neural network is basic, making it easy for beginners but not as powerful as advanced models (like LSTMs).



Azure Advantage: Running this in Azure makes it easier to scale up for larger datasets or more complex models, and you’ll learn how cloud tools support AI projects.
