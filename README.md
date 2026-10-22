INTRODUCTION

We always talk about studying hard, but how do variables like screen time, internet quality, sleep hygiene, and caffeine intake actually intertwine with exam scores and burnout? To find out, I put together a comprehensive analysis and interactive dashboard titled Scholars Academic Success & Lifestyle Analytics. This dashboard was built from a student productivity dataset to see which daily habits really change a student’s results and burnout. The data covers 5,000 students across 21 columns, aged 16 to 25, with three genders (Female, Male and Others) and three academic levels (High School, Undergraduate and Postgraduate). The average productivity score is 37.27, and the average sleep is 7.0 hours. At the top end, Student ID #21 has the highest exam score of 64.09 after studying 9.31 hours a day. Student ID #3376 has the highest productivity score of 98.02, with 11.84 study hours a day, even with poor internet.

Data Source: Kaggle(https://www.kaggle.com/datasets/sampathvinayakbablu/ultimate-student-productivity-dataset)

Tool: Microsoft Excel (Tables, PivotTables, PivotChart, slicers, KPI cards, dashboard)

DATA STORY

This dataset tells the story of the modern digital student, following 5,000 students as they juggle online classes, part-time jobs, deadlines and the constant pull of social media. At the top are students like ID #21, who has the highest exam score of 64.09, and ID #3376, a 17-year-old High School student who has the highest productivity score of 98.02 and the second-highest exam score of 62.82. She did it with poor internet, no job, no deadline and about 6.7 hours of sleep, but with 11.84 hours of study, very high focus and low burnout. At the other end are students like ID #20 and ID #42, who studied only about half an hour a day and finished with an exam score of 1, the lowest in the data. For me, it shows that daily habits and not only textbook time, shape how well students do and how drained they feel.

DATA CLEANING PROCESS

Checked for blank cells and found none.
Checked for duplicate rows and found none.
Checked ranges (age 16 to 25, sleep 4 to 10 hours, all scores above 0) and found nothing impossible.
Replaced “Prefer not to say” in the gender column with “Others”, so gender has three clean groups: Female, Male and Others.
Removed a stray space in front of “Others”.
Made sure every column heading was properly spelt out and clear.
Expanded the columns to fit, so all the data can be read.
Grouped the number fields (study hours, sleep hours, screen time, social media hours and caffeine intake) into bins, so trends are easy to read.
Sorted the grouped bins in the right order, because Excel sorts them alphabetically by default.

Columns Within the Data

Profile: Student ID, Age, Gender, Academic Level.

Study: Study Hours, Self Study Hours, Online Classes Hours.

Lifestyle: Sleep Hours, Screen Time Hours, Social Media Hours, Gaming Hours, Exercise Minutes, Caffeine Intake (mg).

Situation: Part-time Job, Upcoming Deadline, Internet Quality.

Outcomes: Exam Score, Burnout Level, Productivity Score, Focus Index, Mental Health Score.

PRE-ANALYSIS

Splitting the data

Dependent variables (what I measure): Exam Score, Burnout Level, Productivity Score, Focus Index, Mental Health Score.
Independent variables (what might cause change): Age, Gender, Academic Level, Study Hours, Self Study Hours, Online Class Hours, Part-time Job, Sleep Hours, Exercise Minutes, Caffeine Intake, Social Media Hours, Gaming Hours, Screen Time Hours, Internet Quality and Upcoming Deadline.
Industry Type: This dataset belongs to the EdTech and Student Wellness industry, specifically Learning Analytics. Schools, universities and app developers use this kind of data to build early warning systems that spot students at risk before an exam.

Stakeholders: They include: school and university leaders, teachers and lecturers, student counsellors, parents, EdTech and wellness app teams, and the students themselves.

What success means to the industry: Success in this industry means keeping students in school and in good health, not only helping them pass exams. It means keeping students from dropping out because of burnout, and helping them reach a high productivity score in fewer study hours, so they work smarter and not harder. It also means making sure students with poor internet don’t fall behind, and spotting a drop in mental health early enough to give support before it affects their results.

IN-ANALYSIS

This was done after the cleaned data was turned into PivotTables and charts, one for each of my pre-analysis questions. At this stage, I looked at each chart on its own to see what it shows and what it means, before putting them together on the dashboard. I also kept the number of students in each group in mind, so I wouldn’t read too much into small groups.

1. Study vs Grade Trend
<img width="781" height="249" alt="image" src="https://github.com/user-attachments/assets/ffcac49d-c77d-499d-bb42-c537c24e3ed8" />

Press enter or click to view image in full size

Observation: exam score climbs at every step: 8.5 (0–2 hours), 13.9, 19.9, 26.7, 34.1, then 45.2 at more than 10 hours.
Insight: about 6 extra exam points for every 2 extra study hours (r = 0.51). The last group has only 8 students, so I read it with care. ID #3376 (11.84 hours, exam score 62.82) sits in that top group.

2. Average Productivity by Academic Level
   <img width="664" height="278" alt="image" src="https://github.com/user-attachments/assets/3a341397-575a-4412-b4ee-e94e07f8f0e2" />



Observation: Undergraduate 37.33, High School 37.25, Postgraduate 37.23.
Insight: a gap of 0.1 is nothing. Level does not decide productivity. Habits do. The student with the highest productivity in the data (#3376) is in High School.

3. Sleep Hour vs. Mental Health
   <img width="775" height="354" alt="image" src="https://github.com/user-attachments/assets/fb3e19a1-7892-4693-b57d-70db1ef2f44e" />


Press enter or click to view image in full size

Observation: the line stays between 5.15 and 5.66 with no direction. The lowest point is at 4–5 hours (202 students), but there is no steady climb.
Insight: sleep does not move the mental health score in this data (r = 0.00). This was my biggest surprise. Sleep matters for burnout instead (see post analysis).

4. Digital Usage and Mood Impact
   <img width="811" height="314" alt="image" src="https://github.com/user-attachments/assets/6c846b38-0866-4fbc-8f69-8544cd25f226" />


Press enter or click to view image in full size

Observation: mental health stays between 5.35 and 5.74 from 0–2 hours of screen time up to more than 12 hours.
Insight: screen time does not move the mood score (r = 0.02). The 0–2 and more-than-12 groups are small (124 and 106 students), so I did not read much into them.

5. Internet Quality vs Exam Score
   <img width="775" height="209" alt="image" src="https://github.com/user-attachments/assets/34397d51-1e58-4aad-a19a-9c0c7c285aa5" />


Press enter or click to view image in full size

Observation: Poor 19.01, Average 18.92, Good 18.50.
Insight: poor internet scored slightly higher, but the gaps are tiny. Internet quality does not change exam scores here. ID #3376 is a live example: poor internet, second-highest exam score.

6. Social Media Productivity Drain
   <img width="772" height="267" alt="image" src="https://github.com/user-attachments/assets/c20dfa02-70d0-47ed-a016-1ef7ac70cf1d" />


Press enter or click to view image in full size

Observation: productivity falls from 38.98 (0–2 hours) to 37.14 (2–4) to 35.79 (4–6).
Insight: more social media goes with lower productivity, a small but real drain (r = -0.07). It hurts focus most, which drops from 33.7 to 25.8 over the same groups. The 8-to-10- hour bar (39.10) has only 3 students, so I ignored it. ID #3376 uses just 0.48 hours of social media a day.

7. Burnout Level by Gender
<img width="750" height="283" alt="image" src="https://github.com/user-attachments/assets/17b6b30d-1729-461d-a078-1343a4311685" />

Press enter or click to view image in full size

Observation: Female 45.3, Male 45.8, Others 45.7.
Insight: the gaps are within chance. Burnout is not a gender problem.

8. Caffeine and Focus Efficiency
   <img width="750" height="450" alt="image" src="https://github.com/user-attachments/assets/937820fc-bf85-4d09-a129-8ef1ebdc2142" />


Press enter or click to view image in full size

Observation: all the bars are almost the same height. Focus stays at about 29 to 30 whether a student takes under 50 mg or almost 500 mg of caffeine.
Insight: caffeine does not make students more focused. Taking more coffee does not give a better focus score. The small ups and downs between bars are just chance. Caffeine does link to burnout, which rises from 41.5 (0–49 mg) to 49.9 (450–500 mg).

9. Learning Duration Report
    <img width="772" height="230" alt="image" src="https://github.com/user-attachments/assets/421505d2-72eb-4d24-b2a9-84ecd507de4d" />


Press enter or click to view image in full size

Observation: total study hours are Postgraduate 7,613, High School 7,585, Undergraduate 7,500. On average, students study 4.51 to 4.57 hours a day in every level.
Insight: all three levels have about the same number of students, so the totals are close. Everyone studies about 4.5 hours a day. Study time does not depend on level.

POST ANALYSIS

Become a Medium member
I looked at each chart using the slicer, checking one group at a time. The patterns stayed the same across all groups. Below are the observations and insights I noted down from this review.

1. Study time and focus together decide exam scores

Observation: exam score rises about 6 points for every 2 extra hours of study. Focus has an even stronger link with exam score than study hours do (focus r = 0.75, study hours r = 0.51), and mental health also rises with exam score (r = 0.55).
Insight: hours alone are not enough. A student who studies under 3 hours but is highly focused averages an exam score of 21.0, while a student who studies 7+ hours with low focus averages only 16.2. For teachers and schools, this means helping students to study better (fewer distractions, good rest, a calm place) is worth as much as telling them to study longer.
2. Sleep is the strongest protection against burnout

Observation: burnout is 60.3 at 4–5 hours of sleep, 49.3 at 6–7, 42.5 at 7–8 and 30.5 at 9–10. Half of the students who sleep under 6 hours fall in the high-burnout group, compared with only 6% of those who sleep 8+ hours. Mental health stays flat at every sleep level. 19% of students sleep under 6 hours, and only 51% get 7+.
Insight: the damage from poor sleep shows up in burnout, not in the mental health score, so schools that only track mental health scores would miss it. Counsellors should watch sleep hours as an early warning sign, and schools should avoid early starts and late-night deadlines.
3. Screen time doesn’t change mood, but it raises burnout

Observation: the mood score stays flat from 0 to 12+ hours of screen time, but burnout climbs from 33.6 (0–2 hours) to 56.6 (more than 12 hours). 42% of students with 10+ screen hours are in the high-burnout group, compared with 10% of those under 4 hours.
Insight: a student can look “fine” on a mood check and still be heading to burnout. For schools and app developers, this means screen time needs its own tracking, with screen-free breaks built in, especially for online learning.
4. Caffeine gives no focus advantage and adds burnout

Observation: focus stays at about 29 to 30 in every caffeine group, from under 50 mg to almost 500 mg, while burnout rises from 41.5 to 49.9. Caffeine has no link with deadlines, jobs or sleep, so it adds burnout on its own. 41% of students take 300 mg or more.
Insight: many students lean on coffee to push through tiredness but in this data, it doesn’t buy any focus and costs more burnout. Counsellors and wellness teams can safely tell students that extra coffee is not a study strategy. Sleep and rest are.
5. Deadlines and part-time jobs stack up

Observation: burnout is 33.5 with neither, 43.3 with a job only, 47.3 with a deadline only and 58.4 with both. 61% of students with both are in the high-burnout group, compared with 2% of students with neither. A job does not reduce sleep (7.01 vs 7.02 hours) but still adds burnout.
Insight: a quarter of students carry both pressures, and they are the ones most at risk. Teachers can help by not stacking big deadlines on students who work, and schools can offer flexible due dates for them.
6. Social media hurts focus

Observation: focus falls from 33.7 (under 2 hours of social media) to 25.8 (4–6 hours), and productivity falls too. About 26% of students spend 4+ hours a day on social media.
Insight: social media is a small drain on productivity but a clear one on focus, and focus is what drives exam scores (see 1). Teachers and parents can protect study time by setting phone-free study blocks.
7. Exercise goes with lower burnout

Observation: burnout is 48.9 for students who exercise under 30 minutes and 43.5 for those who exercise 90 minutes or more. Exercise has no link with focus (r = -0.02). 60% of students already exercise 60+ minutes.
Insight: exercise helps with how drained students feel, not with how sharp they are. Schools can use sport and movement breaks as a burnout tool, and not as a grade booster.
8. Gender, academic level and internet quality don’t explain results

Observation: burnout, productivity and exam scores are almost equal across genders, academic levels and internet quality.
Insight: resources should not be targeted by who the student is. They should be targeted by habits (sleep, workload, screen time), which is where the real differences are. Poor internet is still worth fixing for access but in this data, it did not lower results.
9. What the top students look like

Observation: ID #21 (exam score 64.09) and ID #3376 (productivity 98.02, exam score 62.82, burnout 32.6, poor internet) both study 9 to 12 hours a day with very high focus.
Insight: the best results come from a lot of focused study while burnout is kept low. #3376 has no job and no deadline, and uses social media for only 0.48 hours a day, so she had the time and calm to study at that level. This is the profile that early warning systems should try to protect.

ACTIONABLE RECOMMENDATION

1. Teach focus, not just long hours (teachers and schools)

Build study support around focused blocks: a quiet place, phones away, short breaks. A focused 3 hours beat 7 unfocused hours in this data.
2. Make sleep the first thing to protect (schools, parents and counsellors)

Aim for 7+ hours a night. Avoid early starts and late-night deadlines where possible.
Add sleep hours to student check-ins, because mental health scores alone would miss the burnout it causes.
3. Build screen breaks into digital learning (schools and app developers)

Set screen-free time before bed and regular breaks during online classes. Track screen time on its own, since mood scores won’t show the problem.
4. Stop treating caffeine as a study tool (counsellors and wellness teams)

Tell students plainly that extra coffee doesn’t improve focus here and goes with more burnout. Encourage cutting heavy intake (300+ mg), especially late in the day, and pointing to sleep and rest instead.
5. Stop stacking pressure on working students (teachers and schools)

Spread big deadlines out, and offer flexible due dates or lighter loads to students who work. These are the students most at risk, and about one in four carries both a job and a deadline.
6. Protect study time from social media (teachers, parents and app developers)

Use phone-free study blocks and focus modes in study apps. The aim is to protect focus, which is what drives exam scores.
7. Use exercise as a burnout tool (schools)

Keep sport and movement breaks in the timetable. Present them as a way to feel less drained, and not as a way to raise grades.
8. Target by habits, not by who the student is (school leaders and EdTech teams)

Spend support on sleep, workload and screen time, and not on gender, level or internet quality. Keep fixing poor internet for access, but don’t expect it to explain results.
9. Build early warning systems around burnout and habits (school leaders and EdTech teams)

Track sleep, screen time, workload and caffeine, and flag students with several pressures at once (for example, a job, a deadline and short sleep). Learn from top students like #21 and #3376: lots of focused study with low burnout.

CONCLUSION

Going into this project, I had a few guesses. I thought sleep would change mental health, that poor internet would pull grades down, and that coffee would sharpen focus. None of that held up in the data, and that surprised me. What did show up was clear: study time and focus lift exam scores, and burnout follows sleep, screen time, deadlines, jobs and even caffeine. Academic level, gender and internet quality barely changed anything. For schools, teachers, counsellors and app developers, the message is simple: the habits students live with every day matter more than who they are, and burnout is the signal to watch. Students like ID #21 and ID #3376 show what good looks like: a lot of focused study while burnout is kept low. Extra coffee, late nights and long screen hours don’t buy better results, they only cost more burnout.
