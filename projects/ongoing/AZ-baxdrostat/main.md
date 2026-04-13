
# Bax ongoing project

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
