# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram

  class AccuracyTest{
        - phrase: string
        - accuracy: float
        + generate_phrase(phrases: vector~string~)
        + get_phrase() string
        - calculate_accuracy(typed: string, goal: string)
        + get_accuracy() string
  }

  class SpeedTest{
        - phrase: string
        - time: float
        - speed: float
        + generate_phrase(phrases: vector~string~)
        - calculate_speed(time: float, words: int)
        + get_speed() float
  }

 class User{
      - username: string
      - password: string
      - email: string
      - accuracies: vector~float~
      - speeds: vector~float~
      + add_accuracy_test(accuracy: float)
      + add_speed_test(speed: float)
      + get_accuracies() vector~float~
      + get_speeds() vector~float~
      + get_user() string
  }
```
