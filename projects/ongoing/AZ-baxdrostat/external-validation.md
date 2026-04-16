# Overview

<<<<<<< HEAD
=======
This project is located here in the google drive: [AZ2602](https://drive.google.com/drive/folders/1Il8k2azMZiMQT3mgzAlqefPzqMzF09iM?usp=drive_link). The proposal for this workstream is [this one](https://docs.google.com/document/d/1bF7SnGzNFyWN9ZtxJuYPTqZ6VXuAS-f8f_AAKQoTnZQ/edit?usp=sharing). Let me know if you don't have access and I'll give it to you.

As of 2026-04-10, this project is partially blocked by `projects/ongoing/AZ-baxdrostat/scoping-review.md` because we don't yet know what things we will have to do to the `R` model to externally validate it against sources we do not know yet.

However, we can already be making changes to the code to validate against the sources we know we will need to validate against. This includes several of the studies we have already identified in the scoping review.

Summary

### 1. The Core Problem: Baxdrostat is a "Time Traveler"

Baxdrostat is a revolutionary new drug for treatment-resistant hypertension. From its clinical trials, AstraZeneca knows it does one thing really well: **it lowers blood pressure very fast.**

But here is the problem: Healthcare payers (like the NHS or insurance companies) don’t care about blood pressure numbers. They care about _events_. They want to know: _"How many heart attacks, strokes, and kidney failures will this drug prevent over the next 10 to 20 years?"_ Because Baxdrostat is brand new, we don’t have 20 years of data. We can't wait 20 years to find out. So, we have to build a mathematical time machine (the microsimulation model) to predict the future.

### 2. What is a Hazard Ratio (HR)?

To predict the future, we need a mathematical multiplier for risk. That multiplier is the **Hazard Ratio (HR)**.

Think of a Hazard Ratio like a car insurance multiplier:

- **HR = 1.0:** The drug does nothing. Your risk of a heart attack is exactly the same as if you took a sugar pill.
    
- **HR > 1.0:** The drug is actively harming you (e.g., HR 1.2 means a 20% _higher_ risk).
    
- **HR < 1.0:** The drug is protecting you.
    

For example, if the baseline risk of having a heart attack is 10%, and a drug has a Hazard Ratio of **0.80**, the math is simple: $10\% \times 0.80 = 8\%$. The drug reduced the absolute risk to 8%.

### 3. What is the "Treatment Effect"?

The "Treatment Effect" is the bridge between the short-term trial data and the long-term future.

We know Baxdrostat lowers blood pressure by, say, 10 mmHg. But how do we turn "10 mmHg" into a Hazard Ratio for heart attacks?

This is exactly why we found that **2021 BPLTTC paper**. It acts as our universal translator. It says: _"Based on 350,000 patients from history, every time you lower a 65-year-old's blood pressure by 5 mmHg, their Hazard Ratio for a heart attack becomes 0.91."_

So, if Baxdrostat lowers blood pressure by 10 mmHg (which is two "5 mmHg units"), the model does the math: $0.91 \times 0.91 = 0.828$.

Boom. We just calculated Baxdrostat's Treatment Effect. We now know Baxdrostat reduces the risk of major cardiovascular events by about 17% in that patient.

### 4. Why We Care So Much About "Control Groups"

You asked a brilliant question: _"If Baxdrostat is revolutionary, why are we looking at all these papers that don't even mention Baxdrostat, like QRISK4, Schlaich, and Azizi?"_

It all comes down to **Validation**.

Before we can ask the model to predict the _future with Baxdrostat_, we have to prove that the model perfectly predicts the _present without Baxdrostat_.

Imagine building a simulation of a car race. Before you test how fast a new Ferrari (Baxdrostat) can go, you have to prove your simulation perfectly obeys the laws of physics on a normal track with a normal Honda Civic (the Control Group / Standard of Care).

This is how we validate the model:

1. **The Baseline (QRISK4 & Azizi):** We program our virtual patients to be sick, resistant-hypertensive adults on standard medications. We let the simulation run for 10 years.
    
2. **The Check:** We look at the results. Did 10% of our virtual patients have a heart attack? Did their kidneys fail at the exact speed predicted by the **Schlaich 2025** paper?
    
3. **The Green Light:** If our "virtual control group" perfectly matches the real-world control groups from the literature, the model is **validated**. The Evidence Review Group at NICE will say, _"Okay, we trust the engine of your model. It reflects reality."_
    

### The Grand Finale

Once the control group is validated, we run the model _again_. But this time, we give the virtual patients Baxdrostat.

The drug lowers their blood pressure. The model applies the BPLTTC Hazard Ratios. The heart attacks drop. The kidney failure slows down. We compare the "Baxdrostat Run" against the "Control Run," and the difference between the two is the exact number of lives saved and millions of dollars saved for the healthcare system.


# Tasks

- [ ] Using what we get from the extraction to think about methods for showing alignment in the model code
  - [ ] Development of functions to setup and execute the simulation such that we can examine alignment with external source(s)
  - [ ] Probably one function per external source [ ] Probably a larger function for doing a Frankenstein's monster type validation exercise (with argumentation against us cherry picking)
- [ ] Conducting the external validation
  - [ ] Iterative design of the main function as we develop source-specific functions
  - [ ] Documenting the functions abut also the methodology / process for the report
  - [ ] Writing the introduction section of the report
We will be making functions in the future that compares the model outcomes to outcomes from included appropriate papers. 
Work backwards from the outcomes in Baxdrostat, find what's needed. 


