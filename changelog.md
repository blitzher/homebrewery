<style>
h5 {
	font-size: .35cm !important;
}
</style>

# changelog

### Tuesday, 17/08/2021 - v2.13.4
- Fixed user page crashing when user has untitled brew

##### G-Ambatte:
- Tweaks to user page tool tips
- Fix view counts being reset on Google Drive files

##### Gazook89 :
- New **PHB → Artist Credit** snippet
- **PRINT** snippets moved to the **Style Editor** tab

### Monday, 09/08/2021 - v2.13.3

##### G-Ambatte :
- Tooltips hovering over brews in dropdowns / user page.
- Fixed sort-by created date on user page.

##### Gazook89 :
- Hotkey Ctrl-/ and snippets to add HTML comments; use for notes that won't appear in your brew.

### Friday, 30/07/2021 - v2.13.2

- Background work to allow new themes in the future
- Fixed cursor getting stuck when resizing divider bar

##### G-Ambatte :
- Fix Style tab not copying when Cloned To New
- Basic brew sorting on User page
- Reduced data sent on each request from server

##### Gazook89 :
- Cleaned up styling on menus

### Saturday, 28/6/2021 - v2.13.1

- Fixed the issue with new brews not saving!

### Saturday, 26/6/2021 - v2.13.0

- "Share to Reddit" button now works with Google brews
- Downloading or viewing the source of your brew will now show the contents of the Style tab at the top of the document in a backtick code fence like this:

\`\`\`css

myStyle {color: black}

\`\`\`

##### G-Ambatte :
- New **Download**, **View**, and **Clone to New** buttons in the "Source" dropdown on the Share page.
- Pasting your brew into a "New" page and saving will transfer any CSS in the code fence to the Style tab.
- Unsaved work in the New page Style tab is now cached to your browser storage if you navigate away.

\page


### Thursday, 10/6/2021 - v2.12.0

- New "style" tab to better organize custom CSS in preparation for new themes and sharable styles.
- Your own Google brews will no longer show up in the list when viewing someone else's profile.

### Saturday, 02/5/2021 - v2.11.2

- Fix for edge case where brews could accidentally transfer from Google Drive back to Homebrewery.
- Move cursor to end of snippet after insertion

### Saturday, 20/3/2021 - v2.11.1

- Warning when opening brew in your Google Drive trash

##### G-Ambatte :
- Snippet to remove drop caps (fancy first letter after title)

### Saturday, 13/3/2021 - v2.11.0

- Many background things for upcoming v3. Get pumped.

##### G-Ambatte :
- Fixed new brews failing to save when auto-generated file name is too long.
- "New" button added to the Nav bar.
- "Download" button to download your brew as a text file.
- Reduced download size and improved caching.

##### RKuerten :
- Bold and Italics hotkeys for Mac users (Cmd+B, Cmd+I)

### Friday, 25/1/2021 - v2.10.7
- Cover Page snippet now flips left-right page numbering.
- Added instructions for [installing on a FreeBSD Jail](https://github.com/naturalcrit/homebrewery/blob/master/README.FREEBSD.md).
- Fix for box-shadows breaking across columns. <br>(Thanks G-Ambatte for all of these!)
- Small user interface tweaks (Thanks Ericsheid)

### Friday, 02/1/2021 - v2.10.6
- Fixed punctuation for usernames ending with 's' on the user page. (Thanks AlexeySachkov)
- Fixed server crashes due to excessive long lines in brews
- Fixed "automated request" lockouts from Google

### Friday, 18/12/2020 - v2.10.5
- Brews now immediately save when transferring between Google Drive and Homebrewery storage.
- Added confirmation popup to clarify the transfer process.
- Brews transferred or deleted from Google will be found in your Google Drive trash.
- Dependency updates.

### Wednesday, 25/11/2020 - v2.10.4
- Fixed Google Drive brews not saving metadata (view count, description, etc.) Note that we are still working on making published Google brews visible to the public when viewing your profile page.

### Thursday, 22/10/2020 - v2.10.3
- Fixed brews with broken code crashing the edit page when loaded (the "blue screen of death" bug).

### Monday, 19/10/2020 - v2.10.2
- Fixed issue with "recent" item links not updating when transferring between Google Drive.

### Monday, 12/10/2020 - v2.10.1
- Fixed issue with users unable to create new brews
- Fixing brews being lost when loaded via back button

\page

### Wednesday, 07/10/2020 - v2.10.0
- Google Drive integration -- Sign in with your Google account to link it with your Homebrewery profile. A new button in the Edit page will let you transfer your file to your personal Google Drive storage, and Google will keep a backup of each version! No more lost work surprises!

### Friday, 28/08/2020 - v2.9.2
- Many dependency updates
- Finally fixed this changelog page to not run off the edge :P

### Sunday, 19/07/2020 - v2.9.1
- Fixed paragraphs appearing blank on new columns

### Wednesday, 20/05/2020 - v2.9.0
- Major refactoring of site backend to work with updated dependencies for security (should be invisible to users)

### Wednesday, 11/03/2020 - v2.8.2
- Fixed delete button removing everyone's copy for brews with multiple authors
- Compressed homebrew text in database

### Monday, 26/11/2018 - v2.8.1
- Fixed some SSL issues with images in the example page so they appear now
- Fixed duplicate scrollbars in Edit Page
- Fixed issue of being unable to change brew metadata
- Sanitized script tags-javascript typed into the editor was crashing brews

### Sunday, 08/04/2018 - v2.8.0
- Re-enabled box shadows for PDF output
- Added a "contributing guide" for the GitHub
- "Report Issue" navbar button now links to the subreddit
- Refactored background code

### Sunday, 04/06/2017 - v2.7.5
- Fixed the class feature snippet duplicating the entire brew
- Fixed headers in tables being duplicated
- Fixed border-image being scrambled on class tables and descriptive text boxes
- Fixed pages going out of sync in large brews, causing them to be rendered off-page
- Improved performance in the preview window when scrolling through large brews
- Text in the "view source" page now wraps

### Saturday, 22/04/2017 - v2.7.4
- Give ability to hide the render warning notification

### Friday, 03/03/2017 - v2.7.3
- Increasing the range on the Partial Page Rendering for a quick-fix for it getting out of sync on long brews.

### Saturday, 18/02/2017 - v2.7.2
- Adding ability to delete a brew from the user page, incase the user creates a brew that makes the edit page unrender-able. (re:309)

### Thursday, 19/01/2017 - v2.7.1
- Fixed saving multiple authors and multiple systems on brew metadata (thanks u/PalaNolho re:282)
- Adding in line highlight for new pages
- Added in a simple brew lookup for admin

### Saturday, 14/01/2017 - v2.7.0
- Added a new Render Warning overlay. It detects situations where the brew may not be rendering correctly (wrong browser, browser is zoomed in...) and let's the user know

### Sunday, 25/12/2016 - v2.7.0
- Switching over to using Vitreum v4
  - Removed gulp, all tasks are run through npm scripts
- Updating docs for local dev
- Removing support for Docker. I have never used it, nor will I ever test for it, so I don't want to continue to explictly support it on this repo. Feel free to make a fork and make it docker-able though :)
- Changed icon for the metadata
- Made links useable in footer (thanks u/Dustfinger1 re:249)
- Added print media queries to remove box shadow on print (thanks u/dmmagic  re: 246)
- Fixed realtime renderer not functioning if loaded with malformed html on load (thanks u/RattiganIV re:247)
- Removed a lot of unused files in shared
- vitreum v4 now lets me use codemirror as a pure node dependacy

### Saturday, 03/12/2016 - v2.6.0
- Added report back to the edit page
- Changed metaeditor icon
- Added a button to quickly share your brew to reddit :)
- Disabled Partial Page Rendering unless your brew hits 75 pages or longer
- The brew renderer will now try and use your first page to judge the page size of each of your brews. This allows you now to set landscape and other weird sizes and everthing should work fine :)
- UI on the user page improved (thanks u/PalaNolho)
- Fixed lists not breaking across columns (thanks u/tyson-nw)
- Added a table of contents snippet (thanks u/tullisar)
- Added a multicolumn snippet

### Thursday, 01/12/2016
- Added in a snippet for a split table
- Added an account nav item to new page

### Sunday, 27/11/2016 - v2.5.1
- Fixed the column rendering on the new user page. Really should have tested that better
- Added a hover tooltip to fully read the brew description
- Made the brew items take up only 25% allowing you to view more per row.

\page

### Wednesday, 23/11/2016 - v2.5.0
- Metadata can now be added to brews
- Added a metadata editor onto the edit and new pages
- Moved deleting a brew into the metadata editor
- Added in account middleware
- Can now search for brews by a specific author
- Editing a brew in anyway while logged in will now add you to the list of authors
- Added a new user page to see others published brews, as well as all of your own brews.
- Added a new nav item for accessing your profile and logging in

### Monday, 14/11/2016
- Updated snippet bar style
- You can now print from a new page without saving
- Added the ability to use ctrl+p and ctrl+s to print and save respectively.

### Monday, 07/11/2016
- Added final touches to the html validator and updating the rest of the branch
- If anyone finds issues with the new HTML validator, please let me know. I hope this will bring a more consistent feel to Homebrewery rendering.

### Friday, 09/09/2016 - v2.4.0
- Adding in a HTML validator that will display warnings whenever you save. This should stop a lot of the issues generated with pages not showing up.

### Saturday, 20/08/2016 - v2.3.0
- Added in a license file
- Updated the welcome text
- Added in a much better Error page
- If you visit a deleted brew, it will now remove it from your recent list. (Thanks u/sIllverback!)
- Improved parsing of embedded html text in brews. (Thanks u/com-charizard!)
- Added in a new coverpage snippet
- Homebrewery will now try and onsert a good title for your brew if you don't provide one
- Homebrewery now re-renders properly when you zoom
- Fixed the noteblock overlapping into titles (thanks u/dsompura!)
- Fixed a bad search route in the admin panel (thanks u/SnappyTom!)

### Friday, 29/07/2016 - v2.2.7
- Adding in descriptive note blocks. (Thanks calculuschild!)

### Thursday, 07/07/2016 - v2.2.6
- Added a new nav item on the homepage for accessing both recently viewed and edited brews (thanks [ChosenSeraph!](https://github.com/stolksdorf/homebrewery/issues/147))

### Friday, 10/06/2016 - v2.2.4
- Added an id to each rendered page
- Allows adding in hyperlinks to specific pages
- Even works after you print to pdf!

### Tuesday, 07/06/2016 - v2.2.2
- Fixed bug with new markdown lexer and aprser not working on print page

### Sunday, 05/06/2016 - v2.2.1
- Adding in a new Class table div block. The old Class table block used weird stacking of HTML elements, resulting is difficult to control behaviour and poor interactiosn with the rest of the page. This new block is much easier to style and work with.
- Added in a new wide table snippet
- Added in a new auto-incremeting page number snippet (thakns u/Ryrok!)
- Lists in monster stat blocks should be fixed now

### Saturday, 04/06/2016 - v2.2.0
- MIgrating The Homebrewery over to hombrewery.naturalcrit.com. It know runs on it's own server, with it's own repo separate from the other tools I'm working on. Makes updating and deploying much easier.

### Sunday, 29/05/2016 - v2.1.0
- Finally added a syntax for doing spell lists. A bit in-depth about why this took so long. Essentially I'm running out of syntax to use in stardard Markdown. There are too many unique elements in the PHB-style to be mapped. I solved this earlier by stacking certain elements together (eg. an `<hr>` before a `blockquote` turns it into moster state block), but those are getting unweildly. I would like to simply wrap these in `div`s with classes, but unfortunately Markdown stops processing when within HTML blocks. To get around this I wrote my own override to the Markdown parser and lexer to process Markdown within a simple div class wrapper. This should open the door for more unique syntaxes in the future. Big step!
- Override Ctrl+P (and cmd+P) to launch to the print page. Many people try to just print either the editing or share page to get a PDF. While this dones;t make much sense, I do get a ton of issues about it. So now if you try to do this, it'll just bring you imediately to the print page. Everybody wins!
- The onboarding flow has also been confusing a few users (Homepage -> new -> save -> edit page). If you edit the Homepage text now, a Call to Action to save your work will pop-up.
- Added a 'Recently Edited' and 'Recently Viewed' nav item to the edit and share page respectively. Each will remember the last 8 items you edited or viewed and when you viewed it. Makes use of the new title attribute of brews to easy navigatation.
- Paragraphs now indent properly after lists (thanks u/slitjen!)

### Friday, 27/05/2016 - v2.0.6
- Updated the issue template for (hopefully) better reporting
- Added suggestion to use chrome while PDF printing

### Wednesday, 25/05/2016 -v2.0.5
- The class table generators have the proper ability score improvement progression.

\page

### Tuesday, 24/05/2016 - v2.0.4
- Fixed extra wide monster stat blocks sometimes only being one column
- The class table generators now follow the proper progression from the PHB (thakns u/IrishBandit)

### Thursday, 19/05/2016 - v2.0.2

- No longer server-side pre-render brews, just incase the user entered invalid HTML, it might crahsh the server
- Bumped up the allowed entity size for extra-large brew (Thanks for reporting it dickboner93)
- Added a little error box when a save fails with a custom link to reporting the issue on github.

### Saturday, 14/05/2016 - v2.0.0 (finally!)

I've been working on v2 for a *very* long time. I want to thank you guys for being paitent.
It started rather small, but as more and more features were added, I decided to just wait until everything was polished.

Massive changelog incoming:

#### Brews
- New flow for creating new brews. Before creating a new brew would immedaitely create a brew in the database and let you edit it. Many people would create a new brew just to experiment and close it, which lead to many "abandoned brews" (see the Under the hood section below). This started eating up a ton of database space. You now have to manually save a new brew for the first time, however Homebrewery will store anything you don't have saved in local storage, just in case your browser crashes or whatever, it will load that up when you go back to `/homebrew/new`
- Black blocking edges around notes and stat blocks when printing to PDFs have been fixed
- Borders sometimes not showing up in the second column have been fixed
- All pseudo-element borders have been replaced with reliable border images.
- Chrome can finally print to PDF as good as Chrome Canary! Updating instructions.
- Added a little page number box.
- Added in a new editable Brew Title. This will be shown in the navbar on share pages, and will default to the file name when you save as PDF. All exsisting brews will be defaulted with an empty title.
- Mutliline lists render better now
- Firefox rendering has been slithgly improved. Firefox and Chrome render things **slightly** differently, over the course of a brew, these little changes add up and lead to very noticable rendering differences between the browsers. I'm trying my best to get Firefox rendering better, but it's a difficult problem.
- A bunch of you have wanted to donate to me. I am super flattered by that. I created a [patreon page](https://www.patreon.com/stolksdorf). If you feel like helping out, head here :)

#### Under the Hood Stuff
- Setup a proper staging environment. Will be using this for tests, and hopefully getting the community to help me test future versions
- Server-side prerendering now much faster
- Regular weekly database back-ups. Your brews are safe!
- Database is now uniquely indexed on both editId and shareId, page loads/saving should be much faster
- Improved Admin console. This helps me answer people's questions about issues with their brews
- Added a whole querying/pagniation API that I can use for stats and answering questions
- Clearing out "Abandoned" brews (smaller than a tweet and haven't been viewed for a week). These account for nearly a third of all stored brews.

#### Interface
- Added in a whole new editor with syntax highlighting for markdown
- Built a splitpane! Remembers where you left the split in between sessions
- Re-organized the snippets into a hierarchical groups. Should be much easier to find what you need
- Partial page rendering is working. The Homebrewery will now only load the viewable pages, and any page with `<style>` tags on them. If you are working on a large brew you should notice *significant* performance improvements
- Edit page saving interface has been improved significantly. Auto-saves after 3 seconds on inactivity, now allows user to save at anytime. Will stop the tab from closing witha  pop-up if there are unsaved changes.
- Navbar and overall style has been improved and spacing made more consistent
- Elements under the hood are way more organized and should behaviour much more reliably in many sizes.
- Source now opens to it's own route `/source/:sharedId` instead of just a window. Now easier to share, and won't be blocked by some browsers.
- Print page now auto-opens print dialog. If you want to share your print page link, just remove the `?dialog=true` parameter and it won't open the dialog.

\page

### Wednesday, 20/04/2016
- A lot of admin improvements. Pagninated brew table
- Added a searching and removing abandoned brew api endpoints (turns out about 40% of brews are shorter that a tweet!).
- Fixed the require cache being cleared. Pages should render a bit faster now.
- Pulled in `kkragenbrink`s fix for nested lists, Thanks!


### Wednesday, 06/04/2016 - v1.4
* Pages will now partially render. This should greatly speed up *very* large homebrews. The Homebreery will figure out which page you should be looking at and render that page, the page before, and the page after.
* Zooming should be fixed. I've changed the font size units to be cm, which match the units of the page. Zooming in and out now look much better.


### Monday, 29/02/2016 - v1.3.1
* Removng the changelog button from the Share page
* Added a A4 page size snippet (thanks 	guppy42!)
* Added support for `<sup>` and `<sub>` tags (thanks crashinworld14!)

### Saturday, 20/02/2016
* Fixed h1 headers not going full width (thanks McToomin27)
* Added a github issue template

## v1.3.0

### Friday, 19/02/2016
* Improved the admin panel
* Added ability to clear away old empty brews
* Added delete button to the edit page
* Added a dynamically updating changelog page! Nifty!
* Added stlying for wide monster stat blocks and single column class tables
* Added snippets for wide monster stat blocks and single column class tables

### Tuesday, 16/02/2016
* Paragraphs right after tables now indent (thanks LikeAJi6!)
* Added a `@page` css rule to auto turn off margins when printing
* Added a `page-break` property on each `.phb` page to properly page the pages up when exporting (thanks Jokefury!)
* Improved first character rendering on Firefox
* Improved table spacing a bit
* Changed padding at page bottom for better fit and clipping of elements
* Improved spacing for bold text (thanks nickpunt!)


## v1.2.0

### Sunday, 17/01/2016
* Added a printer friendly snippet that injects some CSS to remove backbrounds and images
* Adjusted the styling specific to spell blocks to give it tighter spacing
* Added a changelog! How meta!

## v1.1.0

### Thursday, 14/01/2016
* Added view source to see the markdown that made the page
* Added print view
* Fixed API issues that were causing the server to crash
* Increased padding on table cells
* Raw html now shows in view source

## v1.0.0 - Release

### Wednesday, 3/01/2016

* Added `phb.standalone.css` plus a build system for creating it
* Added page numbers and footer text
* Page accent now flips each page
