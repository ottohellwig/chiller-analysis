<a name="readme-top"></a>

# Chiller Data Analysis

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#operation-analysis">Operation Analysis</a>
      <ul>
        <li><a href="#percentage-operation-activity">Percentage Operation Activity</a></li>
        <li><a href="#operation-activity-over-hours-of-day">Operation Activity Over Hours of Day</a></li>
        <li><a href="#operation-activity-over-days-of-the-week">Operation Activity Over Days of the Week</a></li>
        <li><a href="#monthly-operation-activity">Monthly Operation Activity</a></li>
      </ul>
    </li>
    <li>
      <a href="#kWE">kWe Analysis</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#kWR-and-COP">kWR and COP Analysis</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#references">References</a></li>
  </ol>
</details>

# Operation Analysis

## Percentage Operation Activity
The percentage operation activity is when the chiller is functioning and can be defined as the rows at which kWE is greater than 0 (kWE>0).
<p align="right">(<a href="#readme-top">back to top</a>)</p>


##  Operation Activity Over Hours of Day
**Analysis:** The operating activity and time have a monotic correlation, the line, despite being nonlinear does not increase nor decrease significantly. There is a gradual decrease in the operating activity from 01:00 to the minimum value at 11:00. The operating activity then increases until it reaches maximum operating activity. The operating activity is not an exact representation of the total as it only represents 1 chiller. Thus, the explanation behind the decreased operation activity may be a result of other chillers functioning as the current chiller may be used as a reserve.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Operation Activity Over Days of the Week
**Analysis:** There is a  positive correlation between ascending days of the week and operating activity. The weekend have the highest maximum values and this may be a result of facilities being used more frequently on these days. The results are predominantly inconclusive as there is limited information which can be inferred from the data.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## Monthly Operation Activity
**Analysis:** The monthly operation activity presents a gradual positive correlation between the ascending series of months and the operating activity. From Janurary to September, the operating activity is moderately increasing with a decline from September to October and a recurve back to December. This may be due to the study semesters at the facilities increasing the foot traffic and applying more pressure on the chiller functioning. This decreases with October which is towards the end of the year and is when holidays become apparent.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

# kWE Analysis

## Average kWE (Chiller Energy Consumption) Over Hour of Day
**Analysis:** The relationship between kWE and time is monotonic, with the kWE starting at approximately 40kW at the start and end of a day. The kWE increases from 06:00, peaks at 14:00 and then progressively decreases back to a steady state level. This correlation can be linked to the peak times of facility use at QUT facilities during the afternoon. Residual heat energy from the surrounding area may also contribute to the higher level of energy consumption between those times. 
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## kWE Average of Days of Week
**Analysis:** The average kWE over the days of the week are similar with a gradual decrease from Monday to Wednesday, then increasing to Friday and decreasing till Sunday. There is limited information which can be extracted from this data, the energy input has little differentiation from Monday to Sunday.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## kWE Average of Months in Year
**Analysis:** There is a monotonic correlation between the kWE and months in a year. The relationship mimics the shape of a parabola and indicates that the average energy input of the chiller is significantly lower from May to August with the minimum being between June and July. This may be due to holidays, maintenance of the chiller or other chillers have higher precedence in comparison to chiller 1 during those months. The kWE then increases back to a steady state level of about 70kW of kWE.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

# kWR & COP Analysis

## kWR (Kilowatts of Refrigeration) & COP (Coefficient of Performance)
The constant value (density of water @ a specific temperature) was assumed to be 997kg/m^3 and was used to calculate the kWR using the formula (Evans, 2017):

<p align="center"> <u> kWR (kW) = m (Mass) * Cp (Specific Heat Capacity) * ΔT (Change in temperature). </p>
    
The COP can be formulated using the equation (Langer, 2022): 

<p align="center"> <u> Q/W or energy output/energy input. </p>
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## kWR Plots
The kWR can be defined as the amount of heat energy transferred from the chiller to the condenser and is measured in Kilowatts. The average kWR was defined as the mean and was assigned to the y axis, time indices (Hours in a day, days in a week and months in a year) were assigned to the x axis. The error bars represent standard error which is defined as the standard deviation.

**Analysis:** The average kWR and hours in a day have a monotonic correlation with an increasing curve from 06:00 to 20:00. This also has a positive correlation with the kWE values, as the kWE has mimics the kWR as they are codependent. The increased energy input results can also be seen in the increased usage of the refrigeration. Thus, the kWR increases from 06:00 and progressively decreases as there is less usage of energy/heat transfer.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## COP Plots
The COP can be defined as the efficiency of heat energy transferral and is measured in dimensionless. The average COP was defined as the mean and was assigned to the y axis, time indices (Hours in a day, days in a week and months in a year) were assigned to the x axis. The error bars represent standard error which is defined as the standard deviation.

**Analysis:** There is a positive nonlinear relationship between the kWE and kWR whereas the COP remains constant at a mean value of 9. The kWR has a steep incline from 14:30 onwards and peaks at 1000kWR and mimics the relationship of kWE.
<p align="right">(<a href="#readme-top">back to top</a>)</p>


## References
Evans, P., 2017. Chiller Cooling Capacity – How to calculate. The Engineering Mindset.  <https://theengineeringmindset.com/chiller-cooling-capacity-calculate/>.

Langer, R., 2022. Coefficient Of Performance – What is a Good COP For Heat Pump.  PickHvac. <https://www.pickhvac.com/heat-pump/basics/cop/>.
<p align="right">(<a href="#readme-top">back to top</a>)</p>
