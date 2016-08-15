# TextHighlighter 

TextHighlighter is simple android API for developers to show highlighted text in android apps.

##Description:

The purpose of TextHighlighter API is provide the simplest way to highlight the text in android apps.
The API can be used with all andriod views which allows the rendering of text using ```Html.fromHtml()``` method.

##Usage

Add below line in app ```build.gradle```

 
```gradle
dependencies {
	compile 'com.akshay.texthighlighter:texthighlighterapi:1.0.0'
}
```

##Code snippets

Create the object of TextHighlighter

```TextHighlighter highlighter=new TextHighlighter();```

Set the color for specific word

```
highlighter.setColorForTheToken("Awesome","red");
highlighter.setColorForTheToken("Text","purple");
highlighter.setColorForTheToken("Highlighter","blue");
```

Call the method ```getHighlightedText(String textToBeHighlighted)``` and pass the text to be highlighted

```
String highlightedText=highlighter.getHighlightedText("Awesome Text Highlighter");
```

Pass the returned string to ```Html.fromHtml()``` to get highlighted text

``` textViewobj.setText(Html.fromHtml(highlightedText)); ```

you can add your own tags by appending tags inside ```setText()``` 

##More you can get.

Get the color for specific word

```getColorForTheToken(String token)```

Set the default color if no color is specified

``` highlighter.defaultColor="colorname" ```

##Screenshot


![alt tag](https://raw.githubusercontent.com/akshay-naik/TextHighlighter/master/ScreenShot.png)



##License

Copyright 2016 AKSHAY NAIK

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.




