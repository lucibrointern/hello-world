# hello-world
Readme instructions
MDWiki and Markdown for CS Range setup
 
Need to read up on “MD wiki” and “Markdown”.
1.	http://dynalon.github.io/mdwiki/#!index.md
2.	http://dynalon.github.io/mdwiki/#!quickstart.md 
3.	https://daringfireball.net/projects/markdown/
4.	https://daringfireball.net/projects/markdown/syntax#block
5.	https://www.markdownguide.org/basic-syntax/
Environment
1.	Wiki is at “ruwiki.trainer.dom” or http://wiki.trainer.dom/classwiki/mdwiki.html#!index.md
2.	Target directory (accessable via winscp)
a.	/var/www/html/classwiki
                                                               i.      Under here will need to be
1.	basic 
2.	intermediate
3.	advanced
4.	support
5.	other
b.	menu system will need to be extended in ‘classwiki’ directory
                                                               i.      So – “basic.md” will need links to basic/somedocname.md
                                                             ii.      Other stuff and files need to be dropped into ‘other’
c.	Each class page will need a “index.md” page that points to al of the docs
3.	The necessary ‘pandoc’ convert tool is on trainee-c1-01 only as well as ms word.
Doc Kit update
1.	Source docs are in t:\for_markdown\source
2.	Edit / extend the ‘convert.cmd’ scriptd in t:\for_markdown\
a.	Will need a convert basic, intermediate, advanced, other, etc. 
b.	Convert.cmd is a sample
c.	Must extend convert w/ approp source / dest doc variables
d.	Spaces in target file names are forbidden. Period. 
3.	Target docs need to go to appropriate matching sub directories under T:\For_Markdown\Destination
4.	Root url for docs = http://ruwiki.trainer.dom/classwiki/
Process 
1.	Convert a word doc and update script
2.	Use winscp to copy
3.	Hook up the ‘index’
4.	Edit the word doc until the converted MD doc looks good. 
a.	Move the doc forward by one minor version (1.8 becomes 1.9).
b.	Work on the newer version, getting all of the edits done. Advise Don o/t update.
c.	Once done, move the old version to an “archive” directory under its current directory.
d.	Make sure to update the ver # and last edited date under the title.
5.	“DO NOT” overwrite the source word doc – increment the version number in the file name b/c we will maintain the word doc and then auto convert / copy to the wiki site. 
Process Example:
1.	Edit the baseline word doc
a.	Source \ basic Basic \ Mod_1_Linux_CLA_V0.10.docx
2.	Update the convert script
a.	Source \ Convert_basic.cmd
b.	Update target files for md that do not have version numbers.
3.	Run script
4.	Use Winscp to copy to target
a.	File should be in destination \ basic
b.	Target location -regent@ruwiki:/var/www/html/classwiki/basic
5.	for new file
a.	update index.md in the ‘basic’ directory
b.	add the new file
6.	refresh the Web UI
a.	If the Web UI does not refresh
b.	Clear chrome history

