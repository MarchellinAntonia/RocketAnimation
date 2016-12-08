# RocketAnimation
Learn how to build animation in android,  used rocket animation as example (Android)

## Getting Started

These app show animations can calculate the nearest neighbor coordinate using euclidian distance equation, given some coordinate in ArrayList then system will calculate distance each coordinate with current location.
in this project there is 4 main class:
- Coordinates (Object Class for coordinates with its attributes: place, latitude, longitude)
- Distances (Object Class for distances with its attributes: name, distances)
- DummyActivity (tha main activity)
- DummyCoordinates (contain some main method to calculate distance, calculate nearest distance, add market, etc)

### Code

you need to import ValueAnimator to make this rocket animation

```
import android.animation.ValueAnimator;
```

then you make class that extend BaseAnimationActivity, it will generate Override method onAnimationUpadte, put that method inside ValueAnimator.addUpdateListener
example:

```
valueAnimator.addUpdateListener(new ValueAnimator.AnimatorUpdateListener() {
  @Override
  public void onAnimationUpdate(ValueAnimator animation) {
    float value = (float) animation.getAnimatedValue();
    mRocket.setTranslationY(value);
  }
});
```

## Built With

* IDE - Android Studio 2.1.3
* Operating System - Ubuntu

## Authors
* **Artem Kholodnyi**
* **Marchellin Antonia**

## Screenshot
* the animation list <br />
<img src="https://cloud.githubusercontent.com/assets/12492522/20997700/b4b16fb8-bd3a-11e6-9373-7e77f694aa34.png" width="300">
<br />
* the rocket first state <br />
<img src="https://cloud.githubusercontent.com/assets/12492522/20997699/b4ac1b08-bd3a-11e6-8518-dbe4217db80c.png" width="300">


