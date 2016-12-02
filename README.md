wiki_node_disambiguation
- - -

# What's this ?

- You can run "Wikification" as easy as possible.
    - According to wikipedia, [Wikification](https://en.wikipedia.org/wiki/Wikification) is `in computer science, entity linking with Wikipedia as the target knowledge base`
- You can get disambiguated result with its score.


# Requirement

- Python3.x (checked under )
    - I recommend to use "Anaconda" distribution.

# Setup

`python setup.py install`

## To those who uses interface.predict_japanese_wiki_names()

You're supposed to have mysql somewhere.

The step until using it.

1. start mysql server somewhere
2. download latest mysql dump files
3. initialize wikipedia database with mysql


To download wikipedia dump files, execute following commands

```
wget https://dumps.wikimedia.org/jawiki/latest/jawiki-latest-redirect.sql
wget https://dumps.wikimedia.org/jawiki/latest/jawiki-latest-page.sql
```

To initialize wikipedia database with mysql,

```
% mysql -u [user_name] -p[password] wikipedia < jawiki-latest-redirect.sql
% mysql -u [user_name] -p[password] wikipedia < jawiki-latest-page.sql
```

# Change logs

- version0.1
    - released
    - It supports only Japanese wikipedia
