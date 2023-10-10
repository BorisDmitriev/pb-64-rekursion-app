# School app
[![Status overview badge](../../blob/badges/.github/badges/main/badge.svg)](#-results)

* create an app to add, remove, read and edit Students and Classes in a School

   * the school model:
  ```js
     School=[ classObject1,classObject2,....]
  ```

   * the class model: 
   ```js
    {
        name: "FbW3",
        students: [studentObject1, studentObject2,...],
    }
    ```

    * the Student model: 
  
    ```js
    {
            name: "Pilar",
            email: "pilar@yahoo.com",
            city: "Berlin",
    }
    ```

school data model:
```js
 [
  {
    name: "FbW1",
    students: [
      {
        name: "Alex",
        email: "alex@yahoo.com",
        city: "Berlin",
      },
      {
        name: "Max",
        email: "max@yahoo.com",
        city: "Hamburg",
      },
    ],
  },

  {
    name: "FbW2",
    students: [
      {
        name: "Jon",
        email: "jon@yahoo.com",
        city: "Berlin",
      },
      {
        name: "Pilar",
        email: "pilar@yahoo.com",
        city: "Berlin",
      },
    ],
  },
  {
    name: "FbW3",
    students: [],
  },
]
```




### Tasks
## Task1: Creating a class:
- Create a function named `createClass` to add a new class.
- The `createClass` function should receive an argument(object) that holds the name of the class `name` and an empty array for `students`.

## Task2: Adding a student:
- Create a function named `createStudent` to add a new student.
- The `createStudent` function should receive an argument(object) that holds *student Data*.
-  The student data should look like this example code bellow:
```js
  {
        classID: 21,
        name: "Pilar",
        email: "pilar@yahoo.com",
        city: "Berlin",
  }
 ```
## Task3: Removing a class:
- Create a function to remove the class and name it `removeClass`.
- The `removeClass` function should take an argument of `classID` for the ID of the class.

## Task4: Removing a student:
- Create a function named `removeStudent` to remove a student from a class.
- The `removeStudent` function should receive an argument(object) that holds `classID` for the ID of a class and `studentID` for the ID of a student.

## Task5: Editing a student:
- Create a function to edit an existing student and name it `editStudent`.
- The `editStudent` function should take an argument(object) that holds `classID` for the ID of the class, `studentID` for the ID of the student, `email` for student Email, `city` for the student's city, and `name` for the student's name, __Make sure to use the exact names of the object values__.

## Task6: Rendering School data:
- Create a function to render the school data, name it `RenderSchoolTemplate`.
- The `RenderSchoolTemplate` function should return the school data as a string formated the same way as below:
```js
 School Classes: 
------------------ 
 FbW1 - (class ID: 1): 
  1- Alex, alex@yahoo.com, Berlin - (student ID: 1).
  2- Max, max@yahoo.com, Hamburg - (student ID: 2).
******************************************** 
 FbW2 - (class ID: 2): 
  1- Jon, jon@yahoo.com, Berlin - (student ID: 1).
  2- Pilar, pilar@yahoo.com, Berlin - (student ID: 2).
******************************************** 
 FbW3 - (class ID: 3): 
   The class is empty 
******************************************** 
  Total Classes 3, total students 4
```

[//]: # (autograding info start)
# <img src="https://github.com/DCI-EdTech/autograding-setup/raw/main/assets/bot-large.svg" alt="" data-canonical-src="https://github.com/DCI-EdTech/autograding-setup/raw/main/assets/bot-large.svg" height="31" /> Results
> ⌛ Give it a minute. As long as you see the orange dot ![processing](https://raw.githubusercontent.com/DCI-EdTech/autograding-setup/main/assets/processing.svg) on top, CodeBuddy is still processing. Refresh this page to see it's current status.
>
> This is what CodeBuddy found when running your code. It is to show you what you have achieved and to give you hints on how to complete the exercise.


### Task1: Creating a class

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status0.svg) | `createClass` function takes class object as argument and adds it to `school` |

### Task2: Adding a student

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status1.svg) | `createStudent` function takes student object as argument and adds it to `school` |

### Task3: Removing class

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status2.svg) | `removeClass` function should remove a class based on class ID passed as a argument |

### Task4: Removing student

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status3.svg) | `removeStudent` function should remove a student based on passed object containing class ID and student ID |

### Task5: Editing student

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status4.svg) | `editStudent` function should edit a student based on passed object containing class ID, student ID and new values |

### Rendering

|                 Status                  | Check                                                                                    |
| :-------------------------------------: | :--------------------------------------------------------------------------------------- |
| ![Status](../../blob/badges/.github/badges/main/status5.svg) | `RenderSchoolTemplate` function should return all school data in string |
| ![Status](../../blob/badges/.github/badges/main/status6.svg) | Returned string is formatted as specified |



[🔬 Results Details](../../actions)
[🐞 Tips on Debugging](https://github.com/DCI-EdTech/autograding-setup/wiki/How-to-work-with-CodeBuddy)
[📢 Report Problem](https://docs.google.com/forms/d/e/1FAIpQLSfS8wPh6bCMTLF2wmjiE5_UhPiOEnubEwwPLN_M8zTCjx5qbg/viewform?usp=pp_url&entry.652569746=PB-Function2-School-App)


[//]: # (autograding info end)