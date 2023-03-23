![Highest-paying degrees banner](./img/banner.png)

Hey there!

This repository contains all the code for my story for the San Antonio Express-News that looks at the highest-paying bachelor's degrees in the San Antonio area.

The story is based on data from the U.S. Department of Education's College Scorecard, which is a database of information on colleges and universities in the United States. The data is available on the [College Scorecard website](https://collegescorecard.ed.gov/data/). You can find the main analysis in `notebooks/san-antonio-major-earnings.ipynb` jupyter notebook.

**Specifics of the analysis:**
- Data were pulled March 16, 2023.
- The U.S. Department of Education [says](https://collegescorecard.ed.gov/data/) that the data was last updated September 14, 2022.
- Median income figures are based on students who **graduated during award years 2014-15 and 2015-16** and who **accepted federal aid during their studies**. The scorecard [sources its income figrues](https://collegescorecard.ed.gov/assets/FieldOfStudyDataDocumentation.pdf) from administrative tax records maintained by the IRS within the Department of the Treasury.
- Not all median income figures are publicly available. If class sizes were too small, their data was hidden for privacy reasons.
- If the scorecard's data provided a median income figure for a major while listing 0 graduates for that major, it suggested that either that program was no longer offered at that school or there was a mismatch of data. Refer to page 12 of the education department's [technical documentation](https://collegescorecard.ed.gov/assets/FieldOfStudyDataDocumentation.pdf) for more information. During my analysis, I found two programs with zero graduates. I chose to filter them out of my analysis.
- Only bachelor's degrees were analyzed for this story.

## How to replicate

If you'd like to run the code yourself, use the following steps:

1. Clone the repo.
2. Install the requirements with `pip install -r requirements.txt`.
3. You can either run the jupyter notebook or `cd` into the notebooks folder and use the `nbexec get-coordinates.ipynb` command to run it as a script.