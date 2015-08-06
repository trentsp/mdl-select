# mdl-select

MDL-Select provides a javascript/jquery based function to include a <select>...<option></option>...</select> in Google's Material Design Lite (http://www.getmdl.io/).

# Dependencies
- JQuery
- Material Design Lite

# Usage
```javascript
  $("#select").mdlselect({
    value: ["0", "1", "2", "3"],
    label: ["n/a", "Option 1", "Option 2", "Option 2"],
    fixedHeight: '10em'
  });
```
```html
  <html>
  <body>
    <div id="select-container" class="mdl-textfield mdl-js-textfield mdl-textfield--floating-label">
      <input class="mdl-textfield__input" type="text" id="select" name="select" readonly />
      <label class="mdl-textfield__label" for="select">Select your option</label>
    </div>
  </body>
  </html>
```
# What happens
When the user selects an option, the value is placed in a hidden input. The name/id of the input is: "nameofthefieldfunctionisattachedto"_hidden. In the example above, the hidden input would have an id/name of "select_hidden".
