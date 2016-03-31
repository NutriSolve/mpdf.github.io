---
layout: page
title: InsertIndex()
parent_title: mPDF functions
permalink: /reference/mpdf-functions/insertindex.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>(mPDF &gt;= 6.0)</p>
<p>InsertIndex — Generate an Index for the document</p>
<h2>Description</h2>

<div class="alert alert-info" role="alert">void <b>InsertIndex</b> ([ int <span class="parameter">$usedivletters</span> [,&nbsp;boolean <span class="parameter">$uselinking</span> [, string <span class="parameter">$indexCollationLocale</span> [, string <span class="parameter">$indexCollationGroup</span> ]]]])</div>
<p>Inserts an Index for the document based on index entries made using &lt;<a href="/reference/html-control-tags/tocentry.html">indexentry</a>&gt; or <a href="/reference/mpdf-functions/indexentry.html">IndexEntry()</a>.</p>
<h2>Parameters</h2>
<p><span class="parameter">usedivletters</span></p>
<p class="manual_param_dd">Defines whether to divide index entries starting with the same letter, using a (large) letter as a heading.

<span class="smallblock">DEFAULT</span>: 1</p>
<p class="manual_param_dd"><b>Values</b>

1: show dividing letters in the Index

0: do not show dividing letters in the Index

<span class="smallblock">BLANK</span>&nbsp;or omitted uses a default value of 1</p>
<p><span class="parameter">uselinking</span></p>
<p class="manual_param_dd">Specify whether to add hyperlinks (internal links) to the entries in the document Index.

<span class="smallblock">TRUE</span> or 1: add links to Index 

<span class="smallblock">BLANK</span>&nbsp;or omitted, 0 or <span class="smallblock">FALSE</span>: do not add links to the Index

<span class="smallblock">DEFAULT</span>: <span class="smallblock">FALSE</span></p>
<p><span class="parameter"><span class="parameter">indexCollationLocale</span> </span></p>
<p class="manual_param_dd">Set a Locale to determine the overall sort order of index entries e.g. 'en_GB.utf8'. Available options are determined by the locales available in your system configuration. Always use a utf-8 locale.

<span class="smallblock">BLANK</span>&nbsp;or omitted uses current locale set in your system.</p>
<p><span class="parameter"><span class="parameter">indexCollationGroup</span> </span></p>
<p class="manual_param_dd">If you have set your index to use Dividing letters, this value will determine how letters are grouped under a dividing letter. Values should be selected from the files in folder <span class="filename">/collations/</span> e.g. 'English_United_Kingdom'

NB This will not affect the overall order of entries, which is determined by the value above.

<span class="smallblock">BLANK</span>&nbsp;or omitted - grouping occurs under the first letter of the index entries.</p>
<h2>Changelog</h2>
<table class="bpmTopic"> <thead>
<tr> <th>Version</th><th>Description</th> </tr>
</thead> <tbody>
<tr>
<td>6.0</td>
<td>
<p>Function was added</p>
</td>
</tr>
</tbody> </table>
<h2>See Also</h2>
<ul>
<li class="manual_boxlist"><a href="/what-else-can-i-do/index.html">Indexes</a></li>
</ul>
</div>
</div>
