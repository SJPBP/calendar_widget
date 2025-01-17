# Calendar Widget for use with python tkinter

<img align="left" src="https://github.com/Spartanlasergun/calendar_widget/blob/main/README_info/Calendar%20-%20Light%20Theme.png?raw=true">
<img align="right" src="https://github.com/Spartanlasergun/calendar_widget/blob/main/README_info/Calendar%20-%20Dark%20Theme.png?raw=true">

------

------

------

------

------

------

------

------

------

------

# Installation

##### Install the calendar widget using the following commands
```
pip install calendar_widget
```

# USAGE

#### First, Import the calendar widget along with tkinter
```
import tkinter
from calendar_widget import Calendar
```

##### Define the tkinter window into which the widget will be placed. EXAMPLE:
```
root = tkinter.Tk()
root.geometry('600x600')
```

##### The Calendar Widget can then be created as follows:
```
Calendar = Calendar(root)
```

##### To pass a command to the Calendar, specify the command option when it is created
```
Calendar = Calendar(root, command=user_command, ...)
```

##### To retrieve a selected date on the calendar, use the get_date command:
```
Calender.get_date()
```

##### To create a checkbox on the calendar, the command is as follows:
```
checkbox = Calendar.checkboxes(10, 10, 2022, status=True, ...)

#to remove a chcekbox that has already been created specify the delete option as follows:

Calendar.checkboxes(10, 10, 2022, delete=True)
```

##### To destroy the calendar widget, call the destroy method:
```
Calendar.destroy()
```


The table below specifies opitons availiable for styling and other operations associated with the calendar widget

| options | description |
| ------- | ----------- |
| size= | Sets the width of the widget in pixels. The default/minimum width is 300px. |
| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
| command= | A function to be called when the widget is clicked. |
| background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
| calendar_relief= | Sets the relief of the Calendar widget. |
| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months |
| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months |
| date_box_border= | Sets the colour of the border associated with the monthly calendar grid. |
| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. |
| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. |
| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. |
| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. |
| arrow_fill= | Sets the colour of the calendar arrows. |
| arrow_thickness= | Sets the thickness of the calendar arrows. |
| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. |
| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. |
| weekday_width= | Sets the width of the boxes that hold the weekday headings. |
| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. |
| weekday_font_family= | Sets the type of font used to create the weekday headings. |
| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020) |
| date_heading_font_family= | Sets the font type for the Calendar date heading. |
| date_text_fill= | Sets the colour of the text numbers associated with the month dates. |
| date_text_font_family= | Sets the font type used to create the month dates. |
| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. |
| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. |
| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. |
| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. |
| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. |
| user_highlight_text= | Sets the colour of the text associated with the user highlight. |

