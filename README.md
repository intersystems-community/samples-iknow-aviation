# samples-iknow-aviation
InterSystems iKnow and DeepSee sample solution based on events involving aircraft as registered by the National Transportation Safety Board.
# Installation
Import the latest [release](https://github.com/intersystems-community/samples-iknow-aviation/releases) in any namespace.
Run in terminal
```
d ##class(Aviation.Utils).Setup()
```

This project contains two demos:
# DeepSee Aviation Demo
The DeepSee Aviation demo demonstrates how the iKnow featues embedded in DeepSee can be used to combine analysis of structured and unstructured data. It can be configured by calling the SetupCube class method in this class. Check the "Using unstructured data in cubes" chapter in the "Defining DeepSee models" guide.
# iKnow Aviation Demo
The iKnow Aviation demo uses the same dataset, but just loads it as a normal standalone iKnow domain, which can be explored to the general iKnow APIs. This domain is fully defined through the domain definition in Aviation.ReportDomain and can be set up by calling its %Build() method. This class' SetupStandalone will invoke that %Build() method and call additional configuration code to ensure your security settings allow accessing the UI classes for the SAMPLES namespace. Check the "Using iKnow" guide in the documentation for more details.
The classes in this package represent events involving aircraft as registered by the National Transportation Safety Board.

Note on the data:
The dataset provided in this sample demo is only a lightweight subset of the full NTSB dataset, which is available from http://www.ntsb.gov. This data is supplied here for demonstration purposes only and neither intended nor warranted to be accurate.
Courtesy: National Transportation Safety Board
