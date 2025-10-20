[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/oqKLEXJJ)
# 🎓 Ethical Admissions Algorithm Simulation

This repository is a classroom exercise exploring **ethics and fairness in algorithmic decision-making** — specifically in college admissions.

You’ll implement and reflect on how feature selection and weighting can impact fairness, transparency, and equity in automated systems.

---

## 🧩 Overview

You are part of the admissions committee for **Anonymous University**, located near Anonymous City.  
Due to a large number of applications, the committee decides to use an algorithm to help **rank and shortlist applicants**.

Your task:
- Decide which factors to include (GPA, test scores, extracurriculars, essays, recommendation letters, legacy status, income, etc.)
- Assign weights to each factor.
- Compare outcomes under two models:
  - **Blind model**: Ignores sensitive factors.
  - **Aware model**: Includes them intentionally to promote fairness (e.g., extra weight for first-gen or low-income applicants).

---

## ⚙️ How to Run

You can run the code on any online Java compiler (e.g. [Replit](https://replit.com/~) or [Programiz Java Compiler](https://www.programiz.com/java-programming/online-compiler))  
or locally via terminal:

```bash
javac Applicant.java Admissions.java Main.java
java Main
```

Alexis Quintero

# Feature Selection & Design
- What variables did you include, and why?
  - I included income, firstgen, disability, and ethnicity for the aware model. I included this because I think that students that meet this criteria should have more opportunity

- Did you exclude any sensitive features? Why or why not?
  - I excluded legacy and locality for the aware model. I believe that this should not matter when considering acceptance into a college. 


- Should “legacy” still carry a positive weight?
  - I personally do not think so, I think that students should be judged based on their own achievements and not their parents. I made it so that legacy is actually negative -0.01 points to even out the admissions. 

- What other features (e.g., proximity, essay strength, disability) might you add or adjust?
  - I adjusted extra curriculars and gpa to weigh less, then i increased the essay and recomendations score. I thnk that these are important things to keep in mind. Perhaps a student is busy or doesnt have time for extra curriculars. 

# Fairness & Outcomes
- Between the blind and aware models, which applicants benefited or lost out?
  - Applicants mostly lost or benefited in the aware model as there is where I changed the most criteria, mostly the ones losing out are people who relied on legacy, or locality. 

- Which applicants specifically benefited from the aware model?
  - Carlos rivera, Fatima Al-Sayed, George Johnson

- Does adding income or first-generation status make the system fairer or less fair? Why?
  - I think it makes it more fair by providing more opportunity for people with disadvatages to pursue their education. 

- Which model feels more fair overall, and why?
  - I think the aware model feels more fair because it considers more criteria, and other factors that impact admission

# Transparency & Accountability
- How transparent is your algorithm?
  - My algorithm prioritises people with disadvantages such as income, disability.

- Could you clearly explain a rejection to an applicant?
  - thanks to the model we know exactly where the points are going, so yes

- Would you feel comfortable if this algorithm evaluated your application? Why or why
not?
  - Yes I would feel comfortable, I think that this algorithm considers things fairly. 

# Broader Implications
- What risks might arise if such an algorithm were used in real admissions?
  - There might be a bias as I made this myself with my opinions and what I think. Which might lead to any issues for "discrimination" or "unfairness"

- What real-world parallels exist (e.g., hiring, policing, scholarships)?
  - Yes hiring processes and scholarships are all run by algorithms. 

- What does this exercise reveal about fairness in algorithmic decision systems?
  - It is hard and difficult to decide what is fair and to try to elimante bias, theres is too many factors to consider

- Can algorithms ever be truly fair, or do they just shift where bias appears?
  - In my opinion they cannot, they can get close, but someway somehow their is always bias. Sometimes it may be hard to see.

- How should fairness and accountability be balanced in automated decisions?
  - There should be a balance however it ultimately comes down to the individual organizations themseleves that are making these algorithms and what they want to prioritize or not. 
