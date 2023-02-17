---
title: tocbot_english
layout: post
---

{::options parse_block_html="true" /}

### [tocbot](https://github.com/tscanlin/tocbot#options) **Options**

<div class="table-responsive">

{:.table}
| option  | value  | description  |
| :------------ | :------------ | :------------ |
| tocSelector  | `.js-toc`  | Where to render the table of contents  |
|tocElement   | element  | Or, you can pass in a DOM node instead  |
| contentSelector  | `.js-toc-content`  | Where to grab the headings to build the table of contents  |
| contentElement  | element  | Or, you can pass in a DOM node instead  |
| headingSelector  | 'h1, h2, h3'  | Which headings to grab inside of the contentSelector element  |
|ignoreSelector   | `'.js-toc-ignore'`  | Headings that match the ignoreSelector will be skipped  |
| hasInnerContainers  |false   | For headings inside relative or absolute positioned containers within content  |
| linkClass  | `'toc-link'`  |  Main class to add to links |
| extraLinkClasses  | `''`  | Extra classes to add to links  |
| activeLinkClass  | `'is-active-link'`  | Class to add to active links,the link corresponding to the top most heading on the page  |
| listClass  | `'toc-list'`  | Main class to add to lists  |
|extraListClasses   | `"`  | Extra classes to add to lists  |
| isCollapsedClass  | `'is-collapsed'`  | Class that gets added when a list should be collapsed  |
| collapsibleClass  | `'is-collapsible'`  |Class that gets added when a list should be able to be collapsed but isn't necessarily collapsed   |
| listItemClass  | `'toc-list-item'`  |Class to add to list items   |
| activeListItemClass  | `'is-active-li'`  | Class to add to active list items   |
| collapseDepth  | 0  |  How many heading levels should not be collapsed.For example, number 6 will show everything since there are only 6 heading levels and number 0 will collapse them all. The sections that are hidden will open and close as you scroll to headings within them.  |
| scrollSmooth  | true  | Smooth scrolling enabled  |
| scrollSmoothDuration  | 420  | Smooth scroll duration  |
|scrollSmoothOffset  | 0  | Smooth scroll offset  |
|scrollEndCallback   | `function (e) {}`  | Callback for scroll end  |
| headingsOffset  | 1  |Headings offset between the headings and the top of the document (this is meant for minor adjustments)   |
| throttleTimeout  | 50  | Timeout between events firing to make sure it's not too rapid (for performance reasons)  |
| positionFixedSelector  | null  | Element to add the positionFixedClass to  |
| positionFixedClass  | `'is-position-fixed'`  |Fixed position class to add to make sidebar fixed after scrolling down past the fixedSidebarOffset   |
| fixedSidebarOffset  | `'auto'`  | fixedSidebarOffset can be any number but by default is set to auto which sets the fixedSidebarOffset to the sidebar element's offsetTop from the top of the document on init  |
| includeHtml  | false  | includeHtml can be set to true to include the HTML markup from the heading node instead of just including the textContent  |
| includeTitleTags  | false  | includeTitleTags automatically sets the html title tag of the link to match the title. This can be useful for SEO purposes or when truncating titles  |
| onClick  | `function (e) {}`  | onclick function to apply to all links in toc. will be called with the event as the first parameter, and this can be used to stop, propagation, prevent default or perform action  |
| orderedList  | true  | orderedList can be set to false to generate unordered lists (ul) instead of ordered lists (ol)  |
| scrollContainer  | null  | If there is a fixed article scroll container, set to calculate titles' offset  |
| skipRendering  | false  | prevent ToC DOM rendering if it's already rendered by an external system  |
| headingLabelCallback  | false  | Optional callback to change heading labels.For example it can be used to cut down and put ellipses on multiline headings you deem too long.Called each time a heading is parsed. Expects a string and returns the modified label to display.Additionally, the attribute `data-heading-label` may be used on a heading to specify a shorter string to be used in the TOC.function (string) => string  |
| ignoreHiddenElements  | false  | ignore headings that are hidden in DOM  |
| headingObjectCallback  | null  | Optional callback to modify properties of parsed headings. The heading element is passed in node parameter and information parsed by default parser is provided in obj parameter. Function has to return the same or modified obj. The heading will be excluded from TOC if nothing is returned.`function (object, HTMLElement) => object / void`  |
| basePath  | `''`  | Set the base path, useful if you use a `base` tag in `head`  |
| disableTocScrollSync  | false  | Only takes affect when `tocSelector` is scrolling, keep the toc scroll position in sync with the content  |
| tocScrollOffset  | 0  | Offset for the toc scroll (top) position when scrolling the page. Only effective if `disableTocScrollSync` is false.  |

</div>

1. `abs`
  + 返回一个数字的绝对值
   - {{ 4 | abs }} 输出：4
   - {{ -17 | abs }} 输出：17
  + abs也适用于仅包含数字的字符串
   - {{ "-19.86" | abs }} 输出19.86
    +
    +
    +
    +
    +
    +  
1. `append`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `at_least`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `at_most`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `capitalize`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `ceil`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `compact`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `concat`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `date`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `default`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `divided_by`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `downcase`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `escape`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `escape_once`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `first`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `floor`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `join`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `last`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `lstrip`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `map`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `minus`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `modulo`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `newline_to_br`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `plus`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `prepend`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `remove`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `remove_first`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `replace`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `replace_first`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `reverse`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `round`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `rstrip`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `size`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `slice`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `sort`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `sort_natural`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `split`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `strip`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `strip_html`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `strip_newlines`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `times`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `truncate`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `truncatewords`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `uniq`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `upcase`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `url_decode`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `url_encode`
  > + 
    +
    +
    +
    +
    +
    +
    +  
1. `where`
  > + 
    +
    +
    +
    +
    +
    +
    +  
