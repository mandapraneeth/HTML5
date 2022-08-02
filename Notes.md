
Kinds of Content
Each element in HTML falls into zero or more categories that group elements with similar characteristics together. The following broad categories are used in the specification.
* Metadata content
* Flow content
* Sectioning content
* Heading content
* Phrasing content
* Embedded content
* Interactive content

These categories are related as follows:












Sectioning content, heading content, phrasing content, embedded content, and interactive content are all types of flow content. Metadata is sometimes flow content. Metadata and interactive content are sometimes phrasing content, and sometime is interactive content.

Other categories are also used for specific other purposes. example Form controls are specified using a number of categories to define common requirements. Some elements have unique requirements and do not fit into any particular categories.


Metadata content
----------------
metadata content is content that sets up the presentation or behavior of the rest of the content, or that sets up the relationship of the document with other documents or that conveys other "Out of band" information

=> base, link,  meta, noscript, script, style, template, title


Flow content
------------
most elements that are used in the body of document and applications are categorized as flow content.

=> a, abbr, address, area (if it is a descendent of a map element), article, aside, audio, b, bdi, bdo, blockqoute, br, button, canvas, cite, code, data, datalist, del, details, dfn, dialog, div, dl, em, embed, fieldset, figure, footer, form, h1, h2, h3, h4, h5, h6, header, hgroup, hr, i, iframe, img, input, ins, kbd, label, link ( if it is allowed in the body), main (if it is a hierachically correct main element), map, mark, MathML math, menu, meta(if the itemprop attribute is present), meter, nav, noscript, object, ol, output, p, picture, pre, progress, q, ruby, s, samp, script, section, selection, select, slot, small, span, strong, sub, sup, SVG svg, table, template, textarea, time, u,        
ul, var, video, wbr, autonomous custom element, text

Sectioning content
------------------
sectioning content is content that defines the scope of headings and footers

=> article, aside, nav, section

Each sectioning content element potentially has a heading and an outline. see the section on headings and sections for further details.

Heading content
---------------
Heading content define the header of a section ( whether explicitly marked up using section content elements, or implied by the heading content itself)

=> h1, h2, h3, h4, h5, h6, hgroup

Phrasing content
----------------
phrasing content is the text of the document, as well as elements that mark up that text at the intra paragraph level. Runs of phrasing content form paragraphs.

=> a, abbr, area( if it is a descendant of a map element), audio, b, bdi, bdo, br, button, canvas, cite, code, date, datelist, del, dfn, em, embed, I, iframe, img, input, ins, kbd, label, link (if it is allowed in the body) map, mark, MathML math, meta( if the itemprop attribute is present), meter, noscript, object, output, picture, progress, q, ruby, s, samp, script, select, slot, small, span, strong, sub,sup, SVG svg, template, textarea, time, u, var,video, wbr, autonomous custom elements,text.

Embedded content
-----------------
Embedded content is content that imports another resource into the document, or content from another vocabulary that is inserted into the document.

=> audio, canvas, embed, iframe, img, MathML math, object, picture, SVG svg, video


Interactive Content
-------------------
Interactive content is content that is specifically intended for user interactive 

=> a(if the href attribute is present), audio( if the controls attribute is present), button, details, embed, iframe, img, ( if the use map attribute is present), input( if the type attribute is not in the Hidden state), label, object( if the use map attribute is present), select, textarea, video(if the controls attribute is present)

Palpable content
----------------
As a general rule, element whose content model allows any flow content or phrasing content should have at least one node its content that is palpable content and that does not have the hidden attribute specified.
note: Palpable content make an element non-empty by providing either some desendant non-empty text, or else something users can hear ( audio elements) or view ( video or img or canvas elements ) or otherwise interact with (video or img or canvas elements) or otherwise interact with ( for example interactive form controls)

This requirement is not hard requirment, how ever as there are many cases where an element can be empty legitimately, for example when it is used as a placeholder which will later be filled by a script, or when the element is a part of a template and would on most pages be filled in but on some page is nor relevent.

The following elements are palpable content
=> a, abbr, address, article, aside, audio ( if the controls attribute is present) b, bdi, bdo, blockquote, button, canvas, cite, code, date, details, dfn, div, dl ( if the elements children include at least one name value group) em, embed, fieldset, figure, footer, form, h1, h2, h3, h4, h5, h6, hgroup, header,
I, iframe, img, input, ( if the type attribute is not in the hidden state) ins, kbs, label, main, map, mark, MathML math, menu, ( if the elements children include at least one li element), meter, nav, object, ol( if the element children include at least one li element), output, p, pre, progress, q, ruby, s, SVG svg, samp, section, select, small, span, strong, sub, sup, table, textarea, time, u, ul, (it the elements children include at least one li element) , var, video, autonomous custom element, text that is not inter element whitespace


Script-support element
-----------------------
Script supporting element are those that do not represent anything themselves ( i.e, they are not rendred), but are used to support script .. eg to provide functionally for the user

The following elements are script-supporting elements
=> script, template

Global attributes
-----------------
 The following attributes are common to and may be specified on all HTML elements ( even those not defined in this specification)

	• accesskey
	• autocapital
	• autofocus
	• contenteditable
	• dir
	• draggable
	• enterkeyhint
	• hidden
	• inputmode
	• is
	• itemid
	• itemprop
	• itemref


The following event handler content attributes may be specified on any HTML element:

	• onabort
	• onauxclick
	• onblur
	• oncancel
	• oncanplay
	• oncanplaythrough
	• onchange
	• onclick
	• onclose
	• oncontextmenu
	• oncopy
	• oncuechange
	• oncut
	• ondblclick
	• ondrag
	• ondragend
	• ondragenter
	• ondragexit
	• ondragleave
	• ondragover
	• ondragstart
	• ondrop
	• ondurationchange
	• onemptied
	• onended
	• onerror
	• onfocuse
	• onformdata
	• oninput
	• oninvalid
	• onkeydown
	• onkeypress
	• onkeyup
	• onload
	• onloadeddata
	• onloadedmetadata
	• onloadstart
	
	
	
	
	The elements of HTML
	--------------------
	html, head, title, base, link, meta, style, body, article, section, nav, aside, h1, h2, h3, h4, h5, h6, hgroup, header, footer, address, p, hr, pre, blackqoute, ol, ul, menu, li, dl, dt, dd, figure, figcaption, main, div, a, em, strong, small, s, cite, q, dfn, abbr, ruby, rt, rp, data, time, code, var, samp, kbd, sub, sup, i, b, u,mark, bdi, bdo, span, br, wbr, area, ins, del, picture, source, img, iframe, embed, object, param, video, audio, track, map, area, table, caption, colgroup, col, tbody, thead, tfoot, tr, td, th, form, label, input, button, select, datalist, optgroup, option, textarea, output, progress, meter, fieldset, legend, details, summary, slot, canvas, marquee, meter, progress, select, textarea, frameset, xmp
	
	Links
	-----
	alternate, author, bookmark, canonical, dns-prefetch, external, help, icon, licence, maifest, modulepreload, nofollow, noopener, norefferrer, opener, pingback, preconnect, prefetch, preload, prerender, search, stylesheet, tag, next, prev
	
	
	type= attribute
	----------------
	type= hidden text, search, tel, url, email, password, date, mont, week, time, number, datetime-local, range, color, checkbox, radio, file, submit, image, reset, button
	
	input attribute
	---------------
	maxlength and minlength attribute
	size, randomly, required, multiple, pattern, min, max, step, list, placeholder, disable, autocomplete, itemprop, hidden, tabindex, autofocus, accesskey, itemprop, hidden, tabindex, autofocus, accesskey, countenteditable, inputmode, enterkeyhint, draggable, title
	
	element MATHML & SVG
	---------------------
	MathML mi, MathML mo, MathML mn, MathML ms, MathML mtext, and MathML annotation-xml, and SVG foreign Object, SVG desc and SVG title, MathML math, MathML math, MathML merror, SVG use, SVG svg, SVG script, SVG image, SVG a
	
	• onmousedown
	• onmouseleave
	• onmouseenter
	• onmouseleave
	• onmousemove
	• onmouseout
	• onmouseover
	• onmouseup
	• onpaste
	• onpause
	• onplay
	• onplaying
	• onprogress
	• onratechange
	• onreset
	• onresize
	• onscroll
	• onsecuritypolicyviolation
	• onseeked
	• onseeking
	• onselect
	• onslotchange
	• onstalled
	• onsubmit
	• onsuspend
	• ontimeupdate
	• ontoggle
	• onvolumechange
	• onwaiting
	• onwheel


CSS modules
----------------
	• viewport
	• line box
	• out-of-flow
	• in-flow
	• context area
	• border box
	• content box
	• margin box
	• border edge
	• margin edge
	• collapsing margins
	• containing block
	• inline box
	• block box


	• margin-top, margin-bottom, margin-left, margin-right
	• padding-top, padding-bottom, padding-let, padding-right
	• top, bottom, left, right
	• float
	• clear
	• width
	• height
	• line-height
	• vertical-height
	• content
	• inline-block value of 'display' prop
	• visibility


CSS border properties
-----------------------------

                      Top                                      Bottom                                          left                                          right
width       border-top-width              border-bottom-width            border-left-width             border-right-width
style         border-top-style                border-bottom- style             border-left-style              border-right-style
color         border-top-color              border-border-color                border-left-color             border-right-color

CSS logical properties
-----------------------------
	• margin-block-start, margin-block-end, margin-inline-start, margin-inline-end
	• padding-block-start, padding-block-end, padding-inline-start, padding-inline-end
	• border-block-start-width
	• block-size
	• inline-size

	CSS color
	------------
	•  name color
	• <color>
	• the 'color' property
	• the 'current color' value
	• opaque black
	• transparent black
	

CSS image
---------------
	• default object size
	• intrinsic dimensions
	• intrinsic aspect ratio
	• intrinsic height
	• intrinsic width
	• image-orientation
	• object-fit

CSS background and Border
-----------------------------------
	• background-color 
	• background-image
	• border-radius

CSS Display
---------------
	• outer display type
	• block-level
	• block container
	• formatting content
	• block formatting content
	• inline formatting content
	• absolutely positioned
	• replaced element
	• css box

CSS flexible Box Layout
-------------------------------
	• flex-direction
	• flex-wrap

CSS grid Layout
--------------------
	• grid-auto-flow
	• grid-auto-rows
	• grid-column-gap
	• grid-row-gap
	• grid-template-area
	• grid-template-columns
	• grid-template-row

CSS-inline layout
---------------------
	• ascent-metric
	• descent-metric

CSS font
-------------------
	•  font-family
	• font-weight
	• font-size
	• font

CSS intrinsic & Extensic
-----------------------------
	• fit-content inline size

CSS overflow
------------------
	• 'overflow' prop 'hidden' value
	• text-overflow

CSS position layout
-------------------------
	• 'position' prop 'static' value

CSS Multi-column layout
----------------------------------
	• column-count
	• column-fill
	• column-gap
	• column-rule
	• column-width

CSS ruby layout
---------------------
	• 'ruby-base' value 'display' prop


CSS Table
------------
	• border-spacing
	• border-collapse
	• table-cell, table-row, table-caption 'table' value, display prop

CSS writing model
------------------------
	• direction
	• unicode-bidi
	• block flow direction, block size, inline size, block-start
           block-end, inline-start, inline-end, inline-left, inline-right

CSS Basic user interface
-------------------------------
	• outline
	• cursor
	• appearance

CSS Text
-----------
	• text-transform
	• white-space
	• text-align
	• letter-spacing

CSS Values and units
------------------------------
	• <length>
	• em
	• ex
	• vw
	• in
	• px
	• attr()
	• math function
