# accessibility-gherkin

## COMPONENTS

### FORM

GIVEN I am a screen reader user  
WHEN I submit a form with validation errors  
THEN I will be focused on the first form field in error state  
THEN I will hear the label for that form field  
THEN I will hear if the form field is required  
THEN I will hear a description of how to fix the error.

### DIALOG

GIVEN I am a screen reader user  
WHEN I activate a button to call a dialog (the control is NOT a link)  
THEN the keyboard focus goes to the active dialog  
AND I hear the screen reader read the title of the dialog  
(AND the button in default focus, if applicable)  
AND I cannot escape the dialog with the tab key  
AND I can escape the dialog with the escape key  
AND WHEN I close the dialog, the focus goes back to the original button  
(OR to the most appropriate place, if the button is not appropriate)

### TABPANEL

GIVEN I am a screen reader user  
WHEN I navigate to a tabpanel widget with the tab key, the focus should land on the active tab.  
WHEN I hit tab again, the focus should go past the remaining tabs to the next focusable item (beyond the tablist).  
IF I need to navigate within the tabs, when the keyboard focus is on the active tab, I can use the right arrow key to go forward through the tabs, or the left arrow key to go backward through tabs.

GIVEN I am a screen reader user  
WHEN I land on the active tab using the tab key, the screen reader reads the label for the tab, it says "tab," it says how many tabs are in the group,  
AND which tab it is (e.g. "tab 1 of 4")  
AND it says "selected." When I navigate with the arrow keys to other tabs, it says all of the above plus gives the accurate location (e.g. "tab 2 of 4").

### AJAX

GIVEN I am a screen reader user  
WHEN I click a button with that executes an ajax request  
THEN IF the request response is slow I will hear that content is loading before the request is complete  
THEN I will hear a message that content has been loaded after the request is complete  
AND I will see focus visual change  
AND I will hear the new content added to the page  

### YOUTUBE

GIVEN I am a screen reader user  
WHEN I navigate to the iframe with my keyboard  
THEN I will hear 'YouTube video player'  
AND I will be able to navigate the iframe content  

## ELEMENTS

### ANCHORS

GIVEN I am a screen reader user  
WHEN I navigate to an anchor with the tab key  
THEN I hear the anchor text read aloud  
AND I will hear element identified as an anchor  
AND the helper text provides an indication of the content of the linked to location

GIVEN I am a keyboard user  
WHEN I navigate to an anchor with the tab key  
THEN I will see focus visual change

### BUTTONS

GIVEN I am a screen reader user  
WHEN I navigate to a button with the tab key  
THEN I will hear element identified as a button  
AND the helper text provides an indication of the action that will be taken

GIVEN I am a keyboard user  
WHEN I navigate to a button with the tab key  
THEN I will see focus visual change

### LABELS

GIVEN I am a screen reader user  
WHEN I select a form element label using the keyboard  
THEN I will hear the label read aloud

### LEGENDS

GIVEN I am a screen reader user  
WHEN I navigate to a legend with the keyboard  
THEN I hear the legend text read aloud

### LISTS

GIVEN I am a screen reader user  
WHEN I select the list using the keyboard  
THEN I hear element identified as a list  
AND I will hear the number of items in the list

GIVEN I am a screen reader user  
WHEN navigate the list with my keyboard arrow keys  
THEN I will hear the next item read aloud

GIVEN I am a screen reader user  
WHEN navigate the past the last item in a list with the keyboard arrow key  
THEN I will hear that I have come to the end of the list

### CHECKBOXES

GIVEN I am a screen reader user  
WHEN I navigate to a checkbox with the tab key  
THEN I will hear the element identified as a checkbox  
AND I will hear the label read aloud  
AND I will hear if it is selected

GIVEN I am a screen reader user  
WHEN I select a checkbox using the keyboard  
THEN I will hear the element be selected  
AND I will hear the label read aloud  
AND I will hear if it is selected

GIVEN I am a keyboard user  
WHEN I navigate to a checkbox with the tab key  
THEN I will see focus visual change

### RADIO BUTTONS

GIVEN I am a screen reader user  
WHEN I navigate to a radio button with the tab key  
THEN I will hear the element identified as a radio button  
AND I will hear the label read aloud  
AND I will hear if it is selected

GIVEN I am a screen reader user  
WHEN I select a radio button using the keyboard  
THEN I will hear the element be selected  
AND I will hear the label read aloud  
AND I will hear if it is selected

GIVEN I am a keyboard user  
WHEN I navigate to a radio button with the tab key  
THEN I will see focus visual change

### TEXT INPUTS

GIVEN I am a screen reader user  
WHEN I navigate to a text input with the tab key  
THEN I will hear the element identified as an input  
AND I will hear the label read aloud  
AND I will hear any defined value  
AND I will hear any defined placeholder text  
AND I will hear if the field is required

GIVEN I am a keyboard user  
WHEN I navigate to a text input with the tab key  
THEN I will see focus visual change

### TEXTAREAS

GIVEN I am a screen reader user  
WHEN I navigate to a textarea with the tab key  
THEN I will hear the element identified as an input  
AND I will hear the label read aloud  
AND I will hear any defined value  
AND I will hear any defined placeholder text  
AND I will hear if the field is required

GIVEN I am a keyboard user  
WHEN I navigate to a textarea with the tab key  
THEN I will see focus visual change

### SELECT MENUS

GIVEN I am a screen reader user  
WHEN I navigate to a dropdown menu with the tab key  
THEN I will hear the element identified as an dropdown menu  
AND I will hear the label read aloud  
AND I will hear any defined value  
AND I will hear any defined placeholder text  
AND I will hear if the field is required

GIVEN I am a screen reader user  
WHEN I open the dropdown menu with the spacebar key  
THEN I will hear the number of options  
AND I will hear selected option

GIVEN I am a screen reader user  
WHEN I open the dropdown menu with the spacebar key  
AND I navigate through the options  
THEN I will hear the option label  
AND I will hear a selected indicator if option is selected

GIVEN I am a keyboard user  
WHEN I navigate to a dropdown menu with the tab key  
THEN I will see focus visual change

### TABLES

GIVEN I am a screen reader user  
WHEN I navigate to a table with the tab key  
THEN I will hear table caption  
AND I will hear the number of columns and number of rows

GIVEN I am a screen reader user  
WHEN I navigate from cell to cell using Control + Alt + arrow keys  
THEN I need to hear the table headers

### IMAGES

GIVEN I am a screen reader user  
WHEN an image receives keyboard focus,  
THEN I will hear the destination or function of that image.

GIVEN I am a screen reader user  
WHEN I come across an image that presents useful information,  
THEN I should hear a description that provides equivalent information.

GIVEN I am a screen reader user  
WHEN I come across an image that is decorative or redundant,  
THEN I should not hear anything for that image.

GIVEN I am a screen reader user  
WHEN I come across an image that presents complex information,  
THEN I should hear a detailed description of that image,  
or find a link to a page that presents more information about the image.

### PICTURES

GIVEN I am a screen reader user  
WHEN a picture receives keyboard focus,  
THEN I will hear the destination or function of that picture.

GIVEN I am a screen reader user  
WHEN I come across a picture that presents useful information,  
THEN I should hear a description that provides equivalent information.

GIVEN I am a screen reader user  
WHEN I come across a picture that is decorative or redundant,  
THEN I should not hear anything for that picture.

GIVEN I am a screen reader user  
WHEN I come across a picture that presents complex information,  
THEN I should hear a detailed description of that picture,  
or find a link to a page that presents more information about the picture.
