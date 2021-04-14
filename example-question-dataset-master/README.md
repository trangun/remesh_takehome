# Example Question Dataset

The dataset consists of open-ended text responses to a question as well as two different types of "voting" data points. "Voting" is when respondents are presented with other respondents' thoughts and given the opportunity to express their preference for or against them.

This dataset was collected in response to the question:

> What features do you like about the social media platforms that you use?

The three types of data points in the dataset are:

---

`thoughts.csv` - These are the open-ended text responses to the prompt.

| id | respondent_id | text |
| -- | ------------- | ---- |
| 0  | 17            | It's easy to use and very heavily adopted by other people. |
| 1  | 38            | Easy access is just about the only thing. |
...

---

`agreements.csv` - A respondent is presented a response and they report "I agree" or "I disagree" with this response.

| respondent_id | thought_id | label |
| ------------- | ---------- | ----- |
| 32            | 7          | Disagree |
| 37            | 3          | Agree |
...

---

`binary_choice.csv` - A respondent is presented two responses and they select which one they prefer over the other (A or B), or skip (Neither).

| respondent_id | thought_a_id | thought_b_id | label |
| ------------- | ------------ | ------------ | ----- |
| 32            | 20           | 14           | A     |
| 6             | 35           | 29           | B     |
| 16            | 2            | 36           | Neither |
...