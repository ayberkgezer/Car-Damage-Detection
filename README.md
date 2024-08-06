# Car Damage Detection on VGG-16

[![(article)](https://img.shields.io/badge/cs.CV-DOI%3A10.53608/estudambilisim.1421332.-B31B1B.svg)](https://dergipark.org.tr/en/pub/estudambilisim/issue/86200/1421332)

For this we used a CNN model, VGG16[[1]](https://arxiv.org/abs/1409.1556). We used our own dataset that we had prepared and trained the VGG16 model ourselves. Our study consisted of 4 main questions:

- Is it a car?
- Is there any damage on the car?
- In which part of the car is the damage?
- What is the level of damage?

We prepared and trained our own datasets within these 4 questions.

## Data Sets

| Data Sets                                   | Training | Validation |
| :--------                                   | :------- | :--------- |
| Is it a car?                                | `920`    | `230` |
| Is there any damage on the car?             | `1840`   | `460` |
| In which any part of the car is the damage? | `976`    | `171` |
| What is the level of damage?                | `979`    | `171` |

We used our original dataset, which consists of a total of 5,757 photographs.



## Is it a car?

| Data Sets                                   | Training | Validation |
| :--------                                   | :------- | :--------- |
| Car                               | `920`    | `230` |

The result we will get here is only querying whether there is a car or not.

## Is there any damage on the car?

| Data Sets                                   | Training | Validation |
| :--------                                   | :------- | :--------- |
|   Damaged          | `920`    | `230` |
|   Undamaged          | `920`    | `230` |

We have done this training in order to determine whether there is a similar damage at this stage and to continue with the other stages according to the result.

## In which any part of the car is the damage?

| Data Sets                                   | Training | Validation |
| :--------                                   | :------- | :--------- |
| Front                                | `418`    | `73` |
| Rear                                | `287`    | `50` |
| Side                                | `271`    | `48` |

our aim here is to determine which part of the car the damaged area in the photo belongs to. We trained our parameters as front, back and side.

## What is the level of damage?

| Data Sets                                   | Training | Validation |
| :--------                                   | :------- | :--------- |
| Minor                                | `278`    | `48` |
| Moderate                                | `315`    | `55` |
| Severe                               | `386`    | `68` |

Now that we know the damage is and where it is, it's up to us to separate the level of damage we set ourselves.

## Accuracy Rating

| Training                                    | Accuracy Rating |
| :--------                                   | :-------        |
| Is it a car?                                | %98             |
| Is there any damage on the car?             | %90             |
| In which any part of the car is the damage? | %70             |
| What is the level of damage?                | %66             |

![Accuracy Rating graph](https://i.hizliresim.com/4gqn2gn.png)

## Result Exp

![Result](https://i.hizliresim.com/15uh2nz.jpg)

## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

## Authors

- [@ayberkgezer](https://www.github.com/octokatherine)
- [@TediTae](https://github.com/TediTae/)
