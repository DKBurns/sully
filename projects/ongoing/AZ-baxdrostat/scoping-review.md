# Summary

This project is to conduct a "scoping review" to identify and target a number of clinical / cohort studies as well as any as-yet unidentified cost-effectiveness studies which can be used to externally validate the Baxdrostat cost-effectiveness model going to NICE this year.
# Tasks

## Backlog
I placed some of these into the slack channel to try that out, but if that method isn't nice, then we can ditch it!

### Design search strategy
Generate some formal terms using PubMed, science direct, or Scopus, whichever makes sense.

#### Tasks

- Come up with the search terms and I'll sort the searching
- We may have to resort to desk research considering the amount of grey literature involved
- Using the LLM list and filtering down to the real sources, then looking at associated papers from them (e.g. UKPDS-based studies) is probably the most efficient way, but we need to write up what our searching method is

### Conduct searches
Self explanatory. This will likely be hard work.
### Collate abstracts
I usually do a yes pile, a maybe pile and a no pile, then do a 2nd pass of the maybe pile.

Here if you could get the raw text, and/or PMID number, and/or DOI reference for all of the yes and maybe pile then we can probably do something with an LLM afterwards!


### Screen abstracts

Gruelling work, but needs doing. Possible LLM help here if we have a good enough prompt. The LLM will need the following:

- Detailed explanation of the objective of the scoping review
- Detailed spec of the baxdrostat model including the things it simulates
- Inclusion and exclusion criteria
- Dataset in a standardised format all in a GitHub repo

If each individual abstract is in a markdown format like:

```markdown
# PMID

# DOI

# Abstract

```
where the abstract text is just the raw text dump, even if we don't have a DOI or PMID the LLM can use the text there to determine relevancy and potentially identify points for comparison.

Following this, I can use `opencode` to establish and implement an agentic workflow to draft the review and propose a detailed plan for conducting the external validation.


### Collate shortlist

most likely this will be partially done by generative AI
### Get access to all papers
This is a human step. All the papers where we *need* to have full access that are not open access we will have to ask for AZ to pay for them. This is a necessary hold and hopefully will be minimal.
### Full text screening
Possibly can be done with the LLM workflow
### PRISMA diagram

I can do this in `R` or office, whichever.
### Collate extracted information
Again, probably driven by the LLM in the first instance!

### Write report
Necessary manual step, though LLM might give us a massive boost
### Send report to client

Aiming to send draft End of April if we can, might be a bit too tight though.


## WIP

### Read known materials and design extraction grid

Note that this seems to only be cost-effectiveness type modelling attempts, and doesn't have anything in it we can use to generate a comparison against a single endpoint. For example if there happened to be a study out there that had stroke incidence in a cohort of patients with rHTN, we could use our model to extrapolate that and make a comparison between what the bax model predicts vs what was seen in reality.

This would give us a strong basis to claim external validity.

Equally, decisions on assumptions, treatment combinations, efficacy, blah blah is also really important and useful.

Less important but still good to get right is things like source selection for inputs like costs, resource utilisation rates and so on.

This is one of those CE models where safety actually matters because incremental QALYs are really small. Therefore some look at how safety has been handled previously is probably quite important

We have now read through most of these papers and have a fairly good idea of what could reasonably be compared with the bax model.

This manifested 2026-04-09 in some back and forth with columns to go in the extraction grid

#### Tasks

- Help expand the columns in the extraction grid to include the important things for inclusion/exclusion criteria as well as what to extract from included studies. Please note that our extraction will include clinical studies so focus on things we'd be able to make the microsimulation model produce!
- Tell me when you've come up with a finial set of columns so I can review and tweak
- Help me go through the papers we have again to collate our current information set



### Generate inclusion/exclusion criteria

Using the reading we have done in the papers already, we should then generate some inclusion/exclusion criteria

#### Tasks

- Criteria for inclusion in external validation: Population alignment, treatment setting, things measured
- Criteria for exclusion from external validation: Population alignment, treatment setting, things measured

## Done

# Deadlines

- Client wants the whole thing end of April, but we are just going to do it as best we can
