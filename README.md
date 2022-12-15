
# ![igboAPI](https://user-images.githubusercontent.com/36100251/203620969-25db849c-3060-49a1-a43e-2c56afee68ca.svg)

The aim of this project is to enhance the current process of importing and adding new lexemes from [igboAPI](https://igboapi.com/) into Wikidata. 
This entailed tweaking the [`tfsl`](https://phabricator.wikimedia.org/source/tool-twofivesixlex/) package to import the Igbo API dataset to the Wikidata Lexicographical data project.



## Background
Igbo is one of the three major languages in Nigeria, with approximately 30 million Igbo people around the globe1. Despite its enormous population, Igbo culture is experiencing social violence against its language in many Nigerian homes, schools, churches, governmental organizations, and even neighboring dialectal regions. Igbo has been relegated to a second-class language when compared to English which is seen by many Nigerians as the language of prosperity and opportunity. This social violence has become so consistent and aggressive that UNESCO has predicted Igbo could become extinct by 2025.

In the past decade, we have witnessed incredible technological advancements surrounding language technology and natural language processing. Language technology has been applied to solve many real-world problems that revolve around language. However, many African languages, Igbo especially, have not been able to take advantage of these advancements due to the lack of fundamental lexical resources. For instance, there is no widely accepted, easily accessible, online, standardized Igbo dictionary. The greatest challenge in creating a robust Igbo dictionary is properly cataloging, labeling, organizing, and linking the  known Igboid dialectal varieties. So far, all existing attempts at creating an Igbo dictionary mainly focus on Standard Igbo or one other dialect and therefore are only widely accepted by speakers of that particular dialect. Researchers1,2 have shown that for an Igbo dictionary to be widely accepted by the whole Igbo community it needs to be able to accommodate Igbo dialects besides Standard Igbo. This will make the dictionary more reliable and robust because most Igbo content (social media, news articles, etc.) combine a range of dialects.

## Solution 2: Data sharing and Wikidata syncing
The activities of this work package includes:
- Periodically dumping all Igbo API word data: Snapshots of the Igbo API dataset will be placed on the Igbo API website twice a year in the formats of JSON or CSV.
- Adapting existing Wikidata data importing script(s): We will explore automated approaches (either by creating a new script or adapting an existing one) to import the Igbo API dataset to the Wikidata Lexicographical data project. Wikidata aims to provide metadata for words (or what they call items) in many languages thereby creating a knowledge base across languages.
- Deliverable: Enhancing the current process of importing and adding new lexemes into Wikidata via a publicly accessible API. As a proof of concept, 500 Igbo words will be imported into Wikidata Lexicographical data


## Setup
Clone this repository.
Make sure this ends up in your PYTHONPATH.

By running export PYTHONPATH=$PYTHONPATH:/path/to/tfsl in your terminal


While using windows you may need to add the cloned directory in your python path locally.

follow below steps to add the directory to your python PATH

-Click on PC, hover your mouse to the right side where we have evices and Drives. Right click and choose properties
-Clicking on the Advanced system settings in the menu on the left.
-Clicking on the Environment Variables button o​n the bottom right.
-In the System variables section, selecting the Path variable and clicking on Edit. The next screen will show all the directories that are currently a part of the PATH variable.
-Clicking on New and entering Python’s install directory.
or 
-Copy the path of Python folder.
-Paste path of Python in variable value. Click on Ok button: Click on Ok button:


Now install its dependencies, again substituting the path accordingly:

pip install -r /path/to/tfsl/requirements.txt



# How to Run

