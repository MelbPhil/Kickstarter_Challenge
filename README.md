# Kickstarter_Challenge

## Analysis on how different kickstarter campaigns fared in relation to launch dates and fundraising goals.

### Purpose

Louise wants to know how different campaigns fared in relation to their launch dates and their funding goals. The following uses a Kickstarter dataset to visualize campaign outcomes based on their launch dates and their funding goals.

## Analysis and Challenges

The origional kickstarter data worksheet contains much more information than is required for this particular job. That being said, the primary challenge here is determining which datasets should be leveraged and/or manipulated in order to identify the trends that will be most useful for my client, Louise.

### Analysis of Outcomes Based on Launch Date

The following should help Louise determine the optimal time of year for launching a theater campaign. Constructing this chart required first converting Unix timestamps into more easily interpretable dates, and then subsequently, extracting the years from each of those dates so they could be added to a pivot table and easily filtered when performing future analysis. After removing 'live' campaigns, I was able to create the following graphic:
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106599446/171684771-faa47548-156f-4d07-899a-2a8d3f34d589.png)

### Analysis of Outcomes Based on Goals

The following should help Louise determine the liklihood of reaching various fundraising thresholds. Building the table behind this chart required carefully building a table that categorized the number of Successful, Failed and Canceled campaigns in each Goal bracket. Subsequent calculations of these numbers enabled me to determine the following percentile distribution:
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106599446/171684811-c2c36b26-522d-4e8c-8d1e-6dfdba612232.png)

### Challenges and Difficulties Encountered

I myself did not encounter any challenges in creating these tables and graphs, however could very easily imagine that someone could make a slight calculation error that would drastically impact the results of such an exercise. Being diligent in determining which columns and ranges should be leveraged is vital to acheiving success. Even the slightest of errors will carry over, impacting the entire project. Meticulous checking is key.

## Results

- **Outcomes based on Launch Date:** As shown in the above graphic, more successful theater campaigns were launched in May than any other month. Following this peak, the number of successful campaigns gradually trended down through the end of the year, with October being a slight exception. The number of failed campaigns was mostly consistant, though was slightly elevated between May and October. Regarding canceled campaigns, the number was relatively steady overal, but slightly higher in January, and not a single campaign was canceled in October.
 - **limitations of dataset:** The dataset charted here does not demonstrate that recent years have seen a drastic uptick in Kickstarter theater campaigns and with this uptick, more failures. Perhaps the increased popularity of funding theater campaigns via kickstarter has increased the possibility of failure? _Before 2013, there were much fewer campaigns per year, however none of them failed._ 
- **Outcomes based on Goals:** The chart produced here demonstrates a negative correlation between the funding goal and the chances of successfuly raching that target. In other words, higher goals saw higher percentages of failure.
 - **limitations of dataset:** The data compiled here includes all categories and subcategories of Kickstarter campaigns. Considering that Louise is interested in launching a Theater campaign, it might be more beneificial to review that subset of data as well. _Perhaps the results are being skewed by other categories?_
- **other possible tables and/or graphs that we could create:** By adding more perameters to these tables and graphics, we can determine more granular findings that might help Louise increase her odds of success. Namely, it might be interesting to review these same charts with a regional filter. Additionally, it might be interesting to know how the number of backers/average donation correlates with the success of a campaign. _Are most successful campaigns funded by a large number of people? Or do they find a small number of wealthy doners?_ There is much more usual insights within this dataset that Louise could use in determining the optimal success strategy for her next theater campaign.
