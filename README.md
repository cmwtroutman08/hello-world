export const dayToSchedule = [
    "No School",
    "Normal",
    "Normal",
    "Normal",
    "Normal",
    "Normal",
    "No School"
]

export const ignoredPeriods= [
          "No School",
          "Before School",
          "Warning Bell",
          "Passing Time",
          "Teacher Time"
];

       ]
}

export function schedule(typeOfDay){
  switch (typeOfDay) {
   case "No School" :
      return [
          {name: "No School", start: "12:00a", end: "12:00a"}
         ];
      break;
    case "Normal": 
      return [
           {name: "Period 1", start: 490, end: 540},
           {name: "Passing Time", start: 540, end: 545},
           {name: "Period 2", start: 545, end: 585}, 
           {name: "Passing Time", start: 585, end: 590},
           {name: "Period 3", start: 590, end: 630},
           {name: "Passing Time", start: 630, end: 635},
           {name: "Break", start: 635, end: 655},
           {name: "Period 4", start: 655, end: 714}, 
           {name: "Lunch", start: 714, end: 740},
           {name: "Period 5", start: 740, end: 790},
           {name: "Passing Time", start: 790, end: 795},
           {name: "Period 6", start: 795, end: 850},
           {name: "Passing Time", start: 850, end: 855},
           {name: "Period 7", start: 855, end: 905}
          ];
      break;
    case "Club Day": 
      return [
          {name: "Period 1", start: 490, end: 540},
           {name: "Passing Time", start: 540, end: 545},
           {name: "Period 2", start: 545, end: 570}, 
           {name: "Period 3", start: 570, end: 595},
           {name: "AM Club", start: 595, end: 655},
           {name: "Period 4", start: 655, end: 714}, 
           {name: "Lunch", start: 714, end: 740},
           {name: "Period 5", start: 740, end: 775},
           {name: "PM Club", start: 775, end: 835},
           {name: "Period 6", start: 835, end: 865},
           {name: "Passing Time", start: 865, end: 870},
           {name: "Period 7", start: 870, end: 905}
          ];
      break;
   case "PM Activity": 
      return [
           {name: "Before School", start: 395, end: 455}, 
           {name: "Warning Bell", start: 455, end: 460},
           {name: "Period 1", start: 460, end: 500},
           {name: "Passing Time", start: 500, end: 504},
           {name: "Period 2", start: 504, end: 547}, 
           {name: "Passing Time", start: 547, end: 551},
           {name: "Period 3", start: 551, end: 591},
           {name: "Passing Time", start: 591, end: 595},
           {name: "Period 4", start: 595, end: 635}, 
           {name: "Passing Time", start: 635, end: 639},
           {name: "Period 5, 1st Wave", start: 639, end: 661},
           {name: "Period 5, 2nd Wave", start: 661, end: 687},
           {name: "Period 5, 3rd Wave", start: 687, end: 713},
           {name: "Passing Time", start: 713, end: 717},
           {name: "Period 6", start: 717, end: 757},
           {name: "Passing Time", start: 757, end: 761},
           {name: "Period 7", start: 761, end: 801},
           {name: "Passing Time", start: 801, end: 805},
           {name: "PM Activity", start: 805, end: 875},
           {name: "Teacher Time", start: 875, end: 915}
          ];
      break;
    case "Assembly":
      return [
           {name: "Before School", start: 395, end: 455},
           {name: "Warning Bell", start: 455, end: 460},
           {name: "Period 1", start: 460, end: 505},
           {name: "Passing Time", start: 505, end: 509},
           {name: "Period 2", start: 509, end: 557}, 
           {name: "Passing Time", start: 557, end: 561},
           {name: "Period 3", start: 561, end: 606},
           {name: "Passing Time", start: 606, end: 610},
           {name: "Assembly", start: 610, end: 650},
           {name: "Passing Time", start: 650, end: 654},
           {name: "Period 5, 1st Wave", start: 654, end: 676},
           {name: "Period 5, 2nd Wave", start: 676, end: 702},
           {name: "Period 5, 3rd Wave", start: 702, end: 728},
           {name: "Passing Time", start: 728, end: 732},
           {name: "Period 4", start: 732, end: 777},
           {name: "Passing Time", start: 777, end: 781},
           {name: "Period 6", start: 781, end: 826},
           {name: "Passing Time", start: 826, end: 830},
           {name: "Period 7", start: 830, end: 875},
           {name: "Teacher Time", start: 875, end: 915}
          ];
      break;
    case "7 Period": 
      return [
           {name: "Before School", start: 395, end: 455},
           {name: "Warning Bell", start: 455, end: 460},
           {name: "Period 1", start: 460, end: 512},
           {name: "Passing Time", start: 512, end: 516},
           {name: "Period 2", start: 516, end: 571}, 
           {name: "Passing Time", start: 571, end: 575},
           {name: "Period 3", start: 575, end: 627},
           {name: "Passing Time", start: 627, end: 631},
           {name: "Period 4", start: 631, end: 683},
           {name: "Passing Time", start: 683, end: 687},
           {name: "Period 5, 1st Wave", start: 687, end: 712},
           {name: "Period 5, 2nd Wave", start: 712, end: 738},
           {name: "Period 5, 3rd Wave", start: 738, end: 764},
           {name: "Passing Time", start: 764, end: 768},
           {name: "Period 6", start: 768, end: 820},
           {name: "Passing Time", start: 820, end: 824},
           {name: "Period 7", start: 824, end: 875},
           {name: "Teacher Time", start: 875, end: 915}
          ];
      break;
    case "Exam": 
      return [
           {name: "Before School", start: 395, end: 450},
           {name: "Before Exam 1", start: 450, end: 480},
           {name: "Exam 1", start: 480, end: 570},
           {name: "Passing Time", start: 570, end: 600},
           {name: "Exam 2", start: 600, end: 690}, 
           {name: "Lunch", start: 690, end: 765},
           {name: "Make-Up", start: 765, end: 855},
           {name: "Teacher Time", start: 855, end: 915}
          ];
      break;
  }
}
