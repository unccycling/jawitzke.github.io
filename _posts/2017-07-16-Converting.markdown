---
layout: post
title:  "Converting Documents"
subtitle: "Writing Script to Convert Documents from Makrdown to Other Formats"
date:   2017-07-05 23:34:01
categories: [Computers]
---

___

## Learning to Script!

Hello all, the written work that I added to my repository is a short story that I had written for English 121 that was suppose to be in a  
similar style to that of Charles Dickens. It is a pretty sad story about a man named Mr. Hobson that has had a pretty rought time recently.  
The story is a tad bit based off of true events. A good friend of mine, David "Dobs" Hobson, committe suicide fairley similarily to that  
in the story. He however, was in high school. Anyways I hope you all enjoyed the [story](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.md).  


In order to get the convert the documents in mulitple formats I used pandoc and texlive. I created two variables. $INPUT which is the file
that the user puts in, and $OUTPUT which is the input file name just without the .md. 
{% highlight javascript %} INPUT=$1
OUTPUT=$(echo -n $INPUT | head -c -3) {% endhighlight %}

Then for the file types HTML, DOCX, and ODT I used the pandoc and echo commands such that:
{% highlight javascript %} pandoc -o $OUTPUT.html $INPUT
echo "Created new file in HTML format called $OUTPUT.html"{% endhighlight %}

And for PDF I had to use texlive and pandoc such that:
{% highlight javascript %} pandoc $INPUT --latex-engine=pdflatex -o $OUTPUT.pdf
echo "Created new file in PDF fromat called $OUTPUT.pdf" {% endhighlight %}

Lastly, for RTF I used pandoc such that:
{% highlight javascript %} pandoc -s $INPUT -o $OUTPUT.rtf
echo "Created new file in RTF format called $OUTPUT.rtf" {% endhighlight %}

My resource are the follow:
1. [Script](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/jawitzke-convert-docs.sh)
2. [Input file](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.md)
3. [Output file in HTML](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.html)
4. [Output file in DOCX](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.docx)
5. [Output file in ODT](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.odt)
6. [Output file in PDF](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.pdf)
7. [Output file in RTF](https://github.com/jawitzke/jawitzke-convert-documents/blob/master/story.rtf)
8. [General Repository](https://github.com/jawitzke/jawitzke-convert-documents)






<div>
	  <p>
     <script>
						var week_days = new Array(8);
								week_days[1] = "Sunday";
								week_days[2] = "Monday";
								week_days[3] = "Tuesday";
								week_days[4] = "Wednesday";
								week_days[5] = "Thursday";
								week_days[6] = "Friday";
								week_days[7] = "Saturday";
								
						var month_array = new Array(13);
								month_array[1] = "January";
								month_array[2] = "February";
								month_array[3] = "March";
								month_array[4] = "April";
								month_array[5] = "May";
								month_array[6] = "June";
								month_array[7] = "July";
								month_array[8] = "August";
								month_array[9] = "September";
								month_array[10] = "October";
								month_array[11] = "November";
								month_array[12] = "December";
								
						var date_obj = new 	Date(document.lastModified)
						var curr_day = week_days[date_obj.getDay() + 1]
						var curr_month = month_array[date_obj.getMonth() + 1]
						var curr_date = date_obj.getDate()
						var curr_year = date_obj.getYear()	
							if (curr_year < 2000)
								curr_year+=1900
								document.write("Last updated on" + " " + curr_day + ", " 
								+ curr_month + " " + curr_date + " " + curr_year)
					  </script>
           </p>
      </div>
