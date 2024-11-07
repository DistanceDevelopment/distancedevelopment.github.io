---
title: "New CRAN release of `mrds` and `Distance` R packages"
description: "Announcing new major releases of the mrds package, version 3.0.0, and Distance package, version 2.0.0."
date: November 2024
categories: [camera traps, analysis] # self-defined categories
image: distance_ctds.png
draft: false # setting this to `true` will prevent your post from appearing on your listing page until you're ready!
---

Over the past months we have been working on improving performance when fitting conventional distance sampling (CDS) detection functions - i.e., detection functions with distance as the only covariate.  The results of this work is implemented in the new `mrds` version.  Most users will see no change except perhaps for a speed-up in model fitting.  However, users fitting functions with multiple adjustment terms or with challenging data (such as overdispersed data that tends to come from camera trap distance sampling data) may find improvements in model fit.  For such data we had previously recommended downloading the `MCDS.exe` binary file, but this is no longer needed (although the option remains available). Our thanks to Felix Petersma for leading this work on CDS performance improvement.

Changing the optimization methods is judged to be of a change that we have updated the major version number of the `mrds` package to 3.0.0.  Because the `Distance` package uses `mrds` for detection function fitting, we have also updated this package's version number to 2.0.0.

For more details on the optimizer changes, see the package NEWS files:
* [`mrds` NEWS](https://cran.r-project.org/web/packages/mrds/NEWS)
* [`Distance` NEWS](https://cran.r-project.org/web/packages/Distance/NEWS)

As always, thank-you to those who have made feature requests or reported issues. If you do find any problems, or want to suggest a new feature, please feel free to raise an issue at either
* [`Distance` issues](https://github.com/DistanceDevelopment/Distance/issues) or 
* [`mrds` issues](https://github.com/DistanceDevelopment/mrds/issues)

Lastly, advance notice that we have been working on a number of other improvements to our distance sampling software and training: a new version of Distance for Windows, an updated free online introductory workshop and refreshed web pages including software examples.  We anticipate making an announcement about all this in the next few weeks.
