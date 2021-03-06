# MarkDown

## Getting Started

Markdown is a lightweight markup language that you can use to add formatting elements to plaintext text documents. Created by John Gruber in 2004, Markdown is now one of the world’s most popular markup languages.

Using Markdown is different than using a WYSIWYG editor. In an application like Microsoft Word, you click buttons to format words and phrases, and the changes are visible immediately. Markdown isn’t like that. When you create a Markdown-formatted file, you add Markdown syntax to the text to indicate which words and phrases should look different.Markdown syntax is designed to be readable and unobtrusive, so the text in Markdown files can be read even if it isn’t rendered.

#### Installing

Markdown requires Perl 5.6.0 or later. Markdown also requires the standard Perl library module Digest::MD5.

**MOVABLE TYPE**
Markdown works with Movable Type version 2.6 or later (including Movable Type 3.0).

1. Copy the “Markdown.pl” file into your Movable Type “plugins” directory. The “plugins” directory should be in the same directory as “mt.cgi”; if the “plugins” directory doesn’t already exist, use your FTP program to create it. Your installation should look like this:
  (mt home)/plugins/Markdown.pl
2. Once installed, Markdown will appear as an option in Movable Type’s Text Formatting pop-up menu. This is selectable on a per-post basis
   ![sreen](C:/Users/Admin/Pictures/Saved Pictures/screen.png, "demo")
   Markdown translates your posts to HTML when you publish; the posts themselves are stored in your MT database in Markdown format.

3. If you also install SmartyPants 1.5 (or later), Markdown will offer a second text formatting option: “Markdown With SmartyPants”. This option is the same as the regular “Markdown” formatter, except that it automatically uses SmartyPants to create typographically correct curly quotes, em-dashes, and ellipses. See the SmartyPants web page for more information.

4. To make Markdown (or “Markdown With SmartyPants”) your default text formatting option for new posts, go to Weblog Config: Preferences.


**BLOSXOM**
Markdown works with Blosxom version 2.0 or later.

1. Rename the “Markdown.pl” plug-in to “Markdown” (case is important). Movable Type requires plug-ins to have a “.pl” extension; Blosxom forbids it.

2. Copy the “Markdown” plug-in file to your Blosxom plug-ins folder. If you’re not sure where your Blosxom plug-ins folder is, see the Blosxom documentation for information.

3. That’s it. The entries in your weblog will now automatically be processed by Markdown.

4. If you’d like to apply Markdown formatting only to certain posts, rather than all of them, Markdown can optionally be used in conjunction with Blosxom’s Meta plug-in. First, install the Meta plug-in. Next, open the Markdown plug-in file in a text editor, and set the configuration variable $g_blosxom_use_meta to 1. Then, simply include a “meta-markup: Markdown” header line at the top of each post you compose using Markdown.

**BBEDIT**
Markdown works with BBEdit 6.1 or later on Mac OS X. It also works with BBEdit 5.1 or later and MacPerl 5.6.1 on Mac OS 8.6 or later. If you’re running Mac OS X 10.2 (Jaguar), you may need to install the Perl module Digest::MD5 from CPAN; Digest::MD5 comes pre-installed on Mac OS X 10.3 (Panther).

1. Copy the “Markdown.pl” file to appropriate filters folder in your “BBEdit Support” folder. On Mac OS X, this should be:

  BBEdit Support/Unix Support/Unix Filters/
  See the BBEdit documentation for more details on the location of these folders.

  You can rename “Markdown.pl” to whatever you wish.

2. That’s it. To use Markdown, select some text in a BBEdit document, then choose Markdown from the Filters sub-menu in the “#!” menu, or the Filters floating palette


## How Does it Work?
Dillinger makes writing in Markdown easy because it hides the stuff happening behind the scenes, but it’s worth exploring how the process works in general.

When you write in Markdown, the text is stored in a plaintext file that has an .md or .markdown extension. But then what? How is your Markdown-formatted file converted into HTML or a print-ready document?

The short answer is that you need a Markdown application capable of processing the Markdown file. There are lots of applications available — everything from simple scripts to desktop applications that look like Microsoft Word. Despite their visual differences, all of the applications do the same thing. Like Dillinger, they all convert Markdown-formatted text to HTML so it can be displayed in web browsers.

Markdown applications use something called a Markdown processor (also commonly referred to as a “parser” or an “implementation”) to take the Markdown-formatted text and output it to HTML format. At that point, your document can be viewed in a web browser or combined with a style sheet and printed. 

    ![Process of Markdown](C:/Users/Admin/Pictures/Saved Pictures/process.png, "The Markdown Process") 

## Examples
| Text using Markdown syntax    | Text viewed in a browser |
| ----------- | ----------- |
|  ## Sub-heading   | **Sub-heading**   |
| Text attributes \_italic_\, \**bold**\, \`monospace\`.  |Text attributes _italic_,**bold**, `monospace`.  
|Bullet list:      *apples *oranges *pears | Bullet list: apples oranges pears

  
## Author
 **John Gruber** created the Markdown language in 2004 in collaboration with Aaron Swartz on the syntax, with the goal of enabling people "to write using an easy-to-read and easy-to-write plain text format, optionally convert it to structurally valid XHTML (or HTML)"


#   M a r k d o w n  
 