# Sully's README

## The idea

Keeping everything on paper in a private GitHub repo serves several tasks at
once:

- Provides a way to keep everything down on paper:
  - General line management
  - Task delegation and status
  - Learnings/notes (e.g., 1:1 meeting notes)
  - Feedback
  - Examples of things in code
- Gives some practice: with
  - working with `git`
  - collaborating on code
  - `markdown`, which we use a lot
- Always have access to change things
- Flexible:
  - doesn't need immediate action so can work into day(s)
  - Can be changed to whatever kind of format works best:
    - One central document with everything
    - Folders by project
    - Any other kind of arrangement you like!
- Software agnostic: you only need a text editor and `git`

## Process

```mmd
A
B
C
D


A --> B
B --> C
C --> D



```

## Working days

Monday, Wednesday, Thursday to match up with the internal meetings at
DPA

## Objectives

Just a rough list of general objectives at the moment!

- Learn the ropes!
- Get 1:1s with everybody to help get settled
- Finish all of the DPA courses
- Upskill in the use of `R`
- Figure out project management with GitHub
- Help me with project work!

## Projects

### UCB QC

Main task is to help me get the QC done as I can't do it alone given all
the other stuff I'm juggling at the moment

1. Tasks

   For most of these, I'll be working in parallel to you already. Don't
   worry about posting the same issue, I'll consolidate everything at
   the end.
   1. Code/technical

      Basically, help me make a strategy for technical QC!

      Are there any materials in the app itself which explain the
      conceptual model? Does that model match what's happening in the
      code? Is there any code which is really difficult to read or
      understand?

      This, plus me checking with Shubhram/April will determine
      whether we have to ask for more materials in order to do the QC
      properly, as we need to know the conceptual model and whether
      the model matches that, and whether it makes sense!

      Could you try to work your way down `app.R` and come up with a
      list of things where I can help and/or explain things?

      At the moment, it looks like the entire app basically feeds into
      `generate_markovtrace` in quite a reactive way so
      it's always recalculating if it passes the validation at the
      top, so I would advise trying to work your way back from there
      to the raw data in the calculation chain, and collating anything
      you can see which isn't right or is hard to follow

   2. Server

      There's plenty to talk about in the server, and I've raised some
      issues already. Feel free to raise more and categorise them etc

   3. UI

      Point out UI issues with screenshots and circles in issues.

      use snipping tool `ctrl + win + s` and there's a setting to
      draw on it. you can paste things directly into the GitHub issue
      and it'll work whilst you're typing.

### Bax ongoing project

- We have a project which involved converting a VBA-based microsim into
  R, so a really good learning case for you.
- It uses some advanced `R` applications, especially around the use of
  `data.table` as a state object to give a cross-sectional snapshot of
  the population which gets updated every cycle, rather than row updates
- I'll get you access to this repo so you can have a look

1. Code task

   In terms of help, the immediate task is to extend the way AEs are
   incorporated into the model by allowing a rate for 1st cycle and
   another rate for subsequent cycles after the AE. This is because it
   was being massively overestimated in the existing model. This will
   require a small structural change to the model.

   What I would like you to do as a bit of a challenge/learning chance
   is:
   - Make an issue themed around your reading/learning
   - Make a branch associated with that issue
   - Explore the current (very large) codebase, and have fun comparing
     it to the Excel/VBA model versions (I'll send you the version
     associated with v1.0 release, and the new one with the amendment
     to AEs in it)
   - See if you can isolate the part where AEs are being applied in the
     current model. This is more difficult than it sounds as you'll
     find when you drill down in the code
   - Write into the issue description via `… -> Edit` at the top of
     the issue what your plan would be to extend the current AE
     modelling
   - Let me know when you've had a chance to think about it. This might
     take a while, and I may have made changes by the time you get
     there, but that's what your branch is for as it will freeze time
     within your branch

### BD

1. AZ proposals
   1. New one for full model build

      RFP came through 27th. Rob responded yesterday morning. Proposal
      deadline is April 17th, but it's for a large project. I'll get
      details from Rob today

   2. Bax external validation scoping review proposal
      - Bit like a TLR, but probably don't have time to do formal TLR
      - Folder access with examples in it already, client informed of
        us of this yesterday

   3. Bax external validation proposal
      - Email from client
      - Jeiling mentioned something to do with another external
        validation that's done already and how we could draw
        inspiration from that
