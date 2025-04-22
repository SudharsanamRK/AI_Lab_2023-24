# Ex.No: 9  Logic Programming –  Computer Maintenance Expert System
### DATE: 22-04-2025                                                           
### REGISTER NUMBER : 212222040163
### AIM: 
Write a Prolog program to build a computer maintenance expert system.

###  Algorithm:
1. Start the program.
2. Write the rules for each fault in computer.
3. If system have printing problem, missing dots and no uniform printing then system fault on printer head.
4. If system have not printing, missing dots and spread inks then system fault on ribbon
5. If system have not printing, paper jam and out of paper then system fault on paper stuck in printer
6. Similarly define rules for all faults.
7. Define facts for system problems.
8. Find the fault of computer by passing query to system.
     
### Program:
```prolog
hypothesis(Patient, german_measles) :-
    symptom(Patient, fever),
    symptom(Patient, headache),
    symptom(Patient, runny_nose),
    symptom(Patient, rash).

hypothesis(Patient, flu) :-
    symptom(Patient, fever),
    symptom(Patient, headache),
    symptom(Patient, body_ache),
    symptom(Patient, conjunctivitis),
    symptom(Patient, chills),
    symptom(Patient, sore_throat),
    symptom(Patient, runny_nose),
    symptom(Patient, cough).

hypothesis(Patient, common_cold) :-
    symptom(Patient, headache),
    symptom(Patient, sneezing),
    symptom(Patient, sore_throat).

hypothesis(Patient, chicken_pox) :-
    symptom(Patient, fever),
    symptom(Patient, chills),
    symptom(Patient, body_ache),
    symptom(Patient, rash).

hypothesis(Patient, measles) :-
    symptom(Patient, cough),
    symptom(Patient, sneezing),
    symptom(Patient, runny_nose).

hypothesis(Patient, mumps) :-
    symptom(Patient, fever),
    symptom(Patient, swollen_glands).

symptom(raju, headache).
symptom(raju, sneezing).
symptom(raju, sore_throat).

symptom(kumar, fever).
symptom(kumar, headache).
symptom(kumar, runny_nose).
symptom(kumar, rash).

symptom(sita, fever).
symptom(sita, headache).
symptom(sita, body_ache).
symptom(sita, conjunctivitis).
symptom(sita, chills).
symptom(sita, sore_throat).
symptom(sita, runny_nose).
symptom(sita, cough).
```

### Output:
![image](https://github.com/user-attachments/assets/767708fb-ae56-4536-b7d0-04a5edcb5c30)

### Result:
Thus the simple omputer maintenance expert system was built sucessfully.
