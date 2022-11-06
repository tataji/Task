# Task
Can we nest the Scaffold widget ? 
Yes, we can nest the Scaffold widget body with many widgets, it is like tree of widgets, so we nest as much as we can. Scaffold widget body, can accept any kind widget even it can Scaffold as well, inside the body, we can return as much as possible widgets.

how to reduse the rebuilding of the widget ?
we can avoid the rebuilding of the widget by using the const key word infront of the widget, so that flutter element tree doesnot rebuild, we can avoid setState so that all the widgets are in build method wont be called, we can use the provider to call specific widget if we want to update.

How can we access plartform(android/ios) specifc code from flutter'
we can access the plartform specifc code using the method channel and event channel communication, Using the method channel we can invoke method in the native code and excute the native specific code there and return the value, In the event channel we can send and recive the stream of data 

What is BuildCOntext? and its imprortance 

Build context is to identify the widget location and position in the widget tree, so that we can update the data of a widget, and also we can create global singleton class and pass the context to that class and get the configuration we need in every where in the app

var list1 =['I','@','flutter'];
final list2 = list1;
list2[2] = 'Dart';
const list3= list1;
Will the last two lines compiled ?
list2[2] = 'Dart'; this line will be compiled and executed, we can replace the 'flutter' with 'dart' string in list2  
const list3= list1;  this line will not be compiled, will get a compile time error Const variables must be initialized with a constant value. that means we need to change the list1 to const, but if we do this list2 can not be modifed.
  
 String  longOperationMethod(){
    var counting =0;
    for (var i=1;i<=1000000000;i++){
      counting = i;
      print(i);
    }
     return '$counting! times i print the values';
  }
  
  Fix for above block is the following 
  
   Future<String>  longOperationMethod() async{
    var counting =0;
    for (var i=1;i <= 1000000000; i++){
      counting = i;
    }
     return '$counting! times i print the values';
  }
  longOperationMethod().then((val){
    print(val);
  });
  
 ![Screenshot (4)](https://user-images.githubusercontent.com/12562731/200171343-e07c8572-2abe-4dba-a194-0f2d5c49e97d.png)                               
  and result would be 1000000000! times i print the values
  
Difference between Provider and Mobx, can we use both together and write code to demonstrate it 

Using provider we can update the specific widget in the widget tree using the consumer widget, we can access the provider value at any place in the app, if we add our provider in the root of the tree 
Mobx uses obesrver and obeservale patteren 
  
  
  
