<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style id="distill-article-specific-styles">
    <%=require("static/styles.css") %>
  </style>
  <script src="https://distill.pub/template.v2.js"></script>
</head>

<body>

  <d-front-matter>
    <script type="text/json">
      <%= JSON.stringify(require("./frontmatter.json"), null, 4) %>
    </script>
  </d-front-matter>

  <d-title>
    <h1>How we age - updated</h1>
    <p>A quantitative description of our functional decline</p>
  </d-title>

  <d-article>

    <p>
Aging is a complex phenomenon. How should we approach it?
    </p>

    <h4>Introduction</h4>
    <p>How and why do you age? We will take you through some of the major functions, and how they change with time. Additionally, we will cover the difference between cohort-based and longitudinal aging.</p>

    <h4>Cognition</h4>
    <p> We get worse on most cognitive tasks as we age.There are two major types of cognitive tasks - fluid intelligence and crystallized intelligence. Fluid intelligence is like processing speed - taking in and manipulating new information. Crystallized intelligence is like a concept graph or stored information - what you already know. Fluid intelligence appears to peak in your 20s and decline monotonically thereafter. Crystallized intelligence appears stable or increasing into your 60s, at which point it declines. </p>
    <p>Cohort and longitudinal studies show different results in cognitive aging. Cohort studies show monotonic decreases on most markers of cognitive function for fluid intelligence with age. Longitudinal studies, surprisingly, show increase longitudinal in cognitive function, particularly in the young. You see less of this over age 60. This could be explained by artifact (people dropping out to bias the results for those who stay), or possibly (though this is a guess) the Flynn effect (those born later might just be smarter than those of a similar age born earlier).</p>
<p> A heuristic for sample sizes is 300-5,000 individuals to detect a cognitive difference over 5 years with p<0.05 with .8 probability. You might expect your score to drop by a few points (on most of the major scales) every 5 years, after age 50.
</p>

<figure class="l-screen">                                                       
<div id="observablehq-5cb18737"></div>                                          
<script type="module">                                                          
import {Runtime, Inspector} from "https://cdn.jsdelivr.net/npm/@observablehq/ru\
ntime@4/dist/runtime.js";                                                       
import define from "https://api.observablehq.com/@laurademing/cognition-with-ag\
e.js?v=3";                                                                      
const inspect = Inspector.into("#observablehq-5cb18737");                       
(new Runtime).module(define, name => name === "chart" ? inspect() : undefined);
</script>                                                                       
</figure>  

    <h4>Hearing</h4>

    <p>As you age, structures inside the ear start to change and their functions decline. Your ability to pick up sounds decreases. You may also have problems maintaining your balance as you sit, stand, and walk.</p>
    <figure>                                                        
      <%= require("static/diagrams/crGIeDie01.svg") %>           
    </figure>   
    <h4>Movement</h4>
    <p>Physically inactive people lose 3-5% of muscle mass each decade after age 30.</p>                                                     
    <figure>                                                  
                                                                    
      <%= require("static/diagrams/4zUSlLFe01.svg") %>                                                                           
    </figure>
    
    <h4>Conclusion</h4>
    <p>
Aging is a complex and multifactorial proces.
    </p>


  </d-article>



  <d-appendix>
    <h3>Acknowledgments</h3>
    <p>
      We are deeply grateful to...
    </p>

    <p>
      Many of our diagrams are based on...
    </p>

    <h3>Author Contributions</h3>
    <p>
      <b>Research:</b> Joanne developed ...
    </p>

    <p>
      <b>Writing & Diagrams:</b> The text was initially drafted by...
    </p>


    <d-footnote-list></d-footnote-list>
    <d-citation-list></d-citation-list>
  </d-appendix>

  <!-- bibliography will be inlined during Distill pipeline's pre-rendering -->
  <d-bibliography src="bibliography.bib"></d-bibliography>

</body>
