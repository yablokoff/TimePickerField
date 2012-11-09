Time Picker Field
=======

Currently, there is no `TimePickerField` for Sencha Touch 2.0. This class
solves that problem.

## INSTALL

Just include the file in your MVC-structured Sencha Touch project.

## USAGE

This field is easy to use. The `xtype` is `timepickerfield`, so you can use it
in your form like so:

```javascript
Ext.onReady(function () {
    Ext.create("Ext.Panel", {
        fullscreen: true,
        
        items: [{
            xtype: "formpanel",

            items: [{
                xtype: "timepickerfield",
                name: "time",
                label: "Time",
                startTime: 600,
                endTime: 2300,
                increment: 30,
                value: "2:00 PM"
            }]
        }]
    });
});
```

Note that `TimePickerField` extends `Ext.field.Text`; mandatory properties
still apply. Optional values for `TimePickerField` are `startTime`, `endTime`,
and `increment`. The defaults are `600`, `2200`, and `15`, respectively.
