# Kickstarter_Challenge

## Is the success of a kickstarter campaign influenced by its launch date or fundraising goals?

### Purpose

My client (_Louise_) is planning on launching a kickstarter campaign for her new theater production. In preparation for this, she wants to know how past kickstarter campaigns have fared in relation to their launch dates and their funding goals. The following analysis leverages a kickstarter dataset to visualize how campaign outcomes (_'successful'/'failed'/'canceled'_) correlate with their launch dates and their funding goals.

## Analysis and Challenges

The raw kickstarter data for this project contains far more information than is required for this particular job. The primary challenge here is in determining which datasets should be leveraged and/or manipulated in order to identify the trends that will be most useful for my client. 

### Reviewing Outcomes Based on Launch Date

The following should help Louise determine the optimal time of year for launching a theater campaign. Constructing this chart required first converting Unix timestamps into easily interpretable dates. By constructing a pivot table, and using proper filters, I was able to create the following graphic:
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106599446/171684771-faa47548-156f-4d07-899a-2a8d3f34d589.png)
Interpretation found below.

### Reviewing Outcomes Based on Goals

The following should help Louise determine whether increasing or lowering her kickstarter's fundraising goal will impact its liklihood of succeeding. Constructing the table that is powering this chart required outlining multiple sets of criteria _('outcomes'/'goal amount'/'play subcategory')_ for determining which datapoints should be counted within each bracket. Subsequent calculations of these numbers enabled me to determine the following percentile distribution:
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106599446/171743802-6e2aefca-30a4-4928-abf1-9ab48272243b.png)
Interpretation found below.

### Challenges and Difficulties Encountered

I myself did not encounter any challenges in creating these tables and graphs, however could very easily imagine that someone could make a slight calculation error that would drastically impact the results of such an exercise. Being diligent in determining which columns and ranges should be leveraged is vital to acheiving success. Even the slightest of errors will carry over, impacting the entire project. Meticulous toubleshooting is key. For instance, someone could easily forget to include one of the filters while reviewing 'Outcomes Based on Goals', and thus, they will be working with faulty data. 

## Results

- **Outcomes based on Launch Date:** As shown in the above graphic, more successful theater campaigns were launched in May than any other month. Following this peak, the number of successful campaigns gradually trended down through the end of the year. _(October was a slight exception, having more successful kickstarter launches as compared to September.)_ The number of failed campaigns was slightly higher between the months of May and October, otherwise was mostly consistent year round. The number of canceled campaigns was relatively steady overal, _(slightly higher in January, and not a single campaign was canceled in October.)_ **The data appears to suggest that the optimal time of year for launching a kickstarter campaign for a theater production will be in the early spring, _(Around May.)_ The end of the year is the worst time to launch a kickstarter campaign fora theater production. _Almost half of campaigns launched in December failed._**
   - **limitations of dataset:** This chart does not effectively demonstrate how recent years have seen a drastic uptick in kickstarter theater campaigns, or how this recent uptick has corresponded with more failed and canceled campaigns. Perhaps the increased popularity of funding theater campaigns via kickstarter has increased the possibility of failure: _Before 2013, there were much fewer campaigns per year, and none of them failed._ In light of this, it might be interesting to review how a campaign outcome correlates with the # of other productions actively being funded at the time of launch.
- **Outcomes based on Goals:** **The chart produced here demonstrates a predomenantly negative correlation between the funding goal and % of campaigns acheiving success,** _however, this trend breaks down once the goal is above roughly $30,000, (reasons for which I explain below)._
    - **limitations of dataset:** Roughly 96% of theater kickstarter campaigns are seeking less than $25,000. With significantly less campaigns seeking over $25,000, the upper end of our dataset is significantly less likely to be predictive of an overarching trend, and morelikely to be skewed by unique sets of circumstances. _Although the data here does seem to suggest that 66% of theater productions with a goal of $35,000 to $44,999 are successful, this statistic very well may **not** persist with an increased sample size. 
- **Other possible tables and/or graphs that we could create:** As mentioned above, it might be interesting to review how a campaign outcome correlates with the # of other productions actively being funded at the time of launch. Additionally, it might be worth knowing how the number of backers/average donation correlates with the success of a campaign, this could provide my client with information on how she should consider marketing her production. _Are most successful campaigns funded by a large number of people? Or do they find a small number of wealthy doners?_ And my final suggestion for now, how does the location of the project impact liklihood of success?
