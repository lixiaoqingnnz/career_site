+++
title =  "Home"
type = "home"
draft = false
+++


{{< showcase-section
    title="Li Xiaoqing"
    subtitle=`<span class="hero-subtitle-animated">Researcher, Coder, Problem Solver</span>`
    buttonText="Email"
    description=`Hi, I am <strong>Li Xiaoqing</strong>, a <em> AI researcher and coder</em> who loves turning messy real-world data into useful ideas.<br/><br/>My work spans <code>traditional machine learning, deep learning, and modern generative models</code>, including large language models (LLMs), diffusion-based synthesis, knowledge-graph reasoning, and retrieval-augmented generation (RAG). I am broadly interested in developing intelligent systems that combine learning, reasoning, and real-world data processing to achieve robust and scalable AI capabilities.<br/><br/>I am also committed to transforming these techniques into practical, real-world solutions—such as interactive websites, data-driven applications, and end-to-end LLM pipelines that enhance automation, analysis, and decision-making.`

    imgSrc="images/showcase/showcase.png"
    imgScale="0.3"
>}}

{{< platform-links >}}
    {{< link icon="linkedin" url="https://www.linkedin.com/in/xiaoqing-li-17a034247/" >}}
    {{< link icon="square-github" url="https://github.com/lixiaoqingnnz" >}}
    {{< link icon="medium" url="https://medium.com/@lixiaoqing.nnz" >}}
    {{< link icon="quote-left" url="https://scholar.google.com/citations?user=diqbYLoAAAAJ&hl=en" >}}

{{< /platform-links >}}

{{< /showcase-section >}}

<!-- {{< about-section
    title="About me"
    content="This content is using the <code>about-section</code> shortcode. <br/>You can write <code>HTML</code>, as long as you <em>wrap it</em> accordingly. "
    button_icon="icon-user"
    button_text="Check my skills"
    button_url="skills"
    imgSrc="images/about/user-picture.png"
    imgScale="0.15"
    text_align="center"
 >}} -->

{{< education-list
    title="🎓 Formal Education" >}}

{{< experience-section
    title="💼 My job experience"
    intro_title="Experience"
    intro_description="I work on <strong>ML research, LLM pipelines, and system development</strong>, with experience turning algorithms into practical tools for real-world use.<br></br>Please click on each experience to view more details!"
    button1_url="https://www.linkedin.com/in/xiaoqing-li-17a034247/"
    button1_text="See in linkedin"
    button1_icon="icon-linkedin"
    button2_text="Skills"
    button2_url="skills"
    hideViewAll="true"
>}}

<!-- 
{{< experience-list
    title="Experience"
    padding="false" >}}
-->

 
<!--
{{< client-and-work-section
    title="A selection of my work"
>}}
-->

<!--
{{< testimonial-section
    title="What they say about me"
>}}
-->

{{< spacer size="large" >}}

<!-- ## Extra home content

Additional content added after the `section` blocks, in the `home.md` file. 

Here you could freestyle, add other shortcodes, ...  Or just let the content empty, and rely on the shortcode sections alone.

{{< spacer size="small" >}}

{{< text-section
title="Extra (centered) content"
centered="true"
>}}

You can also use the `text-section` shortcode to add centered texts

{{< /text-section >}} -->


<script>
document.addEventListener('DOMContentLoaded', function () {
  const el = document.querySelector('.hero-subtitle-animated');
  if (!el) return;

  const fullText = el.textContent.trim(); // 原始文本
  const typingSpeed = 80;                 // 每个字的间隔（毫秒），可以自己调
  const pauseAfterFull = 2000;            // 打完后停顿多久再重来（毫秒）

  function startTypingLoop() {
    let idx = 0;
    el.textContent = '';

    function typeNext() {
      if (idx <= fullText.length) {
        el.textContent = fullText.slice(0, idx);
        idx++;
        setTimeout(typeNext, typingSpeed);
      } else {
        // 打完了，等一会儿，然后重新开始
        setTimeout(startTypingLoop, pauseAfterFull);
      }
    }

    typeNext();
  }

  startTypingLoop();
});
</script>


