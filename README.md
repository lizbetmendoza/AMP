# AMP - Accelerated Mobile Pages 

AMP, is an open-source website publishing technology designed to improve the performance of web content and advertisements.
Also, allows you to create pages that load quickly. Combining speed and smoother loading,
AMP landing pages often give people much better landing page experiences. 
Landing page experience is an important factor for your Quality Score and Ad Rank.

Here is an example of "amp-story" component, each page have different layers and different templates(layouts), audio, video, JSON file, and external links.

#Page - Cover,
      <amp-story-page id="cover">
          <amp-story-grid-layer template="fill">
              <amp-img src="assets/cover.jpg"
                width="720" height="1280"
                layout="responsive">
              </amp-img>
          </amp-story-grid-layer>
          <amp-story-grid-layer template="vertical">
            <h1>About of Art</h1>
            <p>amp-story</p>
          </amp-story-grid-layer>
        </amp-story-page>
        
 The page display something like this: 
      https://i.imgur.com/Fdbrk4M.png

#Page1 - the template for this page changed to template="vertical" and display in this page an image and text in a single layer 
      https://imgur.com/lBJxPyd
      
#page3 - added song whit this new attribute, just for this specific page
        <amp-story-page id="page3" background-audio="https://www.bird-sounds.net/sounds/alder-flycatcher.mp3">
        https://imgur.com/ZmCNe2I
        
#page4 - add video component (youtube) with some controls to play, pause
          <amp-youtube
               data-videoid="Fg-yNMXLWFo"
               width="720" height="1280"
               layout="responsive">
           </amp-youtube>
           https://imgur.com/jUmGTOv
           
#page5 -  Applying animation to elements inside a page.
           ...
           animate-in="fade-in"
           animate-in-delay="0.4s">
           https://imgur.com/3Dmp7r0
     
#page6 - Adding bookend wraps the up the story and allows you to provide social sharing and related links to your story.
         The JSON file, is used to to show information from this file, add "bookend-config-src" attribute like this:
          <amp-story standalone
             bookend-config-src="bookend.json">
         https://imgur.com/RDcwUgH
           
