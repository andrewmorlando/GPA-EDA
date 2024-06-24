# GPA Analysis on Student Performance Dataset
## Initial Question:
- What features or columns of the data attribute to students having a higher GPA on average?
## Source:
- The source of the dataset is from Kaggle.com, URL: https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset
## Cleaning of the Data
- For sepecific code, please reference the notebooks along with this repository.
- .corr was originally used on the data to see if there were initial correlations that I could pick out and focus on. Other than Absences, there did not seem to be any major correlations, but some smaller correlations.
- I used boolean masking to filter out the students who hold a majority count in absences. I determined who had a majority amount of absences by adding the mean number of absences to the standard deviation of absences.
- The addition of mean and standard deviation is the main way I filtered the data to focus on what I needed to see changes to GPA. For example, Parental Support and Study Time Weekly.
## Visualization Decisions
- Since most visualizations I use will need to show comparisons of boolean masked dataframes, I decided to use line or bar graphs layered over eachother. Additionally I added the legend and changed the colors of the lines and bars for viewers to be able to distinguish the difference in data.
## Key Insights
- Realizing that abscenses are the major indicators of a student having a lower GPA; it is seen in the data that interestingly, though there is a difference in the other features between a student with high absences and the other, the differemce were not significant. This indicated to me that there is metrics that are indications of the high absences that is not covered in the survey.
- Since I cannot speculate and only analyze the data, I used boolean masking to filter out those who have high - very high parental support, and GPAs over the mean + std. Though there were minor differences, I aggregated the means to show those that have atleast a difference of .1 from the students performing lower than the mean + std.
## Future Areas of Study
- For the future I would like to incorporate other datasets that could work in tandem with this one to see other areas that could influence a students GPA.