# YAML Syntaxes
- YAML :- YAML Ain't Markup Language
- File extension should be .yml or .yaml
- There are no special symbols or default lines of code required to start YAML
- Starting of YAML can be denoted using 3 dots (...) - Optional
- Ending of YAML can be denoted using 3 hyphens (---)  - Optional but if you are going the multiple config in single file you need to use 3 hyphens
  - EX: 
    ```
       config-1
       ---
       config-2
    ```
- In YAML data will be represented as key-values pairs
- Key should be unique in same block of config on same indentation (2 space)
- Key can't be a empty one
- Comments will be represented usinh Hash Tag (#)
--------------------------------------------------------
# YAML Data Types
## 1. Scalar Data Types
- Numbers: It can be **Integer** and **Floating** values
  - Ex: 23, 25.5
- Boolean: The value can **True** or **False**
  - Ex: is_student: true/false
- Strings: Text enclosed in single or double qutoes
  - email: "muralialakuntla3@gmail.com"
- Null: no value represented as **null or ~**
## 2. Sequence/Array Data Type
- list of items, represented using dash followed by space
  - Ex:
    ```yml
    fruits:
      - apple
      - cherry
      - berry
    fruit: [apple, cherry, berry]
    ```    
## 3. Mapping/Dictionary Data Type
- data represented as key and value pair (key: value)
  - ex: name: murali
---------------------------------------------------
# Types of Strings
## 1. Normal String
- text enclosed in single or double quotes
- Ex:
```yml
jobDescription: "Req 3 years of cloud devops engg. he/she should have exp with kubernetes. he/she should be able to lead the Team,"
output:
  Req 3 years of cloud devops engg. he/she should have exp with kubernetes. he/she should be able to lead the Team.
```
## 2. Literal Block String (|)
- the input will be given line by line and it will be represented using pipe(|) symbol
- Ex:
```yml
jobDescription: |
  Req 3 years of cloud devops engg.
  he/she should have exp with kubernetes.
  he/she should be able to lead the Team.
output:
  Req 3 years of cloud devops engg.
  he/she should have exp with kubernetes.
  he/she should be able to lead the Team.
```
## 3. Folded Block String (>)
- the input will be given line by line and it will be represented using right arrow (>) symbol
```yml
jobDescription: |
  Req 3 years of cloud devops engg.
  he/she should have exp with kubernetes.
  he/she should be able to lead the Team.
output:
  Req 3 years of cloud devops engg. he/she should have exp with kubernetes. he/she should be able to lead the Team.
```
----------------------------------------------------------
# YAML Example 
```yaml
# Learners Data
learners:
  learner1:
    name: murali   # dictionary type - learners.learner1.name
    age: 30        # integer
    email: "kiran@gmail.com" # string
    isCourseCompleted: false  # boolean
    height: 5.8   # flot
    isEmployed: null   # Null
    courses_enrolled:  # array
      - aws
      - devops
      - azure 
  learner2:
    name: krishna   # dictionary type - learners.leraner2.name
    age: 30        # integer
    email: "Abhi@gmail.com" # string
    isCourseCompleted: false  # boolean
    height: 5.8   # flot
    isEmployed: null   # Null
    courses_enrolled:  # array
      devops:
        - docker
        - k8s
        - github actions
      cloud: [aws, azure]
---
# Trainers data
learners:
  learner1:
    name: murali   # dictionary type - learners.learner1.name
    age: 30        # integer
    email: "kiran@gmail.com" # string
```









