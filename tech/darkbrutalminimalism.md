# dark brutal minimalism

WIP

In webdesign there are different trends or design schools you could say. Among them there is minimal design, material design, brutalist design and so on.

And while those designs differ in some aspects, they have others in common that are considered as good practice by all of them. And of course you can mix the styles. For instance, there are pages that are primarily brutalist with minimalist influence. Or pages that are minimal with material design influence.

My own style I want to describe as dark brutal minimalism.

Some principles (some shared with common webdesign practice, some of my own):
* content needs room to shine.
* rules of layering of attention (bigger fonts for text that should be seen first; how to name that?)
* big bold text if a written message is essential to convey
* no text or very little, unobtrusive text if an image is the essential message
* divide the page conceptually into thematic blocks (header, navi, main, footer, but also sections of main like "latest article", "latest artwork", "article list", "artwork category one", "artwork category two". 
* Instead of thinking too much about the website as a whole and how to FIT content INTO the design you imagine, put the Content FIRST and think how to present this specific content the best, to THEN let it become a part of the design as a whole. For example, you have a gallery, but the images belong to different contexts, as in my case: Some are acrobatic related, some webdesign, some gamedesign, some fashion etc., when these would be a list in html, they would be ordered into categories with respective headers; think and implement them on these lines, then look at each of those; the acro pictures may be cooler to present in another way than the webdesign etc.
* minimalism doesn't mean that there has to be big gaps between every image, between every text and image etc.; but there have to be such gaps between thematic SECTIONS.


## Dark brutal minimalism

So. How to go about designing a brutal minimalist website? 

I will try to answer this question by doing just that: Designing such a website for myself. I wanted to redesign my personal website and I wanted to write an article about my thoughts on webdesign; this way I can do both.  

**Why do I want to design a website?** or **What is going to be in there?** 
For every project and every person these questions should be answered differently and this will influence everything from then on. My reply was: *I want to have an online presence to present some of the things that I do, that I love and that I think, in form of images (acrobatics, design) and in form of text (essays).*

Presenting those things in form of images and text requires that such images and texts exist. Designing a website with placeholder content is like making cloth without knowing the wearer. It isn't tailored and therefore it will not fit, simple as that. 

You may say that it's nice on its own; I say it is only as nice as its brought to life by wearing it, fitting the individual body and movement.

Thus: Content first. Content shapes design; design does not shape content. 

We assume that content has been made (text written, photographies taken and so on). Both have to end up in html, the structure of the website. This structure has to be solid and it has to abide to the rules; otherwise it will fall apart. Maybe not for you, but for people on text browsers or for screen-readers for instance.

The structure of every website consists of specific html tags within which the content will be. This is the structure:

```
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```

Now we title the website: What is it about? 
In my case it is about me. So I title it Flosha, like this:

```
 <head>
   <title>Flosha</title>
 </head>
 ```

Now: Do I have to introduce the visitor to the websites topic? Not necessarily. On a news page, the visitor doesn't have to be informed that he is on a news page because he's seeing news presented everywhere. In such cases, the content speaks for itself. But every website is a presentation and in this case it is a *personal* presentation. It is not about an organisation or a project, it is about what I personally love, do and think - at least the part of it I want to share and present.

While in many other cases it may be perfectly viable to approach it anonymously, there is no sense in doing so, when an essential part of the website deals with a performing art (acrobatics). Nonetheless I see no reason to show more of myself than I need to serve the purpose of the presentation. But in any way: When someone comes to my personal presentation, I think I should at least introduce myself.

I try to keep the introduction short and only say what I think is most important in the context of the presentation. In a live presentation people could now connect with me, could suggest cooperation, ask questions, invite me somewhere; but on a website we require some other form of contact possibility. I see no reason to put that on a subpage, when I can just as well make contact accessible more directly. So it will be part of the introduction, the first section of my html frame. 

```
  <body>
    <header>
    </header>
    <main>
      <section id="intro">
        <p>I'm Flosha, an Acrobat with a 
        focus on mixed pair hand to hand 
        and floor work. I write, design, 
        engage in social work and I'm 
        creative director of PHOENIX.</p>

        <p>Enquiries at floshin@matrix.org</p>
	  </section>
    </main>
  </body>
```

Before adding other content to this structure, I have to answer another question:

**Is the content thematically consistent or does it deal with different themes?**
As I have written above, the website is supposed to present things that I love, do and think; since I love, do and think about different things, the content is *not* thematically consistent (and the only consistent theme is me, in this case).

So I have to identify these different themes. 
In my case, the main themes are acrobatics, design and philosophy, because these are the themes that I am mostly interested in and that I want to deal with on the website in form of the before mentioned images and thoughts.  

Every theme will be a section in the html frame:

```
  <body>
    <section id="acro">
    </section>
    
	<section id="philosophy">
	</section>
	
    <section id="design">
    </section>
  </body>
```




Time to style!
While the content is *what* I present, the style is *how* it is presented and serves as a representation of the project the content deals with or of the organisation or person the content is dealt with by. 

At the beginning for me stands the background and colour choice. 
I use dark themes always. They're easier to read, easier on the eyes and easier on phone battery. And if you want to convey some sort of mystic, dusky atmosphere, it has to be dark anyway.

Pure white on pure black is bad for readability and your eyes. So you either have to lighten the black (baseline `#121212`) or to darken the white (baseline `#dddddd`). You create a lighter background that doesn't contrast with the light so much or you leave it as dark as it is and just "dim the light" or a combination of the two. In the end you just want a contrast that is not too low and not too high. 

Google's Material Design for instance recommends the use of pure white on a dark grey background (baseline `#121212`). 

On other websites I made, like phoenixtales.de or the Gothic Archive I have chosen a pure back background and a reduced the brightness of the font because of how characteristic such pure black backgrounds were for dark webdesigns in the 90s and for the official Gothic Website in particular. But for this design I will use rgba 0 0 0 with 95% transparency or `#0d0d0d`, which results in a dark grey that is a bit darker than the one recommended by Google; therefore my font will not be pure white either. I go for `#ddd`.  

The page is already functional. 






For this, images have to be adapted to the web and text has to be converted to html. 




everything on the main page instead of thousend subpages
-> therefore I see pages as posters that should inform about everything relevant.

it is not relevant for a poster to contain the actual footage of a film or the actual story of a book or the actual music of a gig -> they have to be "inside" (subpages). But it has to inform about all the different sections with only as much subpages as needed. 
On a website, that is supposed to be primarily a blog, it makes sense that the latest article is presented completely right on the main page.
On a website, where other things are supposed to be in focus, it makes sense for them to be in subpages.  








At the end I want to share a few websites which I think are really great and do a lot of the things that I propose as good practice. The best websites I know are:

* https://grapheneos.org (functional, minimal, beautiful)
* 


