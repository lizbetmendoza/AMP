# AMP - Accelerated Mobile Pages 

AMP, is an open-source website publishing technology designed to improve the performance of web content and advertisements.
Also, allows you to create pages that load quickly. Combining speed and smoother loading,
AMP landing pages often give people much better landing page experiences. 
Landing page experience is an important factor for your Quality Score and Ad Rank.

Here is an example of "amp-story" component, each page have different layers and different templates(layouts), audio, video, JSON file, and external links.

### Page - Cover 
The page display something like this:
```
<amp-story-page id="cover">
          <amp-story-grid-layer template="fill">
              <amp-img src="assets/cover.jpg"
                width="720" height="1280"
                layout="responsive">
              </amp-img>
          </amp-story-grid-layer>
          <amp-story-grid-layer template="vertical">
          </amp-story-grid-layer>
        </amp-story-page>
```
![cover](../master/img/page1.jpg)

### Page1 - layout="vertical"
The template for this page changed to template="vertical" and display in this page an image and text in a single layer 

![page1](../master/img/page2.jpg)  

### page3 - background-audio
Added song whit this new attribute, just for this specific page,
```
   <amp-story-page id="page3" background-audio="https://www.bird-sounds.net/sounds/alder-flycatcher.mp3">
```
![page3](../master/img/page3.jpg)  

### page4
Add video component (youtube) with some controls to play, pause... 
 ```
  <amp-youtube
  data-videoid="Fg-yNMXLWFo"
  width="720" height="1280"
  layout="responsive">
   </amp-youtube>
 ```
![page4](../master/img/page4.jpg)       ![page4a](../master/img/page4a.jpg)             
### page5 
Applying animation to elements inside a page. 
 ```
           animate-in="fade-in"
           animate-in-delay="0.4s">
 ```
![page5](../master/img/page5.jpg)  
     
### page6 - bookend
Adding bookend wraps the up the story and allows you to provide social sharing and related links to your story.
The JSON file, is used to to show information from this file, add "bookend-config-src" attribute like this:
 ```
   <amp-story standalone
   bookend-config-src="bookend.json">    
```
![page6](../master/img/page6.jpg)    
           
