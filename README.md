<div align="center">

## Protect Your Code


</div>

### Description

Simple way of preventing access to your client side javascripts and even style sheets
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[dselkirk](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dselkirk.md)
**Level**          |Intermediate
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |ASP \(Active Server Pages\)
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__4-14.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dselkirk-protect-your-code__4-7298/archive/master.zip)





### Source Code

I know that very single web developer has either wanted or has been asked
if they can protect there client side scripts. Now there's an answer, it
quite simply prevents an individual from downloading a HTML pages external
scripts files.
<br /><br />
<b>How it works</b><br />
Every good developer knows to rename all there script files to the asp
extension to protect their asp code. This unforunitely does not protect
your client side scripts. The way around it is since we already have our
files renamed to asp extensions, why not take advantage of it. All we need
to do is implement the <b>response.end</b> statement before the actualy
script and nothing will be viewed. The tricky part is to detect whether or
not you to allow the page to render. We can do this by performing some
simple <b>request.servervariable</b> checks. I create an include file
called "validate_view.asp". I simply include the file at the top of each
script file. I then call the procedure "validate_view" which is contained
in the include file. This will perform the check. I also pass the content
type with the procedure to make the page react as it should normally. The
procedure then performs some basic checks of where you came from, what
domain is being used and a couple others. You can even pass a querystring
called <b>page_pass</b> which allows you to view the page from anywhere.
You can even customize various parts of the code for your own personal
needs.
<br /><br />
<b>Download example</b><br />
<a href="http://www.planetsourcecode.com/vb/scripts/ShowCode.asp?txtCodeId=7252&lngWId=4">[here]</a>
<br /><br />
I appreciate any comments or suggestions you may have.

