---
title: Python Coding Lesson 7
layout: post
author: anshu.attavar
permalink: /python-coding-lesson-7/
source-id: 1wkv7ImYmSnCJjWML75ncvsrXxz7Rk59ObrOI-UDHa0Y
published: true
---
This lesson I started the lesson 'The Student Becomes the Teacher'. You had to make a set of code that gives students averages, scores and group averages. By the end of the lesson I had done up to here:

lloyd = {

    "name": "Lloyd",

    "homework": [90.0, 97.0, 75.0, 92.0],

    "quizzes": [88.0, 40.0, 94.0],

    "tests": [75.0, 90.0]

}

alice = {

    "name": "Alice",

    "homework": [100.0, 92.0, 98.0, 100.0],

    "quizzes": [82.0, 83.0, 91.0],

    "tests": [89.0, 97.0]

}

tyler = {

    "name": "Tyler",

    "homework": [0.0, 87.0, 75.0, 22.0],

    "quizzes": [0.0, 75.0, 78.0],

    "tests": [100.0, 100.0]

}

# Add your function below!

def average(numbers):

    total = sum(numbers)

    total = float(total) / float(len(numbers))

    return total

That was getting the averages from the children's scores. This was the final code after homework:

lloyd = {

    "name": "Lloyd",

    "homework": [90.0, 97.0, 75.0, 92.0],

    "quizzes": [88.0, 40.0, 94.0],

    "tests": [75.0, 90.0]

}

alice = {

    "name": "Alice",

    "homework": [100.0, 92.0, 98.0, 100.0],

    "quizzes": [82.0, 83.0, 91.0],

    "tests": [89.0, 97.0]

}

tyler = {

    "name": "Tyler",

    "homework": [0.0, 87.0, 75.0, 22.0],

    "quizzes": [0.0, 75.0, 78.0],

    "tests": [100.0, 100.0]

}

# Add your function below!

def average(numbers):

    total = sum(numbers)

    total = float(total) / float(len(numbers))

    return total

def get_average(student):

    homework = average(student["homework"])* 0.1

    quizzes = average(student["quizzes"])* 0.3

    tests = average(student["tests"])* 0.6

    avrg = homework + quizzes + tests

    return avrg

def get_letter_grade(score):

    if score>= 90:

        return 'A'

    elif score>= 80:

        return 'B'

    elif score>= 70:

        return 'C'

    elif score >= 60:

        return 'D'

    else:

        return 'F'

def get_class_average(students):

    results = []

    for student in students:

        results.append(get_average(student))

    return average(results)

print get_class_average(students)

print get_letter_grade(get_class_average(students))

