# Angular Timepicker Directive

A simple dropdown style timepicker directive.

[Demo](http://www.dnasir.com/github/angular-timepicker/demo.html)

## Prerequisites

1. [Angular 1.2.0+](http://angularjs.org)
2. [Angular UI Bootstrap 0.3.0+](http://angular-ui.github.io/bootstrap/)
3. [Angular DateParser 1.0.0+](https://github.com/dnasir/angular-dateParser)
 
## Usage

Include the timepicker directive file, and attach it to an input field.

    <input type="text" dn-timepicker="h:mm a" min-time="00:00" max-time="23:59" step="15" ng-model="timepicker.model" />
    
## Options

#### dn-timepicker

The format to use when displaying the time in the input box and the dropdown list.

    Default value: 'h:mm a'

<sub>Added: 1.0.5</sub>

#### ng-model (Date)

The model that the timepicker is bound to. If no model is given, it will create a new one.

    Default value: new Date()

<sub>Added: 1.0.0</sub>

#### time-format (string) [DEPRECATED]

The format to use when displaying the time in the input box and the dropdown list.

    Default value: 'h:mm a'

<sub>Added: 1.0.0</sub>

**This attribute is now deprecated. Please specify the time format as value for the directive attribute.**

#### min-time (string)

The lower limit for the list of selectable times. The value must match the format used.

    Default value: '00:00'

<sub>Added: 1.0.0</sub>

#### max-time (string)

The upper limit for the list of selectable time. The value must match the format used.

    Default value: '23:59'

<sub>Added: 1.0.0</sub>

#### step (string)

The amount of time between each item in the list of selectable time. Values are in minutes. Add 'h' after the integer to use hours, i.e. '1h' will be converted to 60 minutes.

    Default value: '15'

<sub>Added: 1.0.0</sub>
