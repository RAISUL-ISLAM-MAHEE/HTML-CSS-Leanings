# Media Query - @media
it is used to implement condition on css and is a great tool for creating responsive websites.

## Syntax of Media Query.

@media media-type and (media-feature-rule){
  css codes.....
}

Search "Media Query mdn" for more information about media feature and media types.

Ex:
1. @media screen and (width:600px){
  body{
    color: red;
  }
}

This will change the color of the text to red when the screen width hits exactly 600px.


2. @media screen and (max-width:600px){
  body{
    color: red;
  }
}

This will change the color of the text to red until the screen width hits  600px.


3.@media screen and (min-width:600px){
  body{
    color: red;
  }
}

This will not change the color of the text to red until the screen width hits exactly 600px.

## Operators:

### 1. "and" operator
is used to implement multiple condition and all of them have satisfy the condition for the change to occur.

Ex:
@media screen and (max-width:600px) and (orientation: landscape){
  body{
    color: red;
  }
}

This will change the color of the text to red if it satisfies the screen width is less or equal to 600px and the screen orientation is equal to landscaping.


### 2. "," operator
 is used to implement or condition. This means we set multiple conditions and if one of them satisfies then the change will occur.

Ex:
@media screen and (max-width:600px),
screen and (orientation: landscape){
  body{
    color: red;
  }
}

This will change the color of the text to red if the screen width is less or equal to 600px or the orientation is landscape.


### 3."not" operator
is used to restrict change till it satisfies the conditions.
When the conditions are not satisfied the changes will occur.

Ex:
@media not screen and (orientation: landscape)
{
  body{
    color: red;
  }
}

This will not change the color of the text to red till the screen orientation is landscape.
