## The Scriptlet
A scriptlet can contain any number of JAVA language statements, variable or method declarations, or expressions that are valid in the page scripting language.

Following is the syntax of Scriptlet −
```html
<% code fragment %>
```
You can write the XML equivalent of the above syntax as follows −

```html
<jsp:scriptlet>
   code fragment
</jsp:scriptlet>
```
## S.No.	Directive & Description

|Directive | Description|
|-----|---|
|<%@ page ... %> | Defines page-dependent attributes, such as scripting language, error page, and buffering requirements.|
|<%@ include ... %> | Includes a file during the translation phase.|
|<%@ taglib ... %> | Declares a tag library, containing custom actions, used in the page|
