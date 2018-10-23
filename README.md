# Flip-page
supported tag for Text formatting in Page flip

-2. `<Audio></Audio>` attributes are as below
 
     * `position` = '%top,%left,%width,%height' `0<=top,left,width,hight<=100`
     * `border` = `{none|dots|line}`
     * `bg-color` = backgroud color of the whole area -> `VALID COLOR CODE`
     * `bg-res` = background resource to drown
     * `res` = audio clip file uri

-1. `<Video></Video>` attributes are as below

     * `position` = '%top,%left,%width,%height' `0<=top,left,width,hight<=100`
     * `border` = `{none|dots|line}`
     * `bg-color` = backgroud color of the whole area -> `VALID COLOR CODE`
     * `bg-res` = background resource to drown
     * `res` = audio clip file uri

0. `<Text></Text>` **Text** tag
      * `font-name`= `{}`
      * `border` = `{none|dots|line}`
      * `bg-color` = backgroud color of the whole area -> `VALID COLOR CODE`
      * `position` = '%top,%left,%width,%height' `0<=top,left,width,hight<=100`
      * `text-color` = TEXT color of the whole text -> `VALID COLOR CODE`
      * `angle` = rotate clock wise angle `0-180`
      * `highlightTextOnAudio` =  high light the text if player is playing audio {`true`|`false`}
      * `action-enable` = make action tag valid only if value is `true` {`true`|`false`}

1. `<p></p>` for **Paragraph**  attributes are below (nested to <Text> tag)
    * `pg-sp` = paragraph Spacing
    * `ls` = line spacing
    * `hi` = head indent
    * `li` = line indent

2. `<ac></ac>` **Action** on tap (nested to <Text> tag)
     * `audio-time` = millis
     * `video-clip` = 'resource identifier'
     * `popup` = 'resource identifier'

3. `<b></b>` **Bold word** (nested to <Text> tag)

4. `<i></i>` **Italic word** (nested to <Text> tag)

5.  `<sh></sh>` **Shadow color for text** (nested to <Text> tag)
    * `c`= color

6. `<bg></bg>` set **Label back ground color for text** (nested to <Text> tag)
    * `c` = color



Implementation :

  1. use interpreter design pattern to extract and validate text in this format
  
  TODO make this documents more generic , include provision for image and video. 
  
  video add on will be added on 5 iteration but needs to be consider and think
  
  Today's todo : 
  
     i. Create task in project as below 
         a. create a model library which contains all the model classes
         b. Create a interpreter model which reads sample json and puts the value in mdoels
         c. create/modify the existing json to fit the modified requirements
  
  
  
