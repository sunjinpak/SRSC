---
layout: default
title: Project 6 - Method and Results
---

[Back to Project 6](https://sunjinpak.com/student-research-guides/project-6-leader-workaholism-food-safety)

# Method and Results - Project 6

**Title**: The Cost of the Grind: Assessing the Impact of Leader Workaholism on Food Safety Compliance and Employee Retention

**Team**: Eric

**Style**: APA 7th Edition

---

## Method

### Participants

Participants were 203 employees recruited from the agriculture and food processing industry in Kern County, California. Eligibility criteria required that participants be at least 18 years old and currently employed in the agriculture or food processing sector. The sample was 58.6% male and 36.9% female, with an average age of 42.45 years (*SD* = 12.75). Regarding job type, 34.5% were field workers, 31.5% worked in packing houses, 22.2% in processing facilities, and 11.8% in office or administrative roles. The majority worked in agriculture (54.7%), followed by food processing (30.5%), and both sectors (14.8%). Most participants worked day shifts (61.1%), followed by night shifts (22.2%) and rotating shifts (14.8%). In terms of education, 33.0% held a high school diploma or GED, 27.1% had less than a high school education, 19.7% had some college, 11.3% held an associate degree, and 8.9% held a bachelor's degree or higher. Average organizational tenure was 11.51 years (*SD* = 9.80).

### Procedure

Data were collected via an online survey. Participants were recruited through LinkedIn and snowball sampling. After providing informed consent, participants completed measures assessing their perceptions of their supervisor's workaholism, food safety compliance behaviors, turnover intentions, after-hours work contact, emotional exhaustion, and job satisfaction. All procedures were approved by the university's Institutional Review Board (Protocol #27-12).

### Measures

Unless otherwise noted, all items were rated on a 5-point Likert-type scale ranging from 1 (*strongly disagree*) to 5 (*strongly agree*).

**Leader workaholism.** Leader workaholism was measured using a 10-item adapted version of the Dutch Work Addiction Scale (DUWAS; Schaufeli et al., 2009). Participants rated their direct supervisor's work behaviors. The scale includes two subscales: Working Excessively (5 items) and Working Compulsively (5 items). A sample item is "My supervisor stays busy and keeps many irons in the fire" (α = .90).

**Food safety compliance.** Food safety compliance was measured using six items adapted from the Safety Compliance Scale (Neal & Griffin, 2006), modified for the food safety context. Items were rated on a 5-point scale ranging from 1 (*never*) to 5 (*always*). A sample item is "I follow all food safety procedures regardless of the situation" (α = .80).

**Turnover intention.** Turnover intention was measured using three items from Colarelli (1984). A sample item is "I frequently think of quitting this job" (α = .71).

**After-hours work contact.** After-hours work contact was assessed using five items adapted from Derks et al. (2015). Items were rated on a 5-point scale ranging from 1 (*never*) to 5 (*very often*). A sample item is "My supervisor contacts me about work-related matters outside of regular working hours" (α = .87).

**Emotional exhaustion.** Emotional exhaustion was measured using five items from the emotional exhaustion subscale of the Maslach Burnout Inventory (Maslach & Jackson, 1981). Items were rated on a 5-point scale ranging from 1 (*never*) to 5 (*always*). A sample item is "I feel emotionally drained from my work" (α = .86).

**Job satisfaction.** Job satisfaction was measured using three items from the Michigan Organizational Assessment Questionnaire (Cammann et al., 1983). A sample item is "All in all, I am satisfied with my job" (α = .73).

**Control variables.** We controlled for age and organizational tenure in all analyses, as both may influence employees' perceptions of their supervisor and their own work attitudes and behaviors (Ng & Feldman, 2010).

### Analytic Strategy

Analyses were conducted using Python 3.13 (via Claude Code, an AI-assisted coding environment) with the pandas, NumPy, SciPy, and statsmodels libraries. First, we computed descriptive statistics and bivariate correlations among all study variables. Second, we assessed the reliability of multi-item scales using Cronbach's alpha. Third, we tested direct effect hypotheses (H1-H3) using hierarchical ordinary least squares regression, entering control variables (age, organizational tenure) in Step 1 and the focal predictor in Step 2. Fourth, we tested mediation hypotheses (H4-H5) using a bootstrapping approach with 5,000 resamples, consistent with recommendations by Hayes (2022) for the PROCESS Model 4 framework. Mediation was considered significant when the 95% bias-corrected bootstrap confidence interval for the indirect effect did not include zero.

---

## Results

### Preliminary Analyses

Means, standard deviations, reliabilities, and intercorrelations among study variables are presented in Table 1. All multi-item scales demonstrated acceptable internal consistency reliability (α > .70; Nunnally, 1978). Consistent with our theoretical expectations, leader workaholism was negatively correlated with food safety compliance (*r* = -.54, *p* < .01) and job satisfaction (*r* = -.66, *p* < .01), and positively correlated with turnover intention (*r* = .65, *p* < .01), after-hours work contact (*r* = .75, *p* < .01), and emotional exhaustion (*r* = .72, *p* < .01). After-hours work contact was strongly positively correlated with emotional exhaustion (*r* = .76, *p* < .01).

### Hypothesis Tests

Results of the hierarchical regression analyses testing Hypotheses 1-3 are presented in Table 2. Hypothesis 1 predicted that leader workaholism would be negatively related to employee food safety compliance. After controlling for age and organizational tenure, leader workaholism was significantly negatively related to food safety compliance (*B* = -0.42, *SE* = 0.05, *t* = -8.71, *p* < .001, 95% CI [-0.52, -0.33]). The addition of leader workaholism to the model explained an additional 26.7% of variance in food safety compliance (Δ*R*² = .267, *F* change = 75.90, *p* < .001). Hypothesis 1 was supported.

Hypothesis 2 predicted that leader workaholism would be positively related to employee turnover intention. Controlling for covariates, leader workaholism was significantly positively related to turnover intention (*B* = 0.75, *SE* = 0.06, *t* = 11.83, *p* < .001, 95% CI [0.63, 0.88]). The addition of leader workaholism explained an additional 39.3% of variance in turnover intention (Δ*R*² = .393, *F* change = 139.96, *p* < .001). Hypothesis 2 was supported.

Hypothesis 3 predicted that after-hours work contact would be positively related to emotional exhaustion. After controlling for covariates, after-hours work contact was significantly positively related to emotional exhaustion (*B* = 0.76, *SE* = 0.05, *t* = 16.04, *p* < .001, 95% CI [0.66, 0.85]). The addition of after-hours work contact explained an additional 53.1% of variance in emotional exhaustion (Δ*R*² = .531, *F* change = 257.32, *p* < .001). Hypothesis 3 was supported.

### Mediation Analyses

Hypothesis 4 predicted that emotional exhaustion would mediate the relationship between leader workaholism and turnover intention. As shown in Table 3, leader workaholism was significantly positively related to emotional exhaustion (path *a*: *B* = 0.85, *SE* = 0.06, *p* < .001), and emotional exhaustion was significantly positively related to turnover intention controlling for leader workaholism (path *b*: *B* = 0.41, *SE* = 0.07, *p* < .001). The total effect of leader workaholism on turnover intention was significant (*c*: *B* = 0.75, *SE* = 0.06, *p* < .001), and the direct effect remained significant after including the mediator (*c'*: *B* = 0.41, *SE* = 0.08, *p* < .001). The indirect effect through emotional exhaustion was significant (*ab* = 0.35, 95% Boot CI [0.23, 0.47]). Because the direct effect remained significant, the results indicate partial mediation. Hypothesis 4 was supported.

Hypothesis 5 predicted that job satisfaction would mediate the relationship between leader workaholism and turnover intention. As shown in Table 3, leader workaholism was significantly negatively related to job satisfaction (path *a*: *B* = -0.75, *SE* = 0.06, *p* < .001), and job satisfaction was significantly negatively related to turnover intention controlling for leader workaholism (path *b*: *B* = -0.38, *SE* = 0.07, *p* < .001). The direct effect of leader workaholism on turnover intention remained significant after including the mediator (*c'*: *B* = 0.47, *SE* = 0.08, *p* < .001). The indirect effect through job satisfaction was significant (*ab* = 0.29, 95% Boot CI [0.19, 0.40]). Because the direct effect remained significant, the results indicate partial mediation. Hypothesis 5 was supported.

---

## Tables

### Table 1

*Means, Standard Deviations, and Correlations Among Study Variables*

| Variable | *M* | *SD* | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|---|---|---|
| 1. Leader workaholism | 3.46 | .79 | (.90) | | | | | | | |
| 2. Food safety compliance | 3.95 | .64 | -.54** | (.80) | | | | | | |
| 3. Turnover intention | 2.68 | .93 | .65** | -.58** | (.71) | | | | | |
| 4. After-hours work contact | 3.11 | .94 | .75** | -.65** | .69** | (.87) | | | | |
| 5. Emotional exhaustion | 3.18 | .95 | .72** | -.62** | .68** | .76** | (.86) | | | |
| 6. Job satisfaction | 3.28 | .90 | -.66** | .52** | -.65** | -.71** | -.63** | (.73) | | |
| 7. Age | 42.45 | 12.75 | -.05 | -.04 | .01 | .06 | -.02 | -.06 | -- | |
| 8. Organizational tenure | 11.51 | 9.80 | -.16* | .12 | -.17* | -.14* | -.21** | .10 | .59** | -- |

*Note.* *N* = 203. Cronbach's alpha reliability coefficients appear in parentheses along the diagonal.

\**p* < .05. \*\**p* < .01.

---

### Table 2

*Hierarchical Regression Results for Direct Effects (H1-H3)*

| | Food safety compliance | | Turnover intention | | Emotional exhaustion | |
|---|---|---|---|---|---|---|
| Predictor | *B* (*SE*) | 95% CI | *B* (*SE*) | 95% CI | *B* (*SE*) | 95% CI |
| **Step 1** | | | | | | |
| Age | -0.01 (0.00)* | | 0.01 (0.01)* | | 0.01 (0.01) | |
| Org tenure | 0.01 (0.01)* | | -0.03 (0.01)** | | -0.03 (0.01)*** | |
| *R*² | .034 | | .049 | | .059 | |
| **Step 2** | | | | | | |
| Leader workaholism | -0.42 (0.05)*** | [-0.52, -0.33] | 0.75 (0.06)*** | [0.63, 0.88] | - | - |
| After-hours contact | - | - | - | - | 0.76 (0.05)*** | [0.66, 0.85] |
| Δ*R*² | .267*** | | .393*** | | .531*** | |
| Total *R*² | .301 | | .442 | | .590 | |

*Note.* *N* = 203. Unstandardized regression coefficients are reported.

\**p* < .05. \*\**p* < .01. \*\*\**p* < .001.

---

### Table 3

*Mediation Analysis Results (H4-H5)*

| Path | H4: LW → EE → TI | | H5: LW → JS → TI | |
|---|---|---|---|---|
| | *B* (*SE*) | 95% CI | *B* (*SE*) | 95% CI |
| *a* path (LW → Mediator) | 0.85 (0.06)*** | [0.73, 0.96] | -0.75 (0.06)*** | [-0.87, -0.63] |
| *b* path (Mediator → TI) | 0.41 (0.07)*** | [0.27, 0.55] | -0.38 (0.07)*** | [-0.52, -0.25] |
| Total effect (*c*) | 0.75 (0.06)*** | [0.63, 0.88] | 0.75 (0.06)*** | [0.63, 0.88] |
| Direct effect (*c'*) | 0.41 (0.08)*** | [0.24, 0.57] | 0.47 (0.08)*** | [0.31, 0.62] |
| Indirect effect (*ab*) | 0.35 | [0.23, 0.47] | 0.29 | [0.19, 0.40] |
| Mediator model *R*² | .535 | | .450 | |
| Outcome model *R*² | .523 | | .517 | |

*Note.* *N* = 203. Unstandardized coefficients reported. Indirect effect confidence intervals are bias-corrected bootstrap CIs based on 5,000 resamples. Controls: age, organizational tenure. LW = leader workaholism; EE = emotional exhaustion; JS = job satisfaction; TI = turnover intention.

\*\*\**p* < .001.

---

## Summary of Hypothesis Testing

| Hypothesis | Prediction | Result |
|---|---|---|
| H1 | Leader workaholism is negatively related to food safety compliance | **Supported** (*B* = -0.42, *p* < .001) |
| H2 | Leader workaholism is positively related to turnover intention | **Supported** (*B* = 0.75, *p* < .001) |
| H3 | After-hours work contact is positively related to emotional exhaustion | **Supported** (*B* = 0.76, *p* < .001) |
| H4 | Emotional exhaustion mediates LW → TI relationship | **Supported** (partial; *ab* = 0.35, CI [0.23, 0.47]) |
| H5 | Job satisfaction mediates LW → TI relationship | **Supported** (partial; *ab* = 0.29, CI [0.19, 0.40]) |

---

## References (for this section)

- Cammann, C., Fichman, M., Jenkins, G. D., & Klesh, J. R. (1983). Assessing the attitudes and perceptions of organizational members. In S. E. Seashore, E. E. Lawler III, P. H. Mirvis, & C. Cammann (Eds.), *Assessing organizational change: A guide to methods, measures, and practices* (pp. 71-138). Wiley.
- Colarelli, S. M. (1984). Methods of communication and mediating processes in realistic job previews. *Journal of Applied Psychology, 69*, 633-642.
- Derks, D., van Duin, D., Tims, M., & Bakker, A. B. (2015). Smartphone use and work-home interference: The moderating role of social norms and employee work engagement. *Journal of Occupational and Organizational Psychology, 88*, 155-177.
- Hayes, A. F. (2022). *Introduction to mediation, moderation, and conditional process analysis: A regression-based approach* (3rd ed.). Guilford Press.
- Maslach, C., & Jackson, S. E. (1981). The measurement of experienced burnout. *Journal of Organizational Behavior, 2*, 99-113.
- Neal, A., & Griffin, M. A. (2006). A study of the lagged relationships among safety climate, safety motivation, safety behavior, and accidents at the individual and group levels. *Journal of Applied Psychology, 91*, 946-953.
- Ng, T. W. H., & Feldman, D. C. (2010). The relationships of age with job attitudes: A meta-analysis. *Personnel Psychology, 63*, 677-718.
- Nunnally, J. C. (1978). *Psychometric theory* (2nd ed.). McGraw-Hill.
- Schaufeli, W. B., Shimazu, A., & Taris, T. W. (2009). Being driven to work excessively hard: The evaluation of a two-factor measure of workaholism in the Netherlands and Japan. *Cross-Cultural Research, 43*, 320-348.

---

[Back to Project 6](https://sunjinpak.com/student-research-guides/project-6-leader-workaholism-food-safety)
