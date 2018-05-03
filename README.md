## Plant search bookmarklets

The following links are 'bookmarklets' – special links to allow you to search BBG's plant records via the its public website. You can search in two ways: by highlighting a plant name or accession number in your web browser and clicking the bookmarklets in your bookmarks bar; or by clicking the bookmarklets first and entering a plant details in the on-screen prompt.

### Demo

To demo and install the following bookmarklets, go to https://rowanblaik.github.io

#### BBG Accession number search:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20an%20accession%20number:',''))};Qr=Qr.replace(/(?!%5Ex)\D/gi,'');if(Qr)window.open('https://www.bbg.org/cgi/bgbase/detail.cgi?'+escape(Qr),'_blank');````

#### BBG Plant name search:
````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name%20%28wildcard=*%29:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('https://www.bbg.org/cgi/bgbase/search.cgi?name='+escape(Qr),'_blank');````

#### BBG Common name search:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20common%20plant%20name%20%28wildcard=*%29:',''))};if(Qr)window.open('https://www.bbg.org/cgi/bgbase/search_advanced.cgi?com_name='+escape(Qr),'_blank');````

#### The Plant List:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://www.theplantlist.org/tpl1.1/search?q='+escape(Qr),'_blank');````

#### RHS Find a Plant:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('https://www.rhs.org.uk/Plants/Search-Results?query='+escape(Qr),'_blank');````

#### RHS Hort Database:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x').replace(/['‘’]/g,'').replace(/%20/g,'+and+');if(Qr)window.open('http://apps.rhs.org.uk/horticulturaldatabase/summary2.asp?crit='+escape(Qr)+'&genus='+Qr.match('[a-zA-Z]+')+'&page=1_blank');````

#### MOBOT Plant Finder:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://www.missouribotanicalgarden.org/PlantFinder/PlantFinderProfileResults.aspx?adv='+escape(Qr),'_blank');````

#### USDA Plants:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://plants.usda.gov/java/nameSearch?mode=sciname&keywordquery='+escape(Qr),'_blank');````

#### NGA Plants database:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x').replace(/[\u2018\u2019]/g,'\u0027');if(Qr)window.open('https://garden.org/plants/search/text/?q='+escape(Qr),'_blank');````

#### Plants for a Future:

````javascript:Qr=document.getSelection().toString();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'x');if(Qr)window.open('http://pfaf.org/user/Plant.aspx?LatinName='+escape(Qr),'_blank');````

#### NY Flora Atlas

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter%20a%20scientific%20plant%20name:',''))};Qr=Qr.replace(/%C3%97/g,'');if(Qr)window.open('http://newyork.plantatlas.usf.edu/Results.aspx?q='+escape(Qr),'_blank');````

### Credits

This bookmarklets were inspired by Kew's, now non-functional, ePIC [browser button](http://epic.kew.org/tbutton.htm).
