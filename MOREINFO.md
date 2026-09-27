# More Information About the Code

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
*is_development_phase* - boolean determining whether vaccination funnels are active <br>
*stay_at_home* - boolean determining whether social distancing policy is enabled <br>

#### Outputs <br>
*function* - 1x15 matrix with the updated populations per occupational class in S,I,R,D,V groups <br>

### sir_model_implicit_euler_matrix
#### Inputs
#### Outputs


## BLAH BLAH

