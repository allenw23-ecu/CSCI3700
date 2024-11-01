## Team Members
Will Allen

## Quick Start
Clone the Repository:
git clone https://github.com/allwnw23-ecu/CSCI3700-HW3.git

## Enter project directory
cd CSCI3700-HW3

## Install Dependencies
pip3 install Flask

pip3 install psycopg2-binary

## Enter PostgreSQL
sudo -u postgres psql

## Populate Database
CREATE TABLE basket_a ( a INT PRIMARY KEY, fruit_a VARCHAR(100) NOT NULL );

CREATE TABLE basket_b ( b INT PRIMARY KEY, fruit_b VARCHAR(100) NOT NULL );

INSERT INTO basket_a (a, fruit_a) VALUES (1, 'Apple'), (2, 'Orange'), (3, 'Banana'), (4, 'Cucumber');

INSERT INTO basket_b (b, fruit_b) VALUES (1, 'Orange'), (2, 'Apple'), (3, 'Watermelon'), (4, 'Pear');

## Exit PostgreSQL
\q

## Run Flask Application
python3 -m venv python_venv

python3 main.py

## Access Database Information:
http://127.0.0.1:5000/api/update_basket_a

http://127.0.0.1:5000/api/unique

