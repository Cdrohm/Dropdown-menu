# Dropdown-menu
 
This is a a selection menu containing options to select. It can take a placeholder, return a value, and can be reset to the default state after the form is filled out and submitted.

------------


## Installation
npm i plugin-dropdown-menu-select

------------


## Explanation / Usage
### there are 6 arguments included
*1*. **label** (string) - Allows you to display a text at the beginning of the menu (option)

**2**. **options** (array) - The options must be an array (required) 
*2-1* (string) 
-strings are used to display text, the returned value is a lowercase version of the string with white spaces converted to an underscore

*2-2* (object)
-**name**: optionText - displayed text
-**value**: returnedValue - Selected value

**3**. **placeholder** (string) - text displayed when there is no selection (option)

**4**.** log** (boolean) - displays nodeElement and the returned value in the console | true by default (option)

**5**. **setvalue**(function) - setter to return the selection to the parent component

**6**. **initComponent**(object) - initialization of the getter and setter to reset the menu to default (required)
*6-1* **init**(boolean) - action state init by getter
*6-2* **setInit**(function) - set the init action to false by a setter when the menu is returned to the default state

------------


## How to get selected value
you need to set a getter/setter variable using the useState() hook. Then you need to pass it to the setter function at the component.

------------


## CSS
the following *3 classes* allow to change the appearance of the menu:

1)**dropdown-label** - to edit the text label
2)**dropdown-select** - to edit the menu part 
3)**dropdown-option** - to edit each option present in the menu

------------

