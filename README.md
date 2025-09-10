**Overview**

The COVID Analysis and Mapping of Policies (AMP) is part of the COVID-Local suite of free resources developed for local decision-makers. The COVID AMP Policy and Plan Database includes a library of polices from US states and the District of Columbia, US local governments (counties, cities) and national governments globally.

COVID AMP is an on-going research effort with data collection performed by researchers at the Georgetown University Center for Global Health Science and Security. As of July 2021, data are most complete for US states, and county-level policy data are available for select localities. This work continues to expand to include new county- and state-level data across the US and country-level data globally, however the addition of new policies stopped on June 1, 2021. In addition, a dataset of COVID-19-related plans published by US states and other organizations is also being collated and is available on the site.

The site includes:

A searchable, filterable database of all policies and plans in the dataset, including legal and governance analysis. The complete dataset can be downloaded in an Excel file format directly from the site. If you are interested in establishing an API or other direct access, please contact us at globalhealthsecurity@georgetown.edu. 
An interactive policy map providing geospatial visualization of the policies implemented over time. Policies can be viewed by any combination of key policy types or by “Distancing level” (see Methods below for detailed information about these categories). All policy maps include COVID-19 case counts, over time, either as an average of new cases in the last 7 days or cumulative cases.
An interactive location profile that displays policies and caseload over time. Each state or country that enacted policies has a page displaying a timeline of cases overlaid with policies and a breakdown of the policies enacted, by policy type (e.g., social distancing, enabling and relief, etc.).
An interactive tool to explore the intersection between policies and caseload for each US state. The tool also provides the ability to:
Compare the effect of not having implemented any policies
Evaluate new policy options given conditions in a state
This work and underlying AMP dataset are available for use under the Creative Commons Attribution By License agreement (https://creativecommons.org/licenses/by/4.0/), with appropriate reference and acknowledgement of the original research team, as available under the About section of https://covid-local.org and https://covidamp.org.

In addition to direct download from the site, we are happy to work with your team to provide automated access via API or other data sharing method. Please contact us at globalhealthsecurity@georgetown.edu for more information.

**COVID-19 policy database documentation**
_Policy data coding process_

To collect the data, the team first developed a custom data taxonomy and data dictionary to define key metadata and organize the dataset. These data are populated directly by the policy coding team into Airtable and transferred via API into a database on Amazon Web Services. These data may be accessed directly from the backend database via API upon request. The data dictionary with complete description of all metadata fields can be downloaded as an Excel file here. The complete dataset can be downloaded from the Policy data page from covidamp.org/data.

For the purpose of this effort, policies are defined as government-issued and backed by legal authority or precedent. Policies are coded and tagged with the relevant metadata manually. Each policy is tagged with a series of descriptive attributes based on a review of the policy language, including (this is a representative subset – see data dictionary for full description of data fields):

Policy name and description
Policy type (e.g., executive order, emergency declaration, statute, etc.)
Categorical description of the scope of policy actions (e.g., social distancing, travel restrictions, enabling and relief measures, support for public health and clinical capacity) as well as more granular subcategory tagging (e.g., face coverings, quarantine, private sector closures, school closures, etc.)
Authorizing role enacting the policy (e.g., governor, mayor, health official, president, city council, etc.)
Start/end dates, including anticipated end dates for those policies still in effect but with declarative expirations
Information about the geographic regions where the policy applies (if different from the level at which the policy was enacted)
Researchers review public sources to identify policies, with the most common sources including government websites that collate policy announcements, either COVID-19-specific or more generally. If a documented policy is not available or where there are questions about the policy, researchers contact local public communications or other offices to confirm. A static copy (PDF or screen capture) of each policy is stored with links to any sites with associated policy announcements in the dataset.

Legal experts review each policy following entry into the dataset to identify and code relevant authorities underlying the policy. This review is ongoing and data from the legal review are continually added to policies in the dataset. In addition, for policies in the US, this data collection includes capturing attributes of the US state with respect to how legal authority is allocated between the local and state government (see definitions for Dillon’s Rule and Home Rule states in the data dictionary available from the AMP documentation page).

Policies listed under the Omicron response include all travel restriction policies issued on or after November 26, 2021.

_COVID-19 plan database documentation_

Plans included in the dataset are documents issued by a government, non-profit, for-profit, or higher education institution that provide recommended actions or guidelines, but do not necessarily have legal basis or authority.

Plans are recorded under a different coding scheme than policies, because plans in AMP are not required to be government-issued or backed by legal authority or precedent. In addition to providing a PDF of the plan, data captured for plans includes (this is a representative subset – see data dictionary for a full description of data fields):

Plan name and description
Name and type of the organization that authored the plan
Information about topics covered in the plan, based on the plan type (e.g., what aspects of school operations are addressed in a government plan; what aspects of operations are addressed in a private sector plan; etc.)
Whether the plan was authored by an entity with authority to enact the plan elements

**Policy map**

The policy map visualizes the policies in effect over time as well as a distancing level determined by analyzing policies in place on a given day (see below). A date slider on the map page provides the ability to select a date or date range over which to compare the policies in effect in a given category, or view distancing level over time. State-level data are available for 50 US states, the District of Columbia, and Puerto Rico (US only view). Country-level policies are available for select countries globally, including sub-national policies for select locations. Expansion of coverage to additional countries is ongoing and are added to the map and policy library as policies are coded by the research team.

_Visualizing distancing level, as analyzed from policies_
Distancing level reflects a general description of the status of an area’s COVID-19-related social distancing policies at a given point in time. Distancing levels are categorized as: Lockdown, Stay-at-home, Safer-at-home, Partially open, and Open. These categories are intended to reflect the combination of policies that, taken together, have been used to mitigate COVID in communities globally.

The distancing status of each location is captured based on a day-by-day analysis of policies in effect for each state, over time, that address school closures, private sector closures, and mass gathering restrictions. To determine distancing level, explicit policies are considered first and that status is used (e.g., stay-at-home policy for stay-at-home distancing level) so long as it addresses the defined combinations of school closures, private sector closures, and mass gathering restrictions listed for each distancing level below. In cases where an explicit policy is in place, but subsequent policies related to social distancing counteract key elements used in the definition of distancing level considered here, the distancing level is determined using the rules below. For example, a stay-at-home order that subsequently relaxes (lifts) private sector closures prior to the end of the stay-at-home order is considered in a safer-at-home status for the purposes of distancing level in COVID AMP. Finally, the rules also serve as the basis for determining distancing level when no explicit policy is in place, but policies addressing school closures, private sector closures, and mass gatherings exist. The definition for each distancing level is included and the bullets that follow reflect the conditions used to differentiate each status.

_Lockdown (Phase I)_: Policies do not allow residents to leave their place of residence unless explicitly permitted to do so

For the purposes of determining distancing level in AMP, lockdown is defined by:

- Lockdown order in place (e.g., includes provisions requiring no movement outside or limits those leaving home for essential functions to specific household members or to only some days of the week)


_Stay-at-home (Phase II)_: Policies limit most in-person activities and social events

For the purposes of determining distancing level in AMP, stay-at-home is defined by simultaneous closure of schools, private sector businesses, and restrictions on mass gatherings and events, as captured by the policy tagging completed by the research team. Stay-at-home distancing level is captured based on one or more policies, as follows:

- Stay-at-home order in place, targeted at the general population
- OR Combination of policies that include all of the following:
    - School closures AND
    - Private sector closures AND
    - Mass gathering and/or event restrictions
 
      
_Safer-at-home (Phase III)_: Policies limit activities to those specifically permitted, encouraging extra precautions and retaining limits on mass gatherings

For the purposes of determining distancing level in AMP, safer-at-home is defined as continuing school closures, partial reopening of the private sector (either as specified in a safer-at-home order or through a combination of stay-at-home order plus relaxed private sector restrictions), and ongoing mass gathering restrictions (though they may be relaxed relative to stay-at-home conditions):

- Safer-at-home order in place
- OR Stay-at-home order in place with simultaneous policies that relax restrictions on (reopen) the private sector
- OR Combination of policies that includes all of the following:
    - School closure AND
    - Private sector closure with some relaxation from prior, most restrictive policies AND
    - Mass gathering and/or event restrictions with some relaxation from initial, most restrictive policies
 
      
_Partially open (New normal/Phase IV)_: A majority of public restrictions on mass gatherings and non-essential businesses are lifted or expired, with some policies in place on private sector reopening, use of face coverings or adaptation and mitigation measures like enhanced cleaning protocols

Partially open distancing level is defined as:

- No stay-at-home or safer-at-home order in place (including by expiration)
- Some restrictions on either mass gathering or private sector businesses
- Includes reopening policies for private sector and/or mass gatherings
- Can include face mask or adaptation and mitigation policies
- Schools may or may not be reopened

_Open_: All policies on mass gatherings and non-essential businesses, including policies governing reopening guidelines, are lifted or expired. There may be some other policies in place such as quarantine guidelines for travelers, visitor restrictions or prison population reductions

These conditions are similar to those prior to the pandemic for any policy related to movement and interactions between individuals:

- No stay-at-home or safer-at-home order in place
- No private sector closures, and no re-opening specific policies
- No mass gathering restrictions, and no re-opening specific policies
- No school closures in place
- No face mask or adaptation and mitigation policies in place


_Visualizing policies in place, by category, over time_

To visualize policies of different types in effect over time, the map queries the policy dataset by date and location. Policies can be viewed by category on the map, including any combination of policies and/or their subcategories:

- Social distancing
- Authorization and enforcement
- Contact tracing/Testing
- Emergency declarations
- Enabling and relief measures
- Face mask
- Military mobilization
- Support for public health capacity
- Travel restrictions
Policies can be filtered by single categories (e.g., social distancing) or multiple sub-categories (e.g., isolation, lockdown, quarantine) to view what kinds of policies were in effect or not in a given location on the selected date, and how many. Other categories include private sector closures, school closures, mass gatherings, and more. On the map, darker-shaded locations have more policies in effect on the selected date belonging to the selected category or sub-categories, with the darkest location having the most.

_Location profiles_

To view how the policy response unfolded over the course of the pandemic, each country and U.S. state where policies were collected has a specific page devoted to that location’s policy environment. At the top of the page, a pandemic timeline of the location’s cases is overlaid with policies, using the 7-day moving average of daily COVID-19 cases (from the New York Times Coronavirus (Covid-19) Dataset) and the number of policies enacted on each day in the selected location. A bar graph below the timeline shows the breakdown of how many policies in each policy category were enacted, active, or expired on a given date. By default, these figures reflect the most recent date available, but users can select a specific date by dragging or using arrow keys to move the blue date slider. Selecting a new date adjusts the bar chart to reflect the policy environment up to that point and displays a pop-up with how many policies from each category were enacted on that day. Clicking on a policy category in the pop-up brings up a modal with information on each policy that was enacted. Below the bar chart, users can also explore and view any policy enacted by that location using a search and filter tool.

_COVID caseload data_

_US map and social distancing policy model_

US state-level COVID-19 caseload data, new cases in the last 7 days and cumulative cases, are sourced from the New York Times Coronavirus (Covid-19) Data in the United States (https://github.com/nytimes/covid-19-data). These data include confirmed cases and, where captured by public health agencies, probable cases. Data are updated daily. These data are collated by the New York Times on the basis of data from state and local health agencies and licensed under the Creative Commons Attribution-Non Commercial 4.0 International license.

_Global map_

Global COVID-19 caseload data, new cases in the last 7 days and cumulative cases, are sourced from the COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University which holds the copyright to all data (https://github.com/CSSEGISandData/COVID-19). These data include only confirmed cases and are updated daily. Additional information about the collation of the data by the Johns Hopkins University is available from the GitHub repository linked above.

_Social distancing policy model_

The COVID AMP policy model supports users in evaluating the impact of policies on the outbreak – a visualization of when (1) policies were implemented in each state relative to their actual caseload and fatalities, (2) predictive analysis for how future policy implementation will impact caseload, and (3) an analysis of what would have been had no mitigation policies been implemented. The social distancing policy model includes actual and modeled data for COVID-19 cases, COVID-related hospitalizations, ICU patient count (specifically for COVID complications), and deaths at daily resolution. These data about the dynamics of COVID outbreaks are accompanied by key designations of policies related to social distancing (i.e., stay-at-home, safer-at-home, partially open) captured from policies in place at different points in the outbreak (see “Visualizing distancing level,” above). For points in the future, users can add new social distancing policies and evaluate their relative impact on the modeled outcome. The AMP social distancing policy model is currently available for US states at state scale.

For past dates, cases are sourced from confirmed and probable cases (see ‘COVID caseload data’ above) data from March 1 to the most recent data update. Because case data is cumulative, we calculate “active” cases by assuming patients recover 13 days after their case is confirmed by testing and deriving deaths from those cases. We assume approximately 25% of total confirmed cases are hospitalized with equates to ~7% of total cases (symptomatic and asymptomatic.) For all dates past the most recent case update, all data for cases, hospitalizations, ICU patient counts, and deaths are modeled using the approach below as seeded with the current case counts from reported actual cases (from the New York Times Coronavirus (Covid-19) Data in the United States, as described above).

Future cases, hospitalizations, ICU patient counts, and deaths are predicted on the basis of a modified SEIR (susceptible, exposed, infectious, recovered) model adding multiple levels of infections and an asymptomatic class (see Figure 1 below). The COVID-19 SEIR model used here was developed in collaboration with COVID Act Now, originally adapted from the original work of Dr. Allison Hilli, Research Fellow at the Harvard Program on Evolutionary Dynamics. In this model, susceptible (S) individuals may become exposed (E) to the virus, then infected (I) at varying levels of disease severity (asymptomatic, mild, moderate, or severe, captured as rates A, I1, I2, and I3 respectively. Infected individuals then either recover (R) or die (D). Figure 1, below, is adapted from Hill et al., and describes the process underling the COVID-19 SEIR model that calculated cases, hospitalizations, ICU patient count, and deaths in the social distancing policy model.



_State descriptions_

The following bullets summarize the states of the SEIR model and how individuals progress through them (see tables below for details on each parameter):

- Susceptible: Starting state for all individuals in a fully predictive run and, in cases where the model run is initiated base on prior cases, the susceptible group includes the proportion of individuals not previously sick.
- Exposed: People move from Susceptible to Exposed when they come in contact with other infectious individuals with a rate that is determined by the number of contacts individuals have with one another (providing basis for susceptible individuals to come into contact with infected individuals and get exposed). In this model, Exposed individuals are not yet infectious to Susceptible individuals and do not have symptoms (are pre-symptomatic). All exposed individuals transition to mild cases (Infected1) after 6 days.
- Asymptomatic: These cases have no symptoms and will not know they are infected unless tested. They can, however, infect other people. We assume 30% of infected people in the model are asymptomatic and infected for a total of 12 days with the final 6 of those being infectious to others.
- Infected1: These are mild cases. After approximately a week, 7% of these cases worsen, and require hospitalization (the Infected2 state), and the remaining 93% progress to the Recovered state.
- Infected2: These are severe, hospitalized cases, requiring non-ICU treatment. After approximately a week, 13% of these cases worsen, thus requiring ICU/ventilation (Infected3), while the remaining 87% progress to the Recovered state.
- Infected3: These are critical cases requiring ICU treatment. This model assumes all deaths must first pass through this category. After approximately a week, 40% of these cases lead to death, while the remaining 60% progress to Recovered.
- Recovered: Includes all individuals who have already had the disease (excluding those who died). For the purposes of the model, recovered individuals are considered to be immune from future infection.
- Dead: Those that have died from the disease. All of these come from ICU (Infected3) cases and make up approximately 1% of all cases.


_Modeling disease characteristics_

Values for the epidemiological model parameters are based on the best available data and academic consensus, wherever possible. Changes in parameters related to policy implementation are based on the expected changes in contact rate and transmission anticipated corresponding to policy status under each category of social distancing (lockdown, stay-at-home, safer-at-home, partially open and open; see above for definitions). These estimates are calculated as a difference in contact rate and transmission based on reproductive rate (R), the number of new cases that result from one individual infecting others. Reproductive rate is an inferred model outcome and is not an input of the SEIR model but is used to calibrate the model state to produce a transmission rate (β) for the given conditions in the table below. The probability of transmission (β), representing the likelihood that a susceptible individual is exposed to someone who is infectious (and the likelihood of infection given exposure, which is not adjusted directly in the model), is set dynamically based on the policies in place at a given time. Thus, the distancing level captured from policies is considered in the transmission dynamics for future COVID spread (e.g., stay-at-home more stringently restricts contacts between individuals and suppresses transmission more than a safer-at-home condition).

_What if we had done nothing? (Counterfactual)_

As the outbreak has unfolded, we have added a counterfactual analysis to assess how the event would have unfolded had states not implemented any policies. The counterfactual scenario is modeled assuming contact rate remained elevated throughout the Spring and early Summer of 2020, as those states had not implemented social distancing policies. We initialize the model on the first day each state hit 100 cumulative cases. We then project forward assuming an R value of 2.1, slightly lower than that before the event to account for changes in behavior as would be expected with only reports of disease threat (as seen in states without social distancing policies, but that still showed a reduction in mobility.) In those states who experienced large, early outbreaks, defined by more than 1,000 cumulative cases before May 15th, (New Jersey and New York) we initialize the counterfactual at the end of these outbreaks to better predict the effect of policies for the next wave. In addition to plotting the counterfactual against the actuals (“What if we had done nothing?”), we present the difference in current actual caseload against the modelled caseload and the modelled number of deaths at the upper right of the chart. Note that the caseload compares today against the “What if” scenario today; for deaths, this value is adjusted to account for modelled fatalities expected to result from the modelled number of cases. (We report the modelled deaths as those 30 days in the future to capture the average 30 day lag from start of infection to death.)


_Policies (distancing level)_

The AMP Policy Model includes policies implemented historically, as captured by the ‘Distancing level’, and allows users to add policies in the future. Future policy interventions update model parameters (specifically the transmission level, or Beta) to reflect the increase or decrease in intra-personal contact level as a result of policies that change the level of social distancing. This feature provides the ability to analyze the relative, future impact of policy implementation on caseload.

i
Hill, Alison, et al. "Modeling COVID-19 Spread vs Healthcare Capacity" https://alhill.shinyapps.io/COVID19seir/


ii
Calculated based on a consideration of literature-reported R values, estimated reduction of transmission by non-pharmaceutical interventions, and bounded by estimated effective R values developed by the Rt COVID-19 project (https://rt.live/).


iii
Wei, Yongyue, et al. “A systematic review and meta-analysis reveals long and dispersive incubation period of COVID-19” https://www.medrxiv.org/content/10.1101/2020.06.20.20134387v1


iv
Koehler, Matt, et al. “Modeling COVID-19 for lifting non-pharmaceutical interventions” https://www.medrxiv.org/content/10.1101/2020.07.02.20145052v1


v
Ferguson, Neil, et al. "Report 9: Impact of non-pharmaceutical interventions (NPIs) to reduce COVID19 mortality and healthcare demand" https://www.imperial.ac.uk/media/imperial-college/medicine/sph/ide/gida-fellowships/Imperial-College-COVID19-NPI-modelling-16-03-2020.pdf. Note: As implemented in the model, the reported values in this reference are weighted by US population demographics.


vi
US Centers for Disease Control and Prevention. “Interim Clinical Guidance for Management of Patients with Confirmed Coronavirus Disease (COVID-19)” https://www.cdc.gov/coronavirus/2019-ncov/hcp/clinical-guidance-management-patients.html


vii
Cummings, Matthew, et al. "Epidemiology, clinical course, and outcomes of critically ill adults with COVID-19 in New York City: a prospective cohort study" https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)31189-2/fulltext


viii
Ferguson, Neil, et al. "Report 9: Impact of non-pharmaceutical interventions (NPIs) to reduce COVID19 mortality and healthcare demand" https://www.imperial.ac.uk/media/imperial-college/medicine/sph/ide/gida-fellowships/Imperial-College-COVID19-NPI-modelling-16-03-2020.pdf. Note: As implemented in the model, the reported values in this reference are weighted by US population demographics.


ix
European Centre for Disease Prevention and Control. “Clinical characteristics of COVID-19” https://www.ecdc.europa.eu/en/covid-19/latest-evidence/clinical
