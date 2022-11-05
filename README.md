# Task
Can we nest the Scaffold widget ? 
Yes, we can nest the Scaffold widget body with many widgets, it is like tree of widgets, so we nest as much as we can. Scaffold widget body, can accept any kind widget even it can Scaffold as well, inside the body, we can return as much as possible widgets.
how to reduse the rebuilding of the widget ?
we can avoid the rebuilding of the widget by using the const key word infront of the widget, so that flutter element tree doesnot rebuild, we can avoid setState so that all the widgets are in build method wont be called, we can use the provider to call specific widget if we want to update 
