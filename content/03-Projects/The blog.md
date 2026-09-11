This very blog is my most recent side project—something I’ve wanted to build for years. I never started, mostly leaning on the usual excuses: no time, too much doomscrolling, and so on. But lately, I realized I was slipping into a spiral of neither thinking nor doing anything that genuinely interested me. I missed building things.

The idea was already cooked inside of me; I just needed to lock in and make it happen. The first real question was: How the hell am I doing this?
## The visual brand

First, I wanted to create a personal visual brand based on my own ideas about myself—not necessarily strictly professional, though I wanted to keep that in mind too. (I'll actually be publishing my process for creating that visual brand soon as another side project!).

I had done some basic visual design before and developed a bit of a feel for turning ideas into visuals. Since I figured I knew myself pretty well, I knew exactly what I wanted to represent. After some sketching, I ended up with a great concept: using the letters of my name to create a representation of a boulder (the letter O) scaling an inclined mountain (the letter M).
## The technical side
Once the visual side was settled, it came down to the technical question: How do I actually build this? A few years ago I dabbled a bit in web dev for side projects like this, but my knowledge was outdated and basic. 
### The main tool (*Quartz 5.0*)
Still, I had a clear vision, started looking around, and ended up finding Quartz. Since the main purpose of this blog is just to write things down, it was the absolute perfect fit. So, I chose it that way.
The current up to date version that I found for Quartz at the time I started this was v5.

I stuck with it and started looking at the pros and cons. On the plus side, it’s pretty user-friendly. The main workflow using Obsidian is absurdly easy, but you always have the option to go more advanced if you want to add your own components and tinker around. It’s a pretty solid option for both entry-level folks and anyone who wants to get their hands dirty in a techy way.
### The domain registration (*Porkbun*)

Once I figured out the main tool for building the static site locally and got used to Quartz's workflow and philosophy, I started looking for a way to publish it with a custom domain. I ended up wading through a lot of options—mostly trash, honestly, full of monthly fees and hidden costs. Of course, I hated that idea, so I kept digging until I found the most basic, affordable, and straightforward way to do it.

Porkbun showed up as the savior, a pretty simple organization that allows you to get your hands on domains without a lot of add ons. Simple and steady, finding something like that in the current times is no easy task. After some looking up, finding the *orlandomejia.me* as the most affordable and reasonable domain to buy. It seems like domains have a yearly fee of renewal if you want to keep them, for this one I have paid around 17 US upfront with no discount (pretty unlucky btw, being one of the few without first year discount).

## The omnipresent (*github*)

Of course, GitHub being part of the project is no surprise. Beyond the usual benefits, it played a key role here because I originally used it to host via GitHub Pages—even though I ultimately switched to a different hosting tool.

## The builder (*Cloudfare*)

The final piece of the puzzle was Cloudflare, which essentially handles everything related to web deployment. At first, I tried using it just as a DNS redirector to point my custom domain to the site I was hosting on GitHub Pages. After running into a few issues there, I ended up exploring Workers and Pages. Once I weighed the advantages and limitations of the free tier, I realized it was more than enough for my purposes.

I'm still trying to wrap my head around how web deployment works and all the data Cloudflare displays on its dashboards. For the blog side, though, it was pretty easy to set up. Once you link your repository to Workers and Pages, you configure it just once, set a deploy command, and from then on, a few quick commands in your local terminal publish and deploy your updates straight to the live blog.

## The final workflow.

Once the infrastructure is set up with the tools I just described, the workflow is pretty straightforward. Having your own blog or digital garden is essentially a one-evening project. After building the foundation, you just open Obsidian, point a vault to your Quartz project's content directory, and write your entries. Run a few commands in your Git terminal, and that's it—DONE. (I'm guessing some troubleshooting will be needed down the road after updates and broken dependencies, but hopefully nothing too painful!)

Note: Now that I've built this, it feels like an empty canvas waiting for my ideas. I know I won't always be consistent, but I'm pretty sure I'll keep coming back—because writing for my future self is something I truly enjoy.
