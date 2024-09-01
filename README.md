**Setting Up WeatherApp on Your Local Machine**

**Prerequisites**

Before you begin, make sure you have the following installed on your local machine:

- [Python 3.10.7](https://www.python.org/downloads/release/python-3107/): Make sure you have Python 3.10.7 installed. You can download it from the official Python website.

**Step 1: Clone the Repository**

1. Clone the Copilot repository from the source code repository using the following command:

        git clone <repository\_url> 

1. Navigate to the cloned repository using the following command:

        cd WeatherApp

**Step 2: Create and Activate a Virtual Environment**

1. Upgrade **pip** to the latest version by running the following command:

        python -m pip install --upgrade pip 

1. Install **virtualenvwrapper-win** to manage virtual environments on Windows:

        python -m pip install virtualenvwrapper-win 

1. Create a new virtual environment named **venv**:

        python -m virtualenv venv

1. Activate the virtual environment:

        venv\Scripts\activate 

**Step 3: Install Dependencies**

1. Install the required Python packages listed in the **requirements.txt** file using the following command:

        pip install -r requirements.txt 

**Step 4: Run the copilot Service**

1. Start the app service by running the following command:

        uvicorn app.server:app --host 0.0.0.0 --port 5000 --reload 

The app service should now be up and running on your local machine.
