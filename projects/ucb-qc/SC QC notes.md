
Running the App Errors:
- (Treatment Costs Pane) Shared input/output ID was found The following ID was used for more than one input/output: "inputTreatmentCosts": 1 input and 1 output (Look at inputsCostsIN.R and inputsTreatmentCosts.R)
- (Economic Outcomes Pane) Duplicate input IDs were found error - The following IDs were used for more than one input/output: "resultSubsetSelector": 2 inputs (Look at resultsEconomicServer.R)

Visual Scan of Code: 
App.r : 
- Should avoid hardcoding numbers (lines 447, 450, 462, 480 and 481)
- Argument typo error on line 371 "patter" 
- Starting at line 524, multiple cases of "relapse" spelled "relpase" consistently
- Starting at line 590 and for all other "need" validation blocks, the severe populations ask for non-severe inputs. 
- Line 1829 - Cycle length is explicitly made weekly with hardcoding, may give problems if want to change to monthly at some point
- Line 539 onwards, "worsen" and "stable" checks could be predefined instead of manually written out repeatedly
- Line 643 and onwards for generating the Markov trace; this could be written as a function to prevent repetition, passing the function with the arguments for the few parameters that do change between the treatment arms (population, comparator etc). 

UI issues:

