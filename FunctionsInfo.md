# Python Code Specifics - Function Information

## Functions <br>
### sir_system_implicit <br>
#### Inputs <br>
*vars* - 1x15 matrix consisting of the updated population values for S,I,R,D,V groups for each of three occupational classes <br>
*S_prev* - 1x3 matrix showing the previous population value for each occupational class' susceptible group <br>
*I_prev* - 1x3 matrix showing the previous population value for each occupational class' infected group <br>
*R_prev* - 1x3 matrix showing the previous population value for each occupational class' recovered group <br>
*D_prev* - 1x3 matrix showing the previous population value for each occupational class' dead group <br>
*V_prev* - 1x3 matrix showing the previous population value for each occupational class' vaccinated group <br>
*beta* - 3x3 contact matrix showing group by group interaction dynamics <br>
*gamma* - 1x3 matrix of recovery rates per occupational group <br>
*death* - 1x3 matrix of death rates per occupational group <br>
*mu* - 1x3 matrix of rate of immunity loss by occupational group <br>
*c* - rate of infection overall, regardless of occupational class <br>
*v_rate* - 1x3 matrix of rate of vaccination by occupational group <br>
*econ_impact* - the impact on interaction of developing a vaccine stage <br>
*distancing_impact* - the impact of social distancing policy on interaction <br>
*dt* - time step <br>
*is_development_phase* - boolean determining whether vaccination funnels can be activated in simulation <br>
*stay_at_home* - boolean determining when social distancing policy is enabled within simulation <br>
<br>

#### Outputs <br>
*function* - 1x15 matrix with the updated populations per occupational class in S,I,R,D,V groups <br>

### sir_model_implicit_euler_matrix
#### Inputs
*S0* - 1x3 matrix of initial susceptible population values per occupational group <br>
*I0* - 1x3 matrix of initial infected population values per occupational group <br>
*R0* - 1x3 matrix of initial recovered population values per occupational group <br>
*D0* - 1x3 matrix of initial dead population values per occupational group <br>
*V0* - 1x3 matrix of initial vaccinated population values per occupational group <br>
*beta* - 3x3 contact matrix showing group by group interaction dynamics <br>
*gamma* - 1x3 matrix of recovery rates per occupational group <br>
*dt* - time step <br>
*death* - 1x3 matrix of death rates per occupational group <br>
*mu* - 1x3 matrix of rate of immunity loss by occupational group <br>
*v_rate* - 1x3 matrix of rate of vaccination by occupational group <br>
*econ_impact* - the impact on interaction of developing a vaccine stage <br>
*distancing_impact* - the impact of social distancing policy on interaction <br>
*T* - total time in days the simulation runs <br>
*c* - rate of infection overall, regardless of occupational class <br>
*development_time* - time in days until vaccine is developed/implemented <br>
*stay_threshold* - the trigger amount for social distancing policy (will go into effect when any occupational class population hits threshold amount infected) <br>
*vaccination_policy_enabled* - boolean to determine if vaccination policy is simulated in overall model <br>
*social_dist_policy_enabled* - boolean to determine if social distancing policy is simulated in overall model <br>
<br> 

#### Outputs
*S_list* - the population values after every timestep of the susceptible group per occupational class <br>
*I_list* -  the population values after every timestep of the infected group per occupational class <br>
*R_list* - the population values after every timestep of the recovered group per occupational class <br>
*D_list* - the population values after every timestep of the dead group per occupational class <br>
*V_list* - the population values after every timestep of the vaccinated group per occupational class <br>

