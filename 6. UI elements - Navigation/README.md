# User Interface native elements
Because a mobile application can have so many features and actions taken cared of, it is important to be able to add special designed elements for each action to improve user experience: for instance, to navigate to the previous page the user would expect a button on the left side of the application because this is consistent with turning left to go back to one previous place - therefore, it is expected. No user would think a toogle would take him or her back to the previous page, just like no one will think an image will expect an input.

## Buttons
_What does this button do?_
<p align="left"><img alt="But-buttons" src="https://github.com/microsoft-dx/xamarin-fundamentals-ui/blob/master/Images/buttons.png?raw=true" margin=auto></p>

[Image source](https://codepen.io/g13nn/pen/yqiDG/image/large.png)

Ever sincer Dexter's sister Dee Dee started pushing buttons in her brother's laboratory, people started to _experience_ pushing buttons, having already in their subconscious that something would (or at least should) happen.

In terms of mobile applications, buttons are used generally to submit or enter data - any user would first complete some text entries and push a button after, expecting for that data to be added.

In the shopping list application, it was previously mentioned that the MainPage consist of two parts, the content and the action part. In the action part, a button is added to allow the user to add a new element to the list - add a suggestive icon to that button and you come up good user experience.
```
<Button 
   x:Name="addNewItem_button"
   HorizontalOptions="Center" 
   VerticalOptions="CenterAndExpand" 
   Margin="0,0,0,10"
   WidthRequest="48"
   HeightRequest="48"
   BackgroundColor="Transparent"
   Image="ic_add_box_black_48dp.png" 
   Clicked="addNewItem_button_Clicked"/>
```

A button has three main properties that need to be set in order to implement a functionality:
- an ID (using the Name property), just like all other elements;
- either a name or an icon, so the user understand what does the button do;
- a [clicked event handler](https://developer.xamarin.com/api/type/Xamarin.Forms.Button/) which is a method implemented in the back-end which will be disscused in the Back-end part of this course.


## Icons
Though are not a specific element used in Xamarin Forms mobile development, icons are used (and have been in this course, too) used to give an image to buttons or ListViews and therefore need a mention.
When using Visual Studio, all the elements need to be added in the project - images, too - and as all used icons are present as images those were added on all the drawable dimensions.
The Resource drawable folders are named this way because a version of the icon is needed for all sizes of the mobile devices, there fore the specific icon needs to be included in the proejects files on all mobile platforms, just like below:
<p align="center"><img height="350" alt="Icons" src="https://github.com/microsoft-dx/xamarin-fundamentals-ui/blob/master/Images/android-icons.PNG?raw=true" margin=auto></p>

A great icons website is [material.io](https://material.io/icons/) which also provides icons on various dimensions and file formats.


### Other native elements
Of course, there are more native elements provided by Xamarin Forms but they weren't presented in this course as only the elements that were used were detailed. If you want more information about other elements, visit Xamarin Forms' [official page](https://developer.xamarin.com/guides/xamarin-forms/user-interface/controls/).
