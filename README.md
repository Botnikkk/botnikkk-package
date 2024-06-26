<p align="center">
  <img src="https://raw.githubusercontent.com/Botnikkk/botnikkk-package/main/images/logo.jpg"/>
</p>

# botnikkk  

Under construction! Not ready for use yet! Currently experimenting and planning!

Developed by BotNikkk / Nikkk

# How To Use :

## 1. centre() function

Usage = Centering Elemtents.

```python
import botnikkk

botnikkk.centre('text')
```

It also takes 3 extra parameters as input :

1. symbol : determines what symbol will fill in the blank space, deault parameter = " "

```python
botnikkk.centre('text',symbol='=')
```

2. left_alignment : determines the space that will be used on the left hand side of the centred string, defaul parameter = None/calculated automatically

```python
botnikkk.centre('text', left_alignment=23)
```

3. str_end : determines what symbol will print as end= in print statement, deault parameter = "\n"

```python
botnikkk.centre('text',str_end='end')
```
#### OUTPUT EXAMPLE :

<p align="center">
  <img src="https://github.com/Botnikkk/botnikkk-package/blob/main/images/output_centre.png?raw=true"/>
</p>

## 2. format_input() function

Usage = centering the input variable.

```python
import botnikkk

answer = botnikkk.format_input('input_question')
```

#### OUTPUT EXAMPLE :
<p align="center">
  <img src="https://github.com/Botnikkk/botnikkk-package/blob/main/images/output_input.png?raw=true"/>
</p>

## 3. int_check() function

Usage = checks if an input variable is a interger or not, takes repetetive inputs if not Interger.

```python
import botnikkk

answer = botnikkk.int_check('any_variable')
```

#### OUTPUT EXAMPLE :
<p align="center">
  <img src="https://github.com/Botnikkk/botnikkk-package/blob/main/images/output_int.png?raw=true"/>
</p>

## 4. ans_check() function

Usage = takes a list of strings as input and displays it to the user as centred options, returns the choosen option. 

```python
import botnikkk

answer = botnikkk.ans_check(['list_of_variables'])
```
#### OUTPUT EXAMPLE :
<p align="center">
  <img src="https://github.com/Botnikkk/botnikkk-package/blob/main/images/output_ans.png?raw=true"/>
</p>

## 5. get_alignments() function

Usage = takes a string as input and returns a dictionary containing the designing alignments of the said string in the form :
```python
dic=  {"left_align":value , "left_gap":value, "right_gap":value, "default_gap":value }
``` 
which can be used to format a string accoring to the alignment format of package in such form :
```python
print_string= left_align*" " + "|" + left_gap*" " + string + right_gap*" " + "|" 
``` 

```python
import botnikkk

alignments = botnikkk.get_alignments("string")
```
#### OUTPUT EXAMPLE :
<p align="center">
  <img src="https://github.com/Botnikkk/botnikkk-package/blob/main/images/output_alignment.png?raw=true"/>
</p>

## 6. redirect() function

Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.

```python
import botnikkk
import asyncio

async def function():

    #some code
    await botnikkk.redirect("screen_name")
    #some more code

asyncio.run(function())
```


check out : https://botnikkk.github.io and https://github.com/Botnikkk/botnikkk-package
