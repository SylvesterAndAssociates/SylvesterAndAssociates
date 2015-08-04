# www
Main Website for Sylvester and Associates dot com
[![Build Status](https://travis-ci.org/SylvesterAndAssociates/SylvesterAndAssociates.svg)](https://travis-ci.org/SylvesterAndAssociates/SylvesterAndAssociates)

Notes on adding a person:

First place the new headshot in templates/sylvester/images you can see all the headshots on github here:
https://github.com/SylvesterAndAssociates/SylvesterAndAssociates/tree/master/templates/sylvester/images

Second ensure prose.io is ‘authorized’ on github: http://prose.io/

then these links should work:
http://prose.io/#SylvesterAndAssociates/SylvesterAndAssociates/tree/master/en/our-staff
http://prose.io/#SylvesterAndAssociates/SylvesterAndAssociates/tree/master/zh/our-staff

on those pages you can click the ‘new’ button, there is a ‘metadata’ button on the right, staff pages need this metadata:

layout: default
background_url: ../../templates/sylvester/images/background_img_11.jpg

The title should be set to the full name of the person, and the body should have an html img tag for the headshot of the person inside a div with class “staff_img”, for example:

```
<div class=”staff_img”>
 <img border=”0” height=”326” src=”../../templates/sylvester/images/KateWang.jpg” width=”218”/>
</div>
```

 then you place separate paragraphs separated by a line with nothing on it.

 for example here is Annie’s page on github:
 https://github.com/SylvesterAndAssociates/SylvesterAndAssociates/blob/master/en/our-staff/annie-lv.md

 on prose.io:
 http://prose.io/#SylvesterAndAssociates/SylvesterAndAssociates/edit/master/en/our-staff/annie-lv.md

 and our live site:
 http://www.sylvester-associates.com/en/our-staff/annie-lv.html

 alternatively to using prose.io, my usual method is to use my favorite editor (vim) and I just copy any staff member, in this case annie-lv.md and copy it to a new file, in this case kate-wang.md

 Then I alter the file with the new info, copy the same file into the ‘zh’ section, swap out the chinese for the english, and we’re done.

 You can see the sum total of my changes here (called a diff):

 https://github.com/SylvesterAndAssociates/SylvesterAndAssociates/commit/e7bae64c36c3c159b4e417e75a53fee19c15b189
