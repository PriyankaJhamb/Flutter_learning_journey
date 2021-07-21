Flutter:

Tour of Dart. 
Flutter Widgets
Assignments-->UI Replications
Flutter and Firebase -->Multimedia and DB Operations
Project Activity


1. JDk and its Path setup
2. Android Studio
3. Plugin-->FLutter in Android Studio
4. Flutter SDK
5. Link the SDK path in Android Studio

## Pre-requirements:

8GB RAM
i3/i5 Processor

## Online site
dartpad.dev


## Program for Water Bottle Sensor:
It has 3 operations--> 
1. Update how much water we drank.
2. Update if it is empty.
3. Update if it is refilled.
need to maintain the quantity in all 3 secenarios.

```
void main() {
  //water measure in litres
  double threshold_value=7.5;
  double sensor=7.5;
  double water_drank= 6.5;
  double water_fill=7.5;
  
  //first scenario
  
  // full
  if (sensor==threshold_value)
     {
        print("Water bottle is full");
      }
  
  //empty
  
  if(sensor==0.0)
  {
    print("water bottle is empty.");
  }
  
  //2nd scenario
  
  if (water_drank<=sensor)
  {
    sensor-=water_drank; 
    print("${sensor} litre of water is left.");
  }
  else
  {
    print("required water is not in the bottle");
  }
  
  //3rd scenario
  
  if (water_fill>(threshold_value-sensor))
  {
    print("Water is more that the water bottle can contain");
  }
  else
  {
    sensor+=water_fill;
    print("${sensor} litre of water is in the bottle");
  }
  
}

```