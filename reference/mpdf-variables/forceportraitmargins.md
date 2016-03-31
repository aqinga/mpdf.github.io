---
layout: page
title: forcePortraitMargins
parent_title: mPDF Variables
permalink: /reference/mpdf-variables/forceportraitmargins.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>mPDF &gt;= 2.3</p>
<p>==========================================================

Special case - rotated margins on Landscape pages

==========================================================

$mpdf-&gt;forcePortraitMargins = true; (default = false)

If default page orientation is P(ortrait), then adding new page L(andscape) causes the left/right margins to be used as top/bottom, and vice-versa.

(NB similar to $forcePortraitHeaders which does the same but also rotates the [HTML] headers/footers.)</p>
<p>

NB - if using OddEven (double-sided document), it is the Portrait orientation L/R margins that alternate.</p>
<p>When adding a page, you must only call $mpdf-&gt;AddPage('L') or &lt;pagebreak orientaion="landscape" /&gt; - if you try to set new margins/headers etc. for new landscape pages when forcePortraitMargins=true, it will go wrong</p>
</div>
</div>
