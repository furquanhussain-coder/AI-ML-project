# create a virtual environment on mac and windows

# Mac
python -m venv venv_name
python -m venv "ssm"

# activate the venv_name
source ./venv_name/bin/activate
source ./ssm/bin/activate

# windows
python -m venv venv_name

# activate the venv_name in windows
./venv_name/Scripts/activate

# terminal - ls to see the list of files
clear - clear the terminal

# check the libraries in this environment
pip3 list


# install the back end depeendcies from requirements.txt
cd backend

pip install -r requirements.txt

python -m data.load_data - only to test load_data function - optinal

python -m train_and_save - this is important

curl -fsSL https://claude.ai/install.sh | bash

https://bbycroft.net/llm

# to run your backend
python -m app

<!-- 
curl -X POST http://localhost:5000/predict \
  -H "Content-Type: application/json" \
  -d '{
    "total_bill": 25.50,
    "sex": 1,
    "smoker": 1,
    "day": 1,
    "time": 1,
    "size": 2
  }' -->

# to run your fornt end
in a new terminal
cd frontend
pip install -r requirments.txt
