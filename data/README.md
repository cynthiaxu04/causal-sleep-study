# Data description

**timezone** = datetime object; participant's primary timezone

**sleep_quality** = int; pre-treatment, Likert scale of participant's answer to "How would you rate your quality of sleep?"
	
 - 1 - Very Poor
 - 2 - Poor
 - 3 - Average
 - 4 - Good
 - 5 - Very Good

**trouble_sleep** = int; pre-treatment, Likert scale of participant's agreement with the statement "I have trouble falling asleep."
	
 - 1 - Strongly Disagree
 - 2 - Somewhat Disagree or Disgaree
 - 3 - Neutral
 - 4 - Somewhat Agree or Agree
 - 5 - Strongly Agree

**gender** = int; pre-treatment, participant's identified gender
	
 - 0 - Male
 - 1 - Female
 - 2 - Other or Prefer not to say

**age_group** = int; pre-treatment, participant's age range
	
 - 1 - 18-24
 - 2 - 25-34
 - 3 - 35-44
 - 4 - 45-54
 - 5 - 55-64
 - 6 - 65+

**total_sleep** = float; pre-treatment, participant's typical total sleep time in hours calculated from participant's reported typical bed time and typical wake up time

**watch** = str; pre-treatment, participant's smart watch type

**watch_model** = str; pre-treatment, specific model of participant's smart watch

**email** = str; pre-treatment, participant's email address

**phase_sq** = int; post-treatment, Likert scale of participant's response to the question "How would you rate your quality of sleep during this phase?
	
 - 1 - Very Poor
 - 2 - Poor
 - 3 - Average
 - 4 - Good
 - 5 - Very Good

**phase_ts** = int; post-treatment, Likert scale of participant's agreement with the statement "I have trouble falling asleep."

- 1 - Strongly Disagree
- 2 - Somewhat Disagree or Disgaree
- 3 - Neutral
- 4 - Somewhat Agree or Disagree
- 5 - Strongly Agree

**treat** = int; participant's treatment or control phase
	
 - 0 - control
 - 1 - treatment

**day1_ss** = int; participant's day 1 sleep score

**day2_ss** = int; participant's day 2 sleep score

**day3_ss** = int; participant's day 3 sleep score

**day4_ss** = int; participant's day 4 sleep score

**Timestamp** = datetime object; time when participant submitted data
