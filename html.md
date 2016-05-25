**What doctype do?**   
For HTML documents, browsers use a DOCTYPE at the beginning of the document to decide how to handle it. load the page in the right way (typically Standard Mode): without it, the browser will load the page in [Quirks-mode](#quirks-mode). In HTML5 the doctype is reduced to *<!DOCTYPE html>*.

**Modes**  
The layout engine of the browser uses three modes
* *<a name="quirks-mode"></a>Quirks mode*  
nonstandard behavior emulation of Navigator 4 and IE 5
* *<a name="almost-standard-mode"></a>Almost standard mode*  
Only a small number of quirks are implemented
* *<a name="full-standard-mode"></a>Full standard mode*  
the behavior is the one described by the HTML and CSS specifications.

**Difference between HTML and XHTML**  
XHTML is actually an XML document using the HTML tags. It adds constraints for making the document well formatted, e.g. opening and closing tags for all the elements, lower case the name of the elements and attributes, DOCTYPE is mandatory and also the tags

```html
<html>, <head>, <title>, <body>
```

**Problems with serving pages as application/xhtml+xml**  
When requesting the document we add the content-type to the header of the request, some browser don't interpretate this value property and download the document instead of visualizing.

**Difference among cookie, local storage and session storage**
* Cookies are used to store informations on the browser for a specific domain and they are sent for every request to that domain. You can only save strings.
* SessionStorage and localStorage let you save informations as JSON and the size of this space depends on the browser, typically few tens of MB.
* SessionStorage differs from localStorage for the fact that the former will be deleted after the browser window will be closed.

**Progressive rendering**
Techniques used to render the page as quickly as possible, for example lazy loading of images and loading first the minimum css/content/scripts needed for visualizing the page.
