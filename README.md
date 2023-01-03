# AiSL
ASL translation powered by AI.

## Inspiration

Only 1%, or 500,000 people in the US can understand ASL. However, there is only 1 interpreter per 50 ASL users, which creates communication difficulties for the affected community.

Compared to the hearing, only 53.3% of the deaf are employed, compared to 75.8% for the hearing. We wanted to help ASL users break down employment barriers and other challenges they may face by providing direct and live translation.

## What it does

AiSL performs live sign-to-text translation powered by a YoloV5 object detection model. The model can run on any image or video, including live webcams.

## How we built it

We created a YoloV5 model using AlexeyAB’s [darknet repository](https://github.com/AlexeyAB/darknet), a [tutorial](https://blog.roboflow.com/how-to-train-yolov5-on-a-custom-dataset/) from roboflow and a [Roboflow dataset](https://public.roboflow.com/object-detection/american-sign-language-letters/1) formatted for YoloV5. The model trained for 300 epochs on these 3000+ labeled images.

## Challenges we ran into
Some predictions were inaccurate and had very low confidence– the model tended to confuse the letters “M” and “N” for example. 

## Accomplishments that we're proud of
We achieved around 90% confidence on some predictions and were able to finish the project on time!
![ASL sign for “u”](https://imgur.com/a/8h1Ipps)

## What we learned

To start, we had to learn the basics of ASL to build a project that would serve ASL user needs. In addition, we learned how to train a model on a larger dataset than we’re used to!

## What's next for AiSL 

With AiSL, we hope to create direct integrations into apps such as Zoom and Facetime, allowing ASL users to communicate with a click of a button. We also plan to train the model on a larger dataset including words, so users don’t have to spell out entire sentences.  We’d also train the AI for a much longer period of time to improve accuracy and confidence. Lastly, we plan to receive more feedback from potential AiSL users to improve our model and develop a mobile application.

