---
title: "A-JavaScript-Class"
date: 2024-11-01
---

### How to create a JavaScript Class ###

In the example below, you have a class named "AI" and in this class it has two constructor variables: name and specialty.
The name is the name of the AI Tool or AI Application, and the specialty is what the AI Tool can do. There are 
three meethods, which behaves like functions: introduce, learn, and performTask that enables each instance to expand on 
what they do or what should be happening.


    class AI {
      constructor(name, specialty) {
          this.name = name;
          this.specialty = specialty;
        }

        introduce() {
          console.log(`Hello, I am ${this.name}, and I specialize in ${this.specialty}.`);
        }

        learn(newSkill) {
          console.log(`${this.name} is learning ${newSkill}...`);
        }

        performTask(task) {
          console.log(`${this.name} is performing task: ${task}.`);
        }
    }

    // Creating an instance of the AI class
    const aiBot1 = new AI('Copilot', 'Natural Language Processing');
    const aiBot2 = new AI('UltimateVision', 'Identifies all objects and gives their full profile or description.');
    
    // Using the methods
    aiBot1.introduce();
    aiBot1.learn('Machine Learning Algorithms');
    aiBot1.performTask('Data Analysis');

    aiBot2.introduce();
    aiBot2.learn('Animals');
    aiBot2.performTask('Watching Lions behavior.');
