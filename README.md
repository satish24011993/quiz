# Online Quiz App in Django

This is an online quiz organizing website project, developed using Python's web framework Django.<br>
For front-end designing we have used Twitter's front-end library Bootstrap4.

### Current Features

**Site access features:**

- Every quiz can be accessed only if the user is logged in.
- In the signing-up process the user is required to give the following information
  1.  Full Name
  2.  Email-id (unique for every user)
  3.  Mobile Number (unique for every user)
  4.  Roll No.
  5.  Password
- For login the user will be required to enter _Email-id_ and _Password_ only

**Features of each quiz:**

- The logged in user either can create his own quiz or take an existing quiz.
- For creating the quiz, the user will be required to enter the _Title_ of the quiz and questions and their corresponding options.
- Or the user can take the existing quiz.
- There will be timer of each quiz and the user is required to finish the quiz in time.
- When the timer stops, the corresponding record (i.e. number of correct answers) will be saved automatically.

**Dashboard features:**

- There are two type of dashboard
  1.  Dashboard of corresponding user
  2.  Global dashboard (i.e. Leaderboard)
- In the _Dashboard of corresponding user_ the user can see his attempted quiz statistics <br>(i.e. _No. of Correct answers_, _Marks obtained_ )
- In the _Global dashboard_ there will be overall ranking of users who have attended the corresponding quiz.

### Getting started with development

Dependenciies:

- Python 3.6.x
- Django 1.11.x
- MySQL 5.7.x
- Ubuntu 17.04 or later

#### 1. Clone this repoistory

```bash
git clone git@github.com:neeraj1909/quiz.git
cd quiz
```

#### 2. Install the [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/)

Follow [instructions on official documentation page](https://virtualenvwrapper.readthedocs.io/en/latest/install.html).

#### 3. Create the virtualenv

```bash
## run following command from `quiz` directory
mkvirtualenv quiz -a "$(pwd)" -p python3.6
```

#### 4. Install python packages

```bash
## Activate the virtualenv which you created on the last step
workon quiz
pip install -r requirements.txt
```

#### 5. Setup the database

_TODO - Add instructions for this when we start using MySQL database._

#### 6. Run database migrations

```bash
python manage.py migrate
```

#### 7. Run development server

```bash
python manage.py runserver
```

#### 8. Implementation of Timer

_TODO - Implementation of timer for the quiz still have to be done._
