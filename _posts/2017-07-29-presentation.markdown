---
layout: post
title:  "Presentation"
subtitle: "HTML Presentation on the Tour de France"
date:   2017-07-29 12:34:01
categories: [Computers]
---

___

In this Assignment I made a presentation we had to create a well-formed presentation for use on scree. I added self-runnning audio embedded within the presentation that I recieved from [here](https://www.youtube.com/watch?v=1v6l1_lfFN0&t=39s). These assignment stregnthed my use of HTML skills while also learning how to create a better presentation than something that is on PowerPoint. 

The [presentation](https://jawitzke.github.io/jawitzke-presentation/) is about 4 minutes longth explaining what the Tour de France is really all about. It goes into detail about the origins, the fans, the different competitions, and the stages. The presentation was made using Reveal.jg which I made a pretty good experience using and I felt quite happy with. I was able to add images, styles, and audio to the slides with ease and it all transitions very nicely, which allows for a wonderful presentation.

I definitely think I will be using Reveal.js for presentations in the future. Overall, I thought the assignment went pretty well, and I am happy with the way that it turned out. The following are the resources for my assignment:
1. [Repository](https://github.com/jawitzke/jawitzke-presentation)
2. [Presentation Code](https://github.com/jawitzke/jawitzke-presentation/blob/master/index.html)


___


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

