# Epidemic_Model_ORNL_Summer-2024
ORNL Internship (2024) - Epidemic Modelling <br>

During the summer of 2024, right after returning from COVID, I completed the Next Generation Pathways to Computing (NGP) Internship at Oak Ridge National Laboratory. I worked with a fellow high school student, Violet Yarkhan, and two accomplished researchers, Dr. Dilip Asthagiri and Dr. Juan Restrepo, to investigate the effectiveness of various health policies on the spread of a disease.

## Goal <br>
1. Examine the comparative effect of vaccination and social distancing policies on the maximum percent of the population infected from a given disease. <br>
2. Analyze the difference in rate of infections between populations categorized by the type of work they perform (occupational class). <br><br>

## Method <br>
A custom-modified stochasic SIR model was used to run the simulation of the epidemic in Python. By starting with a simple set of coupled differential equations from a standard SIR model, we were able to adapt it to the more complex final model. <br>

### Three classes of workers <br>
White-Collar: This population includes workers who tend to do more administrative or clerical work in offices. <br>
Blue-Collar: This segment represents workers who participate in manual labor or trade-related jobs. <br>
Stay-at-Home: This population represents the groups of people who might not work in person. For example, children, the elderly, or those who work from home are included in this population segment. <br>

### Five compartments <br>
Susceptible - the population that has not yet caught the disease but is prone to getting sick <br>
Infected - the population currently infected with the disease <br>
Recovered - the population who has already caught and recovered from the disease <br>
Dead - the population who caught the disease and died from it <br>
Vaccinated - the population who has gotten a vaccine for this disease <br>

<img width="440" height="293" alt="Screenshot 2026-09-24 114803" src="https://github.com/user-attachments/assets/a7013926-31e1-4eec-9b1b-17b0e1d02369" />


### Beta - an interaction matrix <br>
A 3x3 contact matrix showing group-by-group interaction rates. <br>

### Policy levers <br>
Vaccination - activates after a given "vaccine development" time (arbitrarily set as 10 days) <br>
Social Distancing - automatically activates after any one occupational group's infected population surpasses a given threshold (arbitrarily set at 40%) <br>

### Four simulations <br>
There were four simulations run to compare health policies: no policy, vaccination policy only, social distancing policy only, and both vaccination and social distancing policy.

## Results <br>
- Combined vaccination and social distancing policy was the most effective (12.6% reduction in overall population infections)
- Blue-collar workers expererienced the greatest benefit from the standalone social distancing policy (16.2% reduction in within-group infections)
- Stay-at-home populations were most consistently protected across policy scenarios
- The vaccination policy appeared to have very little standalone impact on the epidemic, but it was found that the peak infected value occurred before the vaccine was fully developed. Hence, **the timing of a policy implementation is just as important as the populations it targets.** <br>

## Extensions <br>
Proposed extensions include: 
- sensitivity analysis (adjusting vaccination development time and investigating impact)
- new demographic grouping (utilizing age-based or geographic population clusters)
- cost-weighted comparison (including economic costs for each policy to provide well-rounded insights) <br>

# Files <br>
*ORNL_SIR_CODE.ipynb* - the Python file of code and results plots<br>
*Examining Epidemic Models and Public Health Policy Effectiveness POSTER.pdf* - the official ORNL Internship poster product <br>
*FunctionsInfo.md* - details about input and output values for functions in Python code <br>
