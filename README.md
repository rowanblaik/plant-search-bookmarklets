## Plant search bookmarklets

The following links are 'bookmarklets' – links allow you to search BBG's plant records via the its public website. You can search in two ways: by highlighting a plant name or accession number in your web browser and clicking the bookmarklets in your bookmarks bar; or by clicking the bookmarklets first and entering a plant details in the on-screen prompt.

### How to install

Make sure your web browser's bookmarks bar is visible and drag each of the following three links to it:

|Link|Search by|
|------|-----------------|
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20an%20accession%20number:',''))};Qr=Qr.replace(/(?!%5Ex)\D/gi,'');if(Qr)window.open('https://www.bbg.org/cgi/bgbase/detail.cgi?'+escape(Qr),'_blank');">BBG acc#</a>| accession number |
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name%20%28wildcard=*%29:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('https://www.bbg.org/cgi/bgbase/search.cgi?name='+escape(Qr),'_blank');">BBG name</a>| scientific name |
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20common%20plant%20name%20%28wildcard=*%29:',''))};if(Qr)window.open('https://www.bbg.org/cgi/bgbase/search_advanced.cgi?com_name='+escape(Qr),'_blank');">BBG com</a>| common name |

### To test your installation

Highlight the following plant name: _Magnolia_ × _brooklynensis_ and click the "BBG name" bookmark.

### Other plant databases

|Link|Search by|
|------|-----------------|
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://www.theplantlist.org/tpl1.1/search?q='+escape(Qr),'_blank');">TPL</a>| The Plant List |
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('https://www.rhs.org.uk/Plants/Search-Results?query='+escape(Qr),'_blank');">RHS</a>| RHS 'Find a plant' |
|<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x').replace(/['‘’]/g,'').replace(/%20/g,'+and+');if(Qr)window.open('http://apps.rhs.org.uk/horticulturaldatabase/summary2.asp?crit='+escape(Qr)+'&genus='+Qr.match('[a-zA-Z]+')+'&page=1_blank');">RHS</a>| RHS 'Hort DB'
<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://www.missouribotanicalgarden.org/PlantFinder/PlantFinderProfileResults.aspx?adv='+escape(Qr),'_blank');">MBG</a>| Mobot Plant Finder |
<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://plants.usda.gov/java/nameSearch?mode=sciname&keywordquery='+escape(Qr),'_blank');">USDA PLANTS</a>| USDA PLANTS database |
<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x').replace(/[\u2018\u2019]/g,'\u0027');if(Qr)window.open('https://garden.org/plants/search/text/?q='+escape(Qr),'_blank');">NGA plants</a>| NGA plants database |
<a href="javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://pfaf.org/user/Plant.aspx?LatinName='+escape(Qr),'_blank');">PFAF</a>| Plants for a Future |
<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'');if(Qr)window.open('http://newyork.plantatlas.usf.edu/Results.aspx?q='+escape(Qr),'_blank');">NYFA</a>| New York Flora Atlas |

### Credits

This bookmarklets were inspired by Kew's, now defunct, ePIC [browser button](http://epic.kew.org/tbutton.htm).
