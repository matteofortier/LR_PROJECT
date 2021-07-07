### MVP

*Matteo Fortier*

The focus of the project is to model which aspects of a course impacts the overall satisfaction score of a university coures the most.

![figure](/lasso_path.png)

The 26 student survey features were aggregated into 8 features representing the category of survey features: 'teaching', 'opportunities', 'feedback', 'support', 'management', 'resources', 'community', and 'voice'. A lasso regression model was then fitted to produce a Lasso path graph to show how coefficients are zeroed with increasing/decreasing regularization. This graph potentially shows which groups of survey questions are most significant in impacting overall statisfaction score. 

The figure shows that the top 3 most significant group of questions are:

1. Teaching
2. Management
3. Support

Regarding 'Teaching', this would mean universities should seek to improve the following scores if to improve overall satisfaction:

- Staff are good at explaining things
- Staff have made the subject interesting
- The course is intellectually stimulating
- My course has challenged me to achieve my best work

