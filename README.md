# jquery-keyboard-delimiter
This plugin remove the possibility of pressing any key or group of keys defined previously.

You can use this plugin to delimite the writing on inputs, for example:
- Only numbers.
- Numbers with signs.
- Text without numbers.
- Common keys as ESC, CTRL, etc.

How to use keyboard-delimiter.
-------------
Include keyboard-delimiter & jquery to your Site
  ```
  <script src="http://code.jquery.com/jquery-1.10.2.min.js"></script>
  <script src="js/jquery-keyboard-delimiter.min.js"></script>
  ```
Add a input type text on your html document
```
<input type="text" class="only-numbers" placeholder="Write here.." >
```

And then, add a similar code in your site:
```
<script type="text/javascript">
  $(document).ready(function(){
    $(".only-numbers").delimit({
      numbers: true
    });
  });
</script>
```

Important Note
-------------
When initialize a text input with delimit(), if not has some **Data Options** stabilized, this text input will have all keyboard keys disabled by default. Think that this plugin runs backwards. The idea is that the Keyboard Keys, will be activated.

This plugin allow to prevent that **copied characters** can be inserted too.


Data Options (Attributes)
-------------

You can set the options easily as data attributes. The initial value always be **false** as default value. The attributes are:

E/D = Enable/Disable

- **all**: All keyboard keys are Enabled. Discard any possible option.
- **numbers**: E/D the input for accept only numbers.
- **dot**: E/D use 'dot' (.) in the input.
- **hyphen**: E/D use 'hyphen' sign (-) in the input.
- **plus**: E/D use 'plus' sign (+) in the input.
- **asterisk**: E/D use 'asterisk' (*) in the input.
-	**divide**: E/D use 'divide' (/) in the input.
-	**letters**: E/D write only letters, without numbers.
-	**escape**: E/D the use of Escape key.
- **enter**: E/D the use of Enter/Intro key.
- **space**:  E/D the use of Space key.
- **control**:  E/D the use of Control keys.
