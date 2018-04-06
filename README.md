# react-native-coachmasks
## DEMO

<img src="https://github.com/TranLuongTuanAnh/react-native-coachmasks/blob/master/coachmarkSimulation.gif">


# How to use 
 ```
 
 const CM = [];
     CM.push(
      {
        tooltip: 'The first steps of your tutorial',
        position: {
          top:35,
          left: width - 58,
        },
        tooltipPosition: {
          width: 300,
          height: 120,
          top: 110,
          left: (width - 300) / 2,
        },
        style: {
          width: 50,
          height: 50,
          borderRadius: 30,
        },
      },
      {
        tooltip: 'The second steps of your tutorial',
        position: {
          top:height - 70,
          left: width - 91,
        },
        tooltipPosition: {
          width: 300,
          height: 120,
          top: height - 210,
          left: (width - 300) / 2,
        },
        style: {
          width: 70,
          height: 70,
          borderRadius: 35,
        },
      },
      {
        tooltip: 'The last steps of your tutorial',
        position: {
          top:height - 75,
          left: width - 305,
        },
        tooltipPosition: {
          width: 300,
          height: 120,
          top: height - 210,
          left: (width - 300) / 2,
        },
        style: {
          width: 80,
          height: 80,
          borderRadius: 40,
        },
      },
    );
    
   
    <CoachMarks
      numberOfSteps={CM.length}
      coachMarks={CM}
      congratsText={"Welcome to react-native-coachmark!\n"+"It helps you easily create Coach Marks to enhance user experience"}
      congratsImage={require('./ic_public.png')}
      visible={true}
      onClose={() => {}}
    />
   
 ```
# Properties

```
<CoachMarks
      numberOfSteps={CM.length}
      coachMarks={CM}
      congratsText={"Welcome to react-native-coachmark!\n"+"It helps you easily create Coach Marks to enhance user experience"}
      congratsImage={require('./ic_public.png')}
      visible={true}
      onClose={() => {}}
/>
```

| Prop  | Description |Default |
| ------------- | ------------- | ------------- |
| **coachMarks**  | This is array contains data of coachmasks(see [Properties of each step](https://github.com/TranLuongTuanAnh/react-native-coachmasks/blob/master/README.md#properties-of-each-step))  |None  |
| **numberOfSteps**  | number of steps  | None  |
| **congratsText**  | The text is shown in first view | None  |
| **congratsImage**  | The image is shown in first view | None  |
| **visible**  | CoachMarks is shown or hidden | false  |
| **onClose**  | action is called in last step | None  |

## Properties of each step

```
   {
        tooltip: 'The first steps of your tutorial',
        position: {
          top:35,
          left: width - 58,
        },
        tooltipPosition: {
          width: 300,
          height: 120,
          top: 110,
          left: (width - 300) / 2,
        },
        style: {
          width: 50,
          height: 50,
          borderRadius: 30,
        },
    }
```

| Prop  | Description |Default |
| ------------- | ------------- | ------------- |
| **tooltip**  | Explain text show in this step  |None  |
| **position**  | position of mask  |None  |
| **tooltipPosition**  | position of tooltip  |None  |
| **style**  | style of CoachMark  |None  |

# License
This project is licenced under the [MIT License.](https://opensource.org/licenses/mit-license.html)
