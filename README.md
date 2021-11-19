[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/27410/https://github.com/27410/group-assignment-2021-group_7_p_inhibens_gsm.git/main)

# 27410 - Group assignment - Group 7 - Genome scale model of the marine bacteria P. inhibens

> Dear students, thank you for accepting the group assignment. Please fill in the
> requested information below and above ([Group Number] and [TITLE]) and remove this quoted part before submission (everything prepended with a >).
> Please also replace `[PUT-YOUR-REPOSITORY-HERE]` up in the first line 👆 with the name of your repository here on GitHub.
> That way someone can click on the Binder badge icon and open your project in Jupyter lab to explore it.
> For this to work you will also have to keep `requirements.txt` up to date (by running `pip freeze > requirements.txt`).
> Furthermore, this will only work if you decide to make your repository public (which you can do under Settings -> Options),
> which I would encourage you to do – up to you. A lot of good science happens out in the open these days.
> Good luck!

## Project summary (<300 words)
Our objective is to generate and validate this new GSM from P.inhibens. Also, we want to maximize the production of tropodithietic acid (TPA), a valuable compound with various properties.

For it we've been following all the steps we've been learning throught the different assignments.

We used CarveMe to generate a model from NCBI data, and we made a gapfilling with LB and another with M9 media and adust it later.
We also adjust the ATP maintainance reacion to a realistic value.
After collecting some basic information, we started analyzing our S matrix. The model, comprising 1131 genes of the total 3974 genes of the assembly, includes 1774 metabolites that participate in 2688 reactions. 87 genes were found to be essential for the growth of P. inhibens.

A map of the reaction network was generated for a more visual approach to this model using escher.
Then we proceeded to solve the model and find the fluxes with CPLEX, which we could represent in a number of plots.

Finally, a simplified TDA production pathway was added. The model objective was set to growth, TDA and 20% growth + TDA, respectively. The model proved to yield a decent TDA production, even with a minimum growth.

## Project overview
Describe how your project is organized ...

The main code is in the "GSM code" file. There's also a Memote report, "MEMOTE_RESULTS_GRAPHIC".  The Central Carbon Pathway created with escher is called "Cental Metabolism.json". We also have a notebook where we try all our code called "Testing_code.ipynb". The other files are either models generated by our code, or test files that are not really that important for the final understanding of the project.
