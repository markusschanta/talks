# Overview (2 min)

**This presentation has three parts**: in the first one,...

After the presentation we'll have Q & A session. But if you have any questions about anything I mention during the talk, please let me know.

I will put these slides up on GitHub after the presentation. [...]

# Chart (3 min)

You **will probably have seen visualisations such as this one on the web**. This chart is a representation of different car models that were released in Europe, Japan and the US over a period of 10 years. Each dot represents one model.

On the **x axis** we've got horsepower and on the **y axis** miles per galon - so more fuel efficient cars are towards the top. The points are also color-coded by region.

**Underneath the scatter plot** we've also got a bar chart with the number of cars per year. 

These two **charts are linked** so if I click on any of the bars down here, the corresponding points up there are highlighted.

When we **click on 1970 over here, most of the cars from that year are not very fuel-efficient**. In particular the red points, which are cars produced in the US. When we go to **later years**, we can see how these points start to move to the left and up. There's one particular event that was a catalyst to that, the oil crisis 1973-74.

When you consider a visualisation such as this one, you can see how various elements, such as the colour coding and the interactivity can help you to get a better understanding of your dataset.

When I saw graphics such as this one, I immediately thought to myself: "That's really cool, I want to create visualisations such as that one." Many of these are done in D3, the Javascript library. So I sat down and tried to create one myself. If you do that, you soon find yourself wandering down a very deep and dark rabbit hole. You encounter things such as "Null is not an object". If you don't know any Javascript, this can be a rather frustrating experience.

So here's the good news: if you use Vega, you don't need to know any Javascript to create a chart like this one. So how does that work?

# Vega / SQL (1 min)

If someone asked me to describe Vega in one sentence, this is what I would tell them. I realise that this is a bold comparison, but I think the analogy goes very far:

- Vega is **declarative**. 
- Vega is a **specification rather than a library**. There is of course a library, that is the reference implementation, but anyone can write a different one.
- Vega is **language-agnostic**.

All of these properties are probably positive on the whole. So what does this look like in more detail?

# Roads to Vega (1 min)

So when we want to create a visualisation, the **desired end result is a rendered chart**. In the simplest case we need two ingredients for that: 

- First we need a **specification for the chart**. This is the heart of the matter. For Vega, this specification is represented as a JSON file.
- Second we need an **HTML page where we want to display the chart**. In this page well have a container, such as a div-element that will contain the chart. And then we'll have a short Javascript one-liner to tell the browser to render the chart to that element.

One of the exciting things is that there are various ways in which you can create these chart specs:

- The most obvious way is to write them by hand. Open up an editor and just write them down.
- There is also a library called Altair that allows you to generate them programmatically in Python.
- You can also create chart specs in a special GUI editor. That is perhaps the most convenient way to do this.

# Vega / Vega-Lite (1 min)

Vega comes in two different flavours: Vega and Vega-Lite. 

# Authors (1 min)

- Kanit WONG-SU-PHA-SA-WAT
- Dominik Moritz
- Arvind SAT-YA-NA-RA-YAN
- Jeffrey Heer 

** END OF PART I **