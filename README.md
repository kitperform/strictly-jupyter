# Strictly Open

Goal: To be the most structured, versatile, up-to-date and open Strictly Come Dancing results data resource known to us.

## Project stage

The project is currently in very early stages of discovery

- Work done so far:
  - Researched other existing projects: Four Tens, StrictlyDB. Verdict: open source projects such as Four Tens have some analysis, but not up-to-date. StrictlyDB is a website, which is closed-source and the data doesn't appear to be open.
  - Analysis of Wikipedia data. Verdict: very comprehensive and complete. Some data can be derrived from other sections, so not all of it needs processing
  - Produced a Highly normalised data model created based on analysis of Wikipedia data: https://github.com/kitperform/strictly-jupyter/blob/main/data-model.md
  - Evaluated scraping tools: Scrapy and Beautiful Soup. Verdict: use Beautiful Soup - it's comprehensive, initally got carried away with the virtue of Scrapy based on reading, but actually Beautiful Soup fits much better. Bertie had recommended this as well.
  - Avoiding the "run before walk" problem - started preparing to evaluate other projects in Jupyter but not got that far.
  - Thinking about what questions I want to answer, some notes here:
    - https://github.com/kitperform/strictly-jupyter/blob/main/scraping-evaluation.ipynb
    - also:
      - what makes a successful contestant
      - has scoring inflated over the years
      - who is more generous with scores
      - how much does judges vote versus viewer vote help contestants progress

  - Next steps:
    - add following as tickets into GitHub projects and do them: 
      - explore other projects applying Pandas to get a feel of analysis and further insight into what questions I want to answer
        - continue on with: https://github.com/kitperform/strictly-jupyter/blob/main/four-tens-experimentation.ipynb
      - prototype Beautiful Soup code to scrape data into my database model, start experimenting
        - write code to link tables via foreign keys
      - give a lightning talk at PyData Southampton on Tuesday 17 September



#### setting up on Ubuntu

sudo add-apt-repository universe
sudo apt install python3 python3-pip ipython3
sudo apt install python3.12-venv
python3 -m venv venv
pip3 install jupyter
jupyter notebook
