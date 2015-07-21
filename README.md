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
When initialize a text input with delimit(), if not has some **Data Options** stabilized, this input (text or textarea) will have all keyboard keys disabled by default. Think that this plugin runs backwards. The idea is that the Keyboard Keys, will be activated.

This plugin allow to prevent that **copied characters** can be inserted too.


Data Options (Attributes)
-------------

You can set the options easily as data attributes. The initial value always be **false** as default value. The attributes are:

E/D = Enable/Disable

- **all**: All keyboard keys are Enabled. Discard any possible option.
- **numbers**: Allow to use numbers ( 0-9 ) in the input.
- **number**: Allow to use 'Number' sign (#) in the input.
- **dot**: Allow to use 'dot' (.) in the input.
- **less**: Allow to use 'hyphen or less' sign (-) in the input.
- **plus**: Allow to use 'plus' sign (+) in the input.
- **asterisk**: Allow to use 'asterisk' (*) in the input.
- **letters**: Allow to use letters (a-z and A-Z), without other signs like accents or umlaut.
- **enter**: Allow to use of Enter/Intro key.
- **space**:  Allow to use of Space key.
- **control**:  Allow to use of Control keys.
- **comma**:  Allow to use 'comma' (,) in the input.
- **exclamation**:  Allow to use 'exclamation' signs ( !¡ ) in the input.
- **interrogation**:  Allow to use 'interrogation' signs ( ¿? ) in the input.
- **parenthesis**:  Allow to use 'parenthesis' signs ( () ) in the input.
- **lessMoreThan**:  Allow to use 'Less and More than' signs ( < > ) in the input.
- **brackets**:  Allow to use 'brackets' signs ( [] ) in the input.
- **braces**:  Allow to use 'braces' signs ( {} ) in the input.
- **slash**:  Allow to use 'back slash and slash' signs ( \ / ) in the input.
- **accents**:  Allow to use 'accents' signs ( ` ´ ) in the input. If letters options is set true, can use (áéíóúàèìòù) too.
- **quotes**:  Allow to use 'quotes or double quotes' signs ( ' " ) in the input.
- **percent**:  Allow to use 'percent' sign ( % ) in the input.
- **ampersand**:  Allow to use 'ampersand' sign ( & ) in the input.
- **caret**:  Allow to use 'caret' sign ( ^ ) in the input.
- **underscore**:  Allow to use 'underscore' sign ( _ ) in the input.
- **colon**:  Allow to use 'colon' sign ( : ) in the input.
- **semicolon**:  Allow to use 'semicolon' sign ( ; ) in the input.
- **at**:  Allow to use 'at' sign ( @ ) in the input.
- **equal**:  Allow to use 'equal' sign ( = ) in the input.
- **backSpace**:  Allow to use 'back space' key.
- **verticalBar**:  Allow to use 'vertical bar' sign ( | ) in the input.
- **equivalence**:  Allow to use 'equivalence' sign ( ~ ) in the input.
- **ordinalMF**:  Allow to use 'masculine and feminine ordinal' sign ( º ª ) in the input.
- **umlaut**:  Allow to use 'umlaut' sign ( ¨ ) in the input. If letters options is set true, can use (äëïöü) too.