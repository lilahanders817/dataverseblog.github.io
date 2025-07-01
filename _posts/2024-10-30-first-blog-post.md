## Grappling With Uncertainty in Forecasting the 2024 U.S. Presidential Election 

**Andrew Gelman, Ben Goodrich, and Geonhee Han** </br>
**Harvard Data Science Review** </br>
**October 30th, 2024** </br>

Looking back on the 2024 U.S. presidential election, headlines were filled with polls and predictions. Where were these numbers emerging from? Behind the articles were several statisticians and political scientists that jointly collaborated on a probability model that was made to address the uncertainty involved in American democracy. </br>

In the paper titled “Grappling with Uncertainty in Forecasting the 2024 U.S. Presidential Election”, the authors Andrew Gelman, Ben Goodrich, and Geonhee Han, who worked with The Economist, detailed how they built and updated their election forecast model. As someone interested in data science and its applications in various fields, I found the paper to be an engaging reflection on what it really means to predict the future. </br>

The model they built is Bayesian, which means it outputs a range of possibilities instead of one fixed outcome. For example, in July (when Biden was still in the race), the model gave the Republican candidate a 51% chance of winning the popular vote and 75% chance of winning the Electoral College. By September, after Harris replaced Biden, she was projected to win 52% of the popular vote, but only had a 50% probability of winning the Electoral College due to how votes are distributed geographically. Researchers highlighted that the gap between vote share and electoral power is easy to overlook, but crucial to accurately predicting the projected candidate. </br>

One important challenge the authors addressed was calibration over time. If a model jumps from saying a candidate has a 90% chance of winning to only 10% a week later, something’s wrong (forecasts should evolve with new data, but they shouldn’t swing dramatically).This matters because models must distinguish genuine shifts in voter preferences from transient sampling variability or measurement noise. To do that, the authors set constraints on how volatile national opinion is allowed to be based on historical patterns. </br>

Even though the model runs on code, it reflects human decisions: what to include, how much to trust polls, and how to deal with surprises. For instance, they didn’t explicitly model the possibility that a major-party candidate might be replaced until Biden dropped out. They also admit that some variables, like Supreme Court decisions or felony convictions, are hard to quantify. Instead of ignoring these factors, the authors try to incorporate them into the model’s error terms or leaving room for uncertainty. </br>

After the polling misses in 2016 and 2020, many people are skeptical of poll-based forecasts. The authors attempt to confront this by constructing a model that allows for polling errors at both national and state levels, and they’ve tried to include a wide range of uncertainty. However, they note an interesting omission: their model doesn’t explicitly account for the fact that polling errors are autocorrelated, or if polls were biased in one direction last time, they’re likely to be biased in the same way this time. While they assume pollsters correct their methods, this assumption might mean underestimating systemic error. </br>

I was impressed by how self critical the authors were. They openly discuss where things could go wrong, what assumptions they made, and how unexpected events challenged their approach. People often expect forecasts to be exact indicators of what's to come and this paper is an important reminder that good forecasting is about accounting for uncertainty and not pretending to eliminate it completely. </br>
