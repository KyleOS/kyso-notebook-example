# This is the template for the Kyso template library 😉

## Installation

Git clone this repository:

```
git clone https://github.com/KyleOS/airtable-sales
```

Download and install the [Anaconda Python distribution](https://www.anaconda.com/distribution/).
Then active a conda virtual environment with

```
conda env create -f environment.yml
conda activate dev
```

## Installing libraries

Install any libraries you need with

```
conda install <library>
```

Make sure to run the following command to save the installed libraries into the environment.yml file,
this allows others to run the report easily

```
conda env export --no-builds > environment.yml
```

## Airtable

Airtable Python uses Requests, which you can install by running:

```
conda install -c anaconda requests -y
```

Note that you will need to generate an API key for your account if you haven’t already. You can do this in your [Airtable account settings](https://airtable.com/account).
It is bad practice to have your API keys in the code you are running. Instead, we can set a global variable in our ~/.bash_profile. Copy your API key to the clipboard. Open your bash profile in your preferred editor and enter the following:

```
export 'AIRTABLE_API_KEY' = "API_KEY"
```

replacing “API_KEY” with the string you just copied.

From the command line, run:

```
source ~/.bash_profile
```

Airtable’s REST API interface can be found here: https://airtable.com/api. We are now ready to start using Airtable Python.


## Usage

Start programming! Open jupyter with

```
jupyter lab
```

And start working.

## Sharing

Push to Github and import into Kyso.