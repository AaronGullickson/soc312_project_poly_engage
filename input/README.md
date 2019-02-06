# National Longitudinal Survey of Youth 1997

The data we are using comes from the [National Longitudinal Survey of Youth 1997](https://www.nlsinfo.org/content/cohorts/nlsy97) (NLSY97), conducted by the US Bureau of Labor Statistics. The first wave of the NLSY97 surveyed respondents who were aged 12-17 in 1997. These same individuals are re-interviewed each year, making this a *longitudinal* study. Most of the data that we will be using is from the first wave in 1997, but the political engagement variables are from 2004 when the respondent was a young adult. 

I created an extract of the full NLSY97 data using the [NLS Investigator](https://www.nlsinfo.org/investigator/pages/login.jsp). The questions on family interaction were only asked of a subsample of the full NLSY97 so we restrict our analysis to this subsample. Here is a full description of all variables in the dataset that we will use.

- **gender**: gender of the respondent recorded only as male or female. 
- **race**: race of the respondent: white, black, Latino, Asian/Pacific Islander, American Indian, other. Information here is based off of responses during the screening interview with a household informant and is not self-reported. 
- **family_type**: What type of family does the respondent currently reside in? I have combined two biological and two adoptive parents into a single family type. The other types are a two parent household with one step-parent (bio + step), a single biological parent, and all other cases.
- **hh_income**: The household income for the respondent's household, measured in 1000's of US dollars.
- **hh_networth**: The net worth of the respondent's household, measured in 1000's of US dollars. Note that this value can be negative.
- **high_parent_ed**: the highest years of schooling reported by the respondent's resident parents and/or biological parents.
- **urbanicity**: Did the respondent grow up in an urban or rural location. 
- **poly_interest**: Respondents were asked in 2004 "Some people seem to follow what's going on in government and public affairs most of the time, whether there's an election going on or not. Others aren't that interested. Would you say you follow what's going on in government and public affairs most of the time, some of the time, only now and then, or hardly at all?". Respondents who said "Hardly at all" are coded as a 1. Respondents who said "Only now and then" are coded as a 2. Respondents who said "Some of the time" are coded as a 3. Respondents who said "Most of the time" are coded as a 4. 
- **voted**: Did the respondent vote in the 2004 election? 
- **family_dinner**: Respondents were asked how many days of the week (0-7) they typically sat down and ate dinner with their family.
- **family_fun**: Respondents were asked how many days of the week (0-7) they typically do something fun as a family. 

In the original data, there are missing values for some observations on some of these variables. To simplify our analysis, I have used some advanced techniques that are beyond the scope of our class to impute these missing values.
