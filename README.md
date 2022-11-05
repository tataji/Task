# Task
Can we nest the Scaffold widget ? 
Yes, we can nest the Scaffold widget body with many widgets, it is like tree of widgets, so we nest as much as we can. Scaffold widget body, can accept any kind widget even it can Scaffold as well, inside the body, we can return as much as possible widgets.

how to reduse the rebuilding of the widget ?
we can avoid the rebuilding of the widget by using the const key word infront of the widget, so that flutter element tree doesnot rebuild, we can avoid setState so that all the widgets are in build method wont be called, we can use the provider to call specific widget if we want to update.

How can we access plartform(android/ios) specifc code from flutter'
we can access the plartform specifc code using the method channel and event channel communication, Using the method channel we can invoke method in the native code and excute the native specific code there and return the value, In the event channel we can send and recive the stream of data 

