---
title: "Computational Synthesis Institute"
root: .
venue1: SESYNC
address1: 1 Park Place, Annapolis MD
country: United-States
humandate: Jul 20-22, 2015
humantime: 9:00 am - 5:00 pm
startdate: 2015-07-20
enddate: 2015-07-22
registration: closed
instructor: ["Kelly Hondula", "Philippe Marchand", "Mary Shelley", "Mike Smorul"]
assistant: ["Nick Magliocca"]
contact: mshelley@sesync.org
raw: raw.github.com/sesync-ci/CSI-2015/gh-pages
twitter:
 - csisesync
 - 755481646099492864
etherpad: https://etherpad.mozilla.org/fBqIr3TFrT
---
<!--
    Edit the values in the parameter block above to be appropriate for your bootcamp.
    Please use three-letter month names for the 'humandate' field.
-->

<!--
    This block includes the Eventbrite registration widget if 'eventbrite' has been set in the header.
-->


<h2>General Information</h2>

<p>
This year's CSI will provide our postdocs and graduate theme participants with hands-on instruction in
open source tools for collaborative coding and data management, analysis, visualization, and dissemination
with a focus on using SESYNC infrastructure. The goals of the workshop are to learn new skills, advance
work on team projects, and get familiar with our CI.
</p>

<p>Updates will be posted to this website as they become available.</p>

<!-- This block displays the instructors' names if they are available. -->
{% if page.instructor %}
<p>
  <strong>Instructors:</strong>
  {{page.instructor | join: ', ' }}
</p>
<p>
  <strong>Assistants:</strong>
  {{page.assistant | join: ', ' }}
{% endif %}

<!--
    Modify this block to reflect the target audience for your bootcamp.
    In particular, if it is only open to people from a particular institution,
    or if specialized prerequisite knowledge is required, please mention that.
-->


<!--
    This block displays the address and links to a map showing directions.
-->
{% if page.latlng %}
<p>
  <strong>Where:</strong>
  
<!--  {{ page.address }}. -->
</p>
{% endif %}

<!--
    Modify the block below if there are any special requirements.
-->
<p>
  <strong>Requirements:</strong>
  Participants must bring a laptop.</strong>
</p>

<!--
    This block automatically inserts a contact email address if one has been specified for the page.
    If one hasn't, this block inserts the generic contact address for Software Carpentry.
-->
{% if page.contact %}
<p>
  <strong>Contact</strong>:
  Please email
  {% if page.contact %}
    <a href='mailto:{{page.contact}}'>{{page.contact}}</a>
  {% else %}
    <a href='mailto:{{site.contact}}'>{{site.contact}}</a>
  {% endif %}
  for questions and information not covered here.
</p>
{% endif %}

{% if page.etherpad %}
<p><strong>Etherpad</strong>: <a href="{{page.etherpad}}">{{page.etherpad}}</a></p>
{% endif %}

<h2>Teaching Materials</h2>

<p><a href="https://github.com/SESYNC-ci/CSI-2015" target="_blank">https://github.com/SESYNC-ci/CSI-2015</a></a></p>

<h2>Acknowledgements &amp; Support</h2>
<div class="pull-right" style="max-width: 320px; padding-left: 6px;">
</div>
<p>
Portions of the instructional materials are adopted from <a href="http://www.datacarpentry.org" target="_blank">Data Carpentry</a> and <a href="http://software-carpentry.org" target="_blank">Software Carpentry</a>.
The structure of the curriculum as well as the teaching style are informed by <a href="http://software-carpentry.org" target="_blank">Software Carpentry</a>.
</p>


<!--
    Edit this block to show the syllabus and schedule for your bootcamp.
-->

<h2>Schedule (tentative)</h2>

<p>We'll have coffee and snack breaks at 10:30am and 3:30pm daily. </p>

<p>SESYNC is providing lunch on site; attendees are responsible for their own breakfast and dinner arrangements (we can make recommendations)

<table class="table table-striped">
  <tr> <td>Monday</td>  <td>9:00am</td>  <td>Welcome and overview of SESYNC CI</td> </tr>
  <tr> <td></td>        <td>9:15</td>   <td>R and how to use RStudio Server</td> </tr>
  <tr> <td></td>        <td>10:30</td>   <td>Break</td> </tr>
  <tr> <td></td>        <td>10:45</td>   <td>Intro to relational databases and SQL (from within R)</td> </tr>
  <tr> <td></td>        <td>12:30pm</td> <td>Lunch</td> </tr>
  <tr> <td></td>        <td>1:30</td>   <td>Intro to git and gitlab and data munging with tidyr and plyr</td> </tr>
  <tr> <td></td>        <td>3:30</td>   <td>Break</td> </tr>
  <tr> <td></td>        <td>4:00</td>   <td>ggplot, wrap up/Q&A</td> </tr>
  <tr> <td></td>        <td>5:00</td>   <td>Reception (informal with snacks, tasty beverages, etc.)</td></tr>
  <tr> <td>Tuesday</td> <td>9:00am</td><td>Tools for disseminating results, code, and data (including R Shiny)</td> </tr>
  <tr> <td></td>        <td>10:30</td> <td>Break</td> </tr>
  <tr> <td></td>        <td>10:45</td> <td>Consulting/hacking</td> </tr>
  <tr> <td></td>        <td>12:30pm</td>  <td>Lunch</td> </tr>
  <tr> <td></td>        <td>1:30</td>  <td>Attendee choice: submitting jobs to the cluster OR geo data with R </td> </tr>
  <tr> <td></td>        <td>3:30</td>  <td>Break</td> </tr>
  <tr> <td></td>        <td>3:45</td>  <td>Consulting/hackng</td> </tr>
  <tr> <td>Wednesday</td> <td>9:00am</td>  <td>Consulting/Hacking/Additional instruction as desired</td> </tr>
</table>

<hr/>

<!--
    Edit the setup instructions in _includes/setup.html to reflect your bootcamp.
    (In particular, most bootcamps teach either Python or R, not both.)
-->


<!--
<h2>Additional Resources</h2>

<h3>shell</h3>
<ul>
<li><a href=http://fosswire.com/post/2007/08/unixlinux-command-cheat-sheet/>Unix/Linux Command Reference</a>
<li><a href=https://github.com/swcarpentry/boot-camps/blob/master/shell/shell_cheatsheet.md
>Shell cheat sheet</a>
<li><a href=http://software-carpentry.org/v4/shell/index.html>Software Carpentry shell lessons</a>
</ul>

<h3>R</h3>

<b>Where to learn more about R</b>
<ul>
<li><a href=http://www.statmethods.net/>http://www.statmethods.net/</a> - good for data organization, basics stats and graphs
<li><a href=http://www.gardenersown.co.uk/Education/Lectures/R/anova.htm>http://www.gardenersown.co.uk/Education/Lectures/R/anova.htm</a> - basic parametric and non-parametric stats
<li><a href=http://www.cyclismo.org/tutorial/R/index.html>http://www.cyclismo.org/tutorial/R/index.html</a> - R tutorial
<li><a href=http://www.amazon.com/R-Action-Robert-Kabacoff/dp/1935182390>R in Action</a> - good book as an R reference
<li><a href=http://www.twotorials.com/>http://www.twotorials.com/</a>
<li><a href=http://www.r-bloggers.com/>http://www.r-bloggers.com/</a>
<li><a href=http://tryr.codeschool.com/>http://tryr.codeschool.com/</a>
<li><a href=http://adv-r.had.co.nz/>Advanced R Programming by Hadley Wickham</a>
<li><a href=http://www.computerworld.com/s/article/9239625/Beginner_s_guide_to_R_Introduction>Beginner's Guide to R from Computer World</a>
<li><a href=http://www.scoop.it/t/r-for-journalists>R for Journalists</a>
<li><a href=http://www.r-bloggers.com/>R Bloggers</a>
<li><a href=http://www.inside-r.org/>inside-R</a> 
<li><a href=http://ropensci.org/>rOpenSci</a>
</ul>

<p>
<b>Plotting in R</b>
<ul>
<li><a href=http://www.harding.edu/fmccown/r/>http://www.harding.edu/fmccown/r/</a> - Very simple graphs
<li><a href=https://storify.com/tracykteal/r-galleries>A variety of R gallery recommendations</a>
<li><a href=http://docs.ggplot2.org/>ggplot gallery</a> - extensive and comprehensive; a great resource
<li><a href=http://www.amazon.com/R-Graphics-Cookbook-Winston-Chang-ebook/dp/B00AJ5X7W4/>R Graphics Cookbook</a> - highly recommended
<li><a href=http://www.cookbook-r.com/Graphs/>Some of R Graphics Cookbook plots</a> - a set of some of the plots from the R Graphics Cookbook by Winston Chang
<li><a href=http://rgm3.lab.nig.ac.jp/RGM/R_image_list?page=665&init=true>R Graphical Manual</a> - plots from apparently every R CRAN package
</ul>
-->

<!---
<h2>Setup</h2>

<p>
  To participate, you will need working copies of the software described below.  Please make sure to install everything <em>before</em> the start of your bootcamp.
</p>

{% comment %}
{% include setup.html %}
{% endcomment %}
--->

