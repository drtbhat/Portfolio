## Assignment 2

In this assignment I have re-designed the following visualization:

<img width="905" alt="Screen Shot 2023-02-07 at 11 51 51 PM" src="https://user-images.githubusercontent.com/123350491/217436842-1cce29ed-561c-49f8-9b3d-70c2cb07a679.png">

The image is taken from NBC News website. 
Source URL: https://www.nbcnews.com/data-graphics/covid-hospitalizations-see-latest-trend-current-count-rcna61053

The context of the graph is the most recent/ongoing COVID wave. The story was published on feb 3, 2023 and the data for the visualization was last updated on Feb 7th. 

Although the graph looks visually pleasing because of the soothing color hues, it does not draw the audience in. The flat title, the confusing legend sign, the similar shades of colour hiding the minor differences among states and the lack of a story highlight are some factors that could be improved upon to make the visualization more effective. However, the graph is reliable and truthful to the data. 

### Redesign 1

Since the main news story is about overall changes in hospitalizations in the country, I decided to capture that in a pie chart. I divided the pie in states that have witnessed increased percentage of hospitalizations in the last 14 days and states that have witnessed decreased percentage of hospitalizations in the last 14 days. 

![image](https://user-images.githubusercontent.com/123350491/217443702-962c9101-588e-4ce4-8c38-e0c5c19dbdf5.png)

I decided to highlight the smaller pie, the portion of states with increasing percentage of hospitalizations. This is an overall positive story since most states have decreasing percentage of hospitalizations. 

However, I felt that this graph was not very interesting, particularly because it did not personalize the story to for any audience segment. It just showed a general picture. 

### Redesign 2

To make the visualization interesting I decided to filter out the states and showcase the states with the highest percentages increases in hospitalizations. 

![image](https://user-images.githubusercontent.com/123350491/217444736-35b762e3-cde4-4ad2-a238-a5cb50223fd6.png)

In total, there were 6 states where hospitalization percentages were increasing in the previous 14 days. I created a horizontal bar graph for all of these states and chose to focus on the fact that Alaska has the highest rise in percentage of hospitalizations. The X-axis shows the percentage increase in hospitalizations in the previous 14 days and the Y axis shows the state names. The colour gradient and sorting based on hospitalization percentages highlights the story I am tring to tell. 

### User Research on Redesign 2

I conducted user research with two of my batchmates, one male and one female from the MSPPM program. I asked them the from the question prompts as listed in the assignment. 

1. I have mentioned nothing about COVID in the title, so both the respondents were able to guage that the graph shows hospitalizations but missed that this was amidst the latest COVID wave.
2. Both the respondents were able to correctly and quickly tell the main idea of the story, that is hospitalization is increasing most in Alaska out of the six states shows. 
3. Both the respondents were international students and found the state abbreviations confusing at first. MSPPM male respondent also found hospitalization percentage as a confusing measure. This is when I also realized that I had mentioned nothing about the 14-day increase in the graph. When I explained to him the interpretaion of hospitalization percentage, I realized that the measure of percenatge had a flaw, in the sense that if the intial hospitalizations was a small number, even a minor rise in hospitalization would show a huge percentage increase. 
4. The MSPPM female felt that the intended audience for this graph was anyone who lived in the states shown in the graph. MSPPM male respondent felt that the intended audeince was US citizens. 

### Redesign 3

After incorporating feedback from the user research, I came up with this sketch.

![image](https://user-images.githubusercontent.com/123350491/217450810-844fea9d-b994-42fb-a212-f4c65928cdfe.png)

I changed the value studied from percentage of hospitalization to hospitalizations per 100,000 residents. I also added COVID in the title and retained the chart type, the sorting and the colour gradient. 

### Redesign 3 in Tableau


<div class='tableauPlaceholder' id='viz1675831471265' style='position: relative'><noscript><a href='#'><img alt='Delaware has highest hospitalizations per 100,000 residents ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TS&#47;TSWD-COVIDhospitalization&#47;Sheet2&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TSWD-COVIDhospitalization&#47;Sheet2' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;TS&#47;TSWD-COVIDhospitalization&#47;Sheet2&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
var divElement = document.getElementById('viz1675831471265');                    
var vizElement = divElement.getElementsByTagName('object')[0];                    
vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
var scriptElement = document.createElement('script');                    
scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

The X axis of this horizontal bar chart shows hospitalization per 100,000 residents and Y axes shows state names and percentage change in hospitaltion in the last 14 days. 

In Tableau, I started with a simple horizontal bar graph with sum of hospitalizations per 100,000 residents in caloum and places as row. First I went to the data source to change the column title places to states to make it less confusing. Next, I filtered the rows on the basis of the hospitalizations attribute, selecting the range of values I wanted to show in the graph. Next, I dragged the hospitalizations per 100,000 in the colour section of the toolbar. Then I marked the bars such that the number of hospitalizations value is shown at the end of each bar. To avoid redundancy, I removed the hospitalization values from the x axis. Later, as I was just playing with graph, I added the attribute of 14 day percentage change in hospitalizations and it added to the graph. I thought this information was valuable when the whole number of hospitalizations was also mentioned. Also, staying true to the original source and context, as a news organization, NBC wanted to show the latest development and trends in hospitalization. The percentage value added to the row in the Tableau graph responded to this. I went to data source to edit the column title to make it less confusing. After this I changed the title of the graph, made it bold and bigger to establish the visual hierarchy. I tried to remove the faint grid lines from the graph background but was unable to do so. 

[Back to main page](README.md)
