# Minimal CSS Structure Model

While looking for ways how to order my CSS files consistently, I considered different solutions. The best I found was concentric CSS, pointed out to me by another [webdesigner]. But while it may be a reasonable approach, it never really worked for me, I always had to look up how it is done because it just does not look intuitive to me. Thus I came up with a model on my own. My CSS is ordered based on a model of priorities of minimal webdesign.
  
Assuming that the content is done and the styling begins my first step is to choose colours; this is what I begin with. Just as for a book you would have to choose paper and letters, so I choose the background, fitting font-colors and font-families. 
My understanding of minimal webdesign is to begin with the most minimal, bare-bones framework, then address problems as they arise and improve the details in a order of priorities focused on the content.

For colours, a good approach seems to be to define them in a preceeding :root selector, so that they can be referenced by simple terms by which you may be able to easily remember them and which fit to your project. For instance, for our Phoenix design we have the following colours:

```css
:root {
  --black: #000;
  --dark: #121212;
  --light: #dddddd;
  --blood: #844d44;
  --copper: #8c5f4e;
  --demonic: #855f67;
  --gold: #976b42;
  --ore: #4f6766;
  --silver: ...;
}
```

In a minimal approach to styling the main priority is to let the actual text (or images) look good, make it readible and give it room. For a text focused page, the text has to be styled before thinking about how to position it, including line-height and letter-spacing. When its about a gallery; then the image size and gaps are the most important thing before then coming up with a layout to position them. 

<span class="subtext">For me that is usually flex. Flex is an extremely powerful tool. I never found a need to use grid so far and in comparison to flex it is much more complex and confusing.</span>

The distance of the text to other text and to the border of the page is the next important thing, to give the content room on the background, that means the padding (and the margin as a prior step that is usually 0). 

Now we have to address the content-width, to define the width of the text blocks for better readability. It has to come after, because it has to be chosen based on the font and font-size chosen before. I usually go for something between 500-700px max-width. Based on this scheme, the CSS is structured as follows:

```css
main {
  background: var(--dark);
  color: var(--light);
  font-family: Helvetica, Arial, sans-serif;
  font-size: 16px;
  line-height: ;

  margin: 0;
  padding: 2em;

  max-width: 600px;
}
```

After this general content styling my next priority is to dive into the different text elements. I am now styling headings, paragraphs, lists and links. I may want to make the first heading bigger or put all third headings into a box or whatever. 


At this point the website is already fully functional. 
It looks nice, it is automatically "responsive", it looks good on all devices, it's simple and it works. Everything that comes now has to serve a very specific purpose like solving a specific content-related problem or add a required feature. 


