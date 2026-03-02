# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  ExampleParent <|-- ExampleChild
  class ExampleParent{
        - name: string
        - email: string
        - password: string
        + login(user: string, pass: string) boolean
        + get_email() string
  }
  class ExampleChild{
        - badges vector~string~
        + add_badge(title: string)
        + get_badges() vector~string~
  }

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
```
