## Plant search bookmarklets

The following links are 'bookmarklets' – special links to allow you to quickly search BBG's plant records, and several other institutions plant databases, via their public websites. You can search in two ways: by highlighting plant name text or accession numbers in your web browser and clicking the bookmarklets in your bookmarks bar; or by clicking the bookmarklets first and entering a plant details in the on-screen prompt.

### Demo

To demo and install the following bookmarklets, go to https://rowanblaik.github.io

#### BBG Accession number search:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter an accession number:',''))};Qr=Qr.replace(/(?!^x)\D/gi,'');if(Qr)window.open('https://www.bbg.org/cgi/plant-records/detail.cgi?'+encodeURIComponent(Qr),'_blank');````

#### BBG Common name search:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a common plant name (wildcard=*):',''))};if(Qr)window.open('https://www.bbg.org/cgi/plant-records/search_advanced.cgi?com_name='+encodeURIComponent(Qr),'_blank');````

#### BBG Scientific name search:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name (wildcard=*):',''))};if(Qr)window.open('https://www.bbg.org/cgi/plant-records/search.cgi?name='+encodeURIComponent(Qr),'_blank');````

#### RHS Find a Plant:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('https://www.rhs.org.uk/Plants/Search-Results?query='+encodeURIComponent(Qr),'_blank');````

#### RHS Hort Database:

- No hybrid symbols
- No quotes for cultivar names
- Replaces space with ' and '
- Adds the first word of the query as the search genus

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/×/g,'').replace(/['‘’]/g,'').replace(/\s+/g,' and ');if(Qr)window.open('http://apps.rhs.org.uk/horticulturaldatabase/summary2.asp?crit='+encodeURIComponent(Qr)+'&genus='+Qr.match(/\w+/),'_blank');````

#### MOBOT Plant Finder:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/×/g,'x');if(Qr)window.open('http://www.missouribotanicalgarden.org/PlantFinder/PlantFinderProfileResults.aspx?adv='+encodeURIComponent(Qr),'_blank');````

#### NGA Plants database:

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('https://garden.org/plants/search/text/?q='+encodeURIComponent(Qr),'_blank');````

#### NY Flora Atlas

- No space after hybrid symbols

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x | × /g,' ×');if(Qr)window.open('http://newyork.plantatlas.usf.edu/Results.aspx?q='+encodeURIComponent(Qr),'_blank');````

#### Plants for a Future:

- Replace ' × ' with ' x ' in search query

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/×/g,'x');if(Qr)window.open('http://pfaf.org/user/Plant.aspx?LatinName='+encodeURIComponent(Qr),'_blank');````

#### The Plant List:

- Remove hybrid symbols

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x | × /g,' ');if(Qr)window.open('http://www.theplantlist.org/tpl1.1/search?q='+encodeURIComponent(Qr),'_blank');````

#### USDA Plants:

- No space after hybrid symbols

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x | × /g,' ×');if(Qr)window.open('http://plants.usda.gov/java/nameSearch?mode=sciname&keywordquery='+encodeURIComponent(Qr),'_blank');````

#### World Flora Online

````javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('http://www.worldfloraonline.org/search?query='+encodeURIComponent(Qr),'_blank');````

### Credits

These bookmarklets were inspired by Kew's ePIC [browser button](http://epic.kew.org/tbutton.htm), using update JavaScript
