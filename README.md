
# Data Modeling with Apache Cassandra

## Goal

Sparkify has been collecting on songs and user activity for their new music streaming app. One of their teams is interested in analyzing their users listening habits, which could help them classify their users for targeted ads, create/improve a recommendation algorithm for songs, and more. They are especially interested in the songs that users are playing.

Note: This project is for a fictional company and is part of Udacity's Data Engineering Nanodegree.

### Problem

Currently, Sparkify's user song data is stored in CSV format by day.
This format does not lend itself well to analysis.

### Solution

In order to enable a team to effectively gain insight from user activity, a data engineer needs to structure the data and load it into a database. The proposed plan consists of a Python ETL pipeline that will:

- Extract each CSV file.
- Transform and load the data into an Apache Cassandra database built for the analysis of song plays.

## Data

### User Song Dataset

- This dataset is a set of songs played by users.
- Each file is in CSV format and contains metadata about a song, the artist of that song, and the user.
  - ![Alt text](images/image_event_datafile_new.jpg?raw=true "User Song Dataset example")
- The files are partitioned by the day of event occurrence. For example:
    - event_data/2018-11-08-events.csv
    - event_data/2018-11-09-events.csv


## Data Model



## Installation

Clone the repo onto your machine with the following command:

$ git checkout https://github.com/wyattshapiro/sparkify_cassandra.git


## Dependencies

I use Python 3.7 and Jupyter Notebook.

See https://www.python.org/downloads/ for information on download.
See https://jupyter.org/ for information on download.

----

I use virtualenv to manage dependencies, if you have it installed you can run
the following commands from the root code directory to create the environment and
activate it:

$ python3 -m venv venv

$ source venv/bin/activate

See https://virtualenv.pypa.io/en/stable/ for more information.

----

I use pip to install dependencies, which comes installed in a virtualenv.
You can run the following to install dependencies:

$ pip install -r requirements.txt

See https://pip.pypa.io/en/stable/installing/ for more information.

----

I use a locally hosted Apache Cassandra database.

See https://cassandra.apache.org/s for more information.


## Usage

There is one main scripts:

- src/

**Steps to run**
1. Navigate to top of project directory
2. Create virtualenv (see Dependencies section)
3. Activate virtualenv (see Dependencies section)
4. Install requirements (see Dependencies section)
5. Start local Apache Cassandra server (see Dependencies section)
6. $ jupyter notebook

## Analysis


## Future Optimizations
