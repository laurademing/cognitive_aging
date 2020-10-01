<!doctype html>

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
    <h1>An unsolved problem in cognitive aging</h1>
    <p>A quantitative description of our functional decline</p>
  </d-title>

  <d-article>

    <p>
      <b>TL;DR</b> the longitudinal and cross-sectional components of cohort-based cognitive aging studies generally disagree.
      Hypotheses propounded include the retest effect, attrition effect, and Flynn effect.

    </p>

    <h4>Introduction</h4>
    <p>While we get worse at certain cognitive tasks over time, we get better at others. Abilities that require crystallized intelligence — such as vocabulary and general information — typically stay stable or accumulate over time. Abilities that require fluid intelligence — such as reasoning, forming new associations, and solving novel problems — typically degrade over time.</p>

    <h4>Cognitive Aging Studies</h4>
    <p>You could take a measurement multiple times over many years. For example, a researcher could administer a cognitive test to a group of people aged 18-80 twice over a five years.</p>
    
    <p><b>PROS:</b> Researchers can establish a series of events and draw possible cause-effect conclusions from the study, which provides unique insights that sometimes cannot be obtained otherwise.</p>
    
    <p><b>CONS:</b> Can take a long time and cost a lot of $$$.  <d-footnote id="d-footnote-1">The Framingham Heart Study is a good example of this</d-footnote></p>
    <p>A hack to this is to take one measurement of young, middle-aged, and old people and compare. For example, a researcher could administer a cognitive test or set of cognitive tests to a group of people aged 18-80 once. However, any past or future cognitive tests administered would not be considered.</p>
    <p><b>PROS:</b> Many variables can be tested at once, with fairly quick results.</p>
    <p><b>CONS:</b> Not so accurate –– "snapshot" of individual's cognitive performance highly influenced by external factors.</p>
   <p>People call the first one "longitudinal" and the second one "cross-sectional".</p>
<p>You could also do a hybrid of these two and this is called "cohort-based", which takes cross-sectional measurements over time selecting for a cohort or cohorts based on a specific event such as birth, geographic location, or historical experience. 
 </p>

    <h4>A curious observation</h4>

    <p>
      Curiously, cross-sectional and longitudinal studies do not agree when grouped in cohorts by age! The graph below is taken from a study testing "episodic memory factor score", a proxy for verbal memory, over a period of five years grouped into cohorts by age.
      </p>
<figure class="l-screen">
<div id="observablehq-5cb18737"></div>
<script type="module">
import {Runtime, Inspector} from "https://cdn.jsdelivr.net/npm/@observablehq/runtime@4/dist/runtime.js";
import define from "https://api.observablehq.com/@laurademing/cognition-with-age.js?v=3";
const inspect = Inspector.into("#observablehq-5cb18737");
(new Runtime).module(define, name => name === "chart" ? inspect() : undefined);
</script>
</figure>

    <p>
      How to read the graph: In the above graph, each line represents a longitudinal measurement over a period of five years. Each different line represents a different cohort organized by age. <d-footnote id="d-footnote-2">Figure 2.2, Major Issues in Cognitive Aging by Timothy Salthouse: Means and standard errors of performance on different cognitive tests at different measurement occasions for adults of different ages. The connected lines represent longitudinal data from the same individuals, and different sets of lines correspond to different individuals.</d-footnote></p>

    </p>

    <p>
      For individuals younger than 60 years old, individual cohort performance increases over time when measured longitudinally. But when comparing performance between cohorts cross-sectionally, there is a consistent monotonic decline. So, these two measurements do not agree! Why this occurs is still an unsolved problem in cognitive aging.
    </p>

<p>There are current hypotheses that try to explain this contradiction:</p>

<p><b>Retest Effect:</b> taking the test multiple times makes you better at it, even over a period of 5+ years between taking the first cognitive test and the last cognitive test.</p>

<p>Possible solutions: find a better proxy for cognition that does not require administering a test, but continuously tracks function over a period of time. For example, correlating the speed and time in between taps and swipes on an iPhone to a one-time administered cognitive test that doesn't require an additional test.</p>

<p><b> Attrition Effect:</b> the kind of people who are likely to keep doing the longitudinal study are the kind of people for whom performance would be likely to get better, i.e. the people who drop out are the ones who would test poorly over time, skewing the test results to an increase in cognitive ability over time.</p>

   <p><b>Flynn Effect:</b> the cohort based studies show cognitive aging because (as noted elsewhere) measure of IQ are actually increasing for people of the same age born in later years. So, this doesn't have to do with aging at all, it's just showing that people born later (who would be different ages in the sane year) are getting smarter. 
</p>
    
    <h4>Conclusion</h4>
    <p>
Aging is a complex and multifactorial process.
    </p>


  </d-article>



  <d-appendix>
    <h3>Acknowledgments</h3>
    <p>
      We are deeply grateful to Timothy Salthouse for his excellent writing on this subject, and Sebastien Zany for extensive reviews and editorial commentary.
    </p>

    <p>
      Many of our diagrams are based on Timothy Salthouse's Figure 2.2 in Major Issues in Cognitive Aging.
    </p>

    <h3>Author Contributions</h3>
    <p>
      <b>Research:</b> LD and JP jointly conceived of and researched this project.
    </p>

    <p>
      <b>Writing & Diagrams:</b> The text was initially drafted by JP. LD made the diagram, but based off of Timothy Salthouse's book (it turns out he was wrong about the error bars, thought).
    </p>


    <d-footnote-list></d-footnote-list>
    <d-citation-list></d-citation-list>
  </d-appendix>

  <!-- bibliography will be inlined during Distill pipeline's pre-rendering -->
  <d-bibliography src="bibliography.bib"></d-bibliography>

</body>
