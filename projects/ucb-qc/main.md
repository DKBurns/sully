# UCB QC

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
