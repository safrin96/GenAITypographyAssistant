# Typography Layout Assistant with Generative AI

An AI-driven web application designed to simplify typographic design decisions by generating intelligent, visually appealing, and context-aware layouts. Leveraging machine learning, deep learning, and modern web development, this app assists designers in creating custom typography layouts based on user input, sentiment analysis, and device type selection.

## 📖 Project Overview

Typography is an essential component of visual design but often requires expertise and time. This project automates typography suggestions by analyzing text sentiment, understanding context, and generating responsive layouts with a generative model. The app also includes user account features, layout history filtering, and font customization, providing a robust, personalized experience.

### Key Features

- **Real-Time Typography Preview**: Live updates as users input text.
- **User Accounts**: Secure user registration and login, allowing users to save and view their typography history.
- **Dark/Light Mode Toggle**: User-friendly interface customization.
- **Design History with Search and Filter Options**: Access to past typography suggestions with search and filter functionality based on text and tone.
- **Text Tone Analysis**: Adjusts typography suggestions based on text sentiment.
- **Responsive Layout Options**: Generates layouts optimized for desktop, tablet, and mobile devices.
- **Downloadable Image and SVG Export**: Allows users to download generated layouts as images or SVG files for further customization.

## 🚀 What You’ll Achieve

This project offers hands-on experience with:
- **Full-Stack Web Development**: Integrating machine learning with Flask for a functional, user-friendly web interface.
- **Deep Learning for Typography Generation**: Leveraging PyTorch and TensorFlow to create personalized layout suggestions.
- **Interactive Front-End Design**: Using HTML, CSS, and JavaScript to develop a responsive, interactive user experience.
- **Database Integration**: Using SQLAlchemy to manage user data, history, and font uploads.
- **Data Analysis and NLP**: Employing text sentiment analysis to align typography with tone.
- **Responsive Design**: Ensuring optimal layouts across devices for consistent UX.

## 📂 Data, Tools, and Libraries

### Data

- **Fonts and Layouts**: A variety of font files and predefined layouts to train and validate the model.
- **User Input Data**: Captures text input, device type, font choices, and stores layout history.

### Tools

- **Generative AI Models**: Uses neural networks to generate typography layouts based on user input and sentiment analysis.
- **Flask and SQLAlchemy**: Flask serves as the web framework, and SQLAlchemy manages user and history data.
- **HTML/CSS/JavaScript**: For the front end, creating an intuitive user interface with interactive features.

### Libraries

The project utilizes several libraries (specified in `requirements.txt`):
- **torch** and **tensorflow**: Power the generative AI model and layout suggestions.
- **flask** and **flask-login**: Serve the application, manage authentication, and handle requests.
- **flask-wtf**: For managing secure form inputs, including file uploads.
- **pillow**: For image creation and manipulation.
- **requests**, **matplotlib**, and **pandas**: For API requests, data manipulation, and visualization.
- **textblob** and **transformers**: Handle text tone analysis to adjust layout style.
- **scikit-learn**: For data processing and model evaluation.

## 📈 Project Files and Code Overview

### Core Components

1. **app.py**:  
   The main Flask application file that handles user input, generates typography suggestions, and manages routes for registration, login, history, and font uploads.

2. **typography_model.py**:  
   Defines the deep learning model for generating typography layout suggestions based on user input.

3. **context_analysis.py**:  
   Uses OpenAI’s API and transformers to perform sentiment analysis on input text to adjust typography based on tone.

4. **responsive_layouts.py**:  
   Generates device-optimized layout images based on text, device type, and selected font. Images are saved directly in the `static` folder for display in the web app.

5. **recommendation_engine.py**:  
   A reinforcement learning-based engine that refines layout suggestions based on previous user feedback.

6. **font_downloader.py**:  
   Downloads and manages fonts required for typography suggestions, storing them in the `static/fonts` directory.

7. **data_processing.py**:  
   Manages text and image preprocessing, including loading fonts, manipulating layout dimensions, and optimizing for different devices.

8. **Templates** (`register.html`, `login.html`, `history.html`):  
   HTML templates for registration, login, and history pages. Includes search and filter options in the history template to improve navigation.

## 🔧 Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/typography-layout-assistant.git
   cd typography-layout-assistant
   
2. Install Requirements:

    ```bash
    pip install -r requirements.txt

3. Run the Application:

    ```bash
    python app.py

4. Access the App: Open http://127.0.0.1:5000 in your browser to start generating typography suggestions.

## 🎨 Screenshots

Add screenshots here to demonstrate the various features of the application:

1. Main Page: Highlighting the text input, device selection, and theme toggle.
2. Font Selection: Dropdown for selecting from available and uploaded fonts.
3. Real-Time Preview: Demonstrates the live preview feature while typing.
4. Generated Layout with Suggestions: Shows the suggested layout, tone analysis, and download options.
5. History Page with Search and Filter: Displaying search and filter fields, along with a list of past typography suggestions with thumbnails.

## 🛠 Future Improvements and Additional Features

Here are additional features and improvements you might consider:

1. User Profile Management: Allow users to update their profile information and manage saved preferences.
2. Advanced Typography Controls: Enable custom adjustments to font size, color, and spacing directly in the preview.
3. Enhanced SVG Export Options: Provide advanced export settings, allowing users to tailor SVG properties.
4. Integration with Design Tools: Allow users to export layouts directly to tools like Adobe Illustrator or Figma.
5. Tagging and Categorization: Allow users to tag and categorize layouts in their history for better organization.

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues, create pull requests, or suggest new features. Follow the standard GitHub flow for contributing: fork the repository, make your changes, and submit a pull request.

## 📝 License

This project is licensed under the MIT License.
