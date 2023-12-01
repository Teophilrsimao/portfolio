---
Title: Load
---

Laddningstid
=======================


<style>
    table, th, td{
        border: 1px solid black;
    }

    th, td{
        padding: 15px;
        text-align: left;
        border-collapse: collapse;
    }

    .nob {
        border: none;
    }

    .column {
        float: left;
        width: 50%;
        padding: 10px;
    }


    .row:after {
        content: "";
        display: table;
        clear: both;
    }

    @media screen and (max-width: 850px) {
        .column {
            width: 100%;
            float: none;
        }
    }
</style>

Syftet med denna rapport är att undersöka och utvärdera webbplatsers laddningstid och användbarhet. Målet är att identifiera förbättringsområden och föreslå åtgärder för att optimera prestanda samt förbättra användarupplevelsen.

#  

Urval
-----------------------
Webbplatserna som ska undersökas är: <a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a>, <a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a> och <a href="https://kelseydake.com/" target="_blank">KelseyDake</a>. Urval av sidorna beror till stor del på att sidorna har redan undersökts när det gäller färgaspekten. Alla dem tre sidor innehåller dessutom väldigt mycket material såsom bilder och video. Med tanke på detta blir det spännade att testa och utvärdera deras laddningstid och användbarhet. 

#  

Metod
-----------------------
För att samla in data använde jag mig av <a href="https://pagespeed.web.dev/">Google PageSpeed Insights</a> för att ta fram och mäta prestanda för både Mobile och Desktop. Jag änvände mig även av Firefox/Chrome devtools för att analysera nätverksprestanda på tre olika sidor på varje webbplats. Och själva resultaten dokumenterades i Google Kalkylark.

#  

Resultat
-----------------------
### <a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a>
![Leaf](%base_url%/image/golfspace.jpg)
<div class="row">
    <div class="column">
        <table>
            <h5>PageSpeed Insights</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://www.golfspace.com.au/" target="_blank">Sida-1</a></th>
                <th><a href="https://www.golfspace.com.au/indoor-virtual-golf-simulator/" target="_blank">Sida-2</a></th>
                <th><a href="https://www.golfspace.com.au/play/" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Mobile</th>
                <td>27</td>
                <td>31</td>
                <td>36</td>
            </tr>
            <tr>
                <th>Desktop</th>
                <td>63</td>
                <td>70</td>
                <td>70</td>
            </tr>
        </table>
    </div>
    <div class="column">
        <table>
            <h5>DevTools</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://www.golfspace.com.au/" target="_blank">Sida-1</a></th>
                <th><a href="https://www.golfspace.com.au/indoor-virtual-golf-simulator/" target="_blank">Sida-2</a></th>
                <th><a href="https://www.golfspace.com.au/play/" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Resurser</th>
                <td>129</td>
                <td>101</td>
                <td>97</td>
            </tr>
            <tr>
                <th>Storlek</th>
                <td>26.4 mb</td>
                <td>6.3 mb</td>
                <td>6.0 mb</td>
            </tr>
            <tr>
                <th>Laddningstid</th>
                <td>13.68 s</td>
                <td>5.6 s</td>
                <td>5.1 s</td>
            </tr>
        </table>
    </div>
</div>

#  

<a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a> kan förbättras genom att man minskar anatalet begäran genom att minimera och kombinera JS- och CSS-filer, samt att bilder komprimeras för att minska sidans totala storlek.

#  

### <a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a>
![Leaf](%base_url%/image/besthorrorscenes.jpg)
<div class="row">
    <div class="column">
        <table>
            <h5>PageSpeed Insights</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-1</a></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-2</a></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Mobile</th>
                <td>38</td>
                <td>29</td>
                <td>12</td>
            </tr>
            <tr>
                <th>Desktop</th>
                <td>52</td>
                <td>62</td>
                <td>68</td>
            </tr>
        </table>
    </div>
    <div class="column">
        <table>
            <h5>DevTools</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-1</a></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-2</a></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Resurser</th>
                <td>92</td>
                <td>91</td>
                <td>91</td>
            </tr>
            <tr>
                <th>Storlek</th>
                <td>5.0 mb</td>
                <td>4.9 mb</td>
                <td>4.9 mb</td>
            </tr>
            <tr>
                <th>Laddningstid</th>
                <td>2,44 s</td>
                <td>2,44 s</td>
                <td>2,44 s</td>
            </tr>
        </table>
    </div>
</div>

#  

<a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a> kan förbättras genom att man slår ihop och minskar CSS- och JS-filer, samt att man minskar onödiga filer och optimerar bilder för att minska sidans storlek.

# 

### <a href="https://kelseydake.com/" target="_blank">KelseyDake</a>
![Leaf](%base_url%/image/kelseydake.jpg)
<div class="row">
    <div class="column">
        <table>
            <h5>PageSpeed Insights</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://kelseydake.com/" target="_blank">Sida-1</a></th>
                <th><a href="https://kelseydake.com/?tag=People" target="_blank">Sida-2</a></th>
                <th><a href="https://besthorrorscenes.com/" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Mobile</th>
                <td>33</td>
                <td>37</td>
                <td>34</td>
            </tr>
            <tr>
                <th>Desktop</th>
                <td>37</td>
                <td>53</td>
                <td>58</td>
            </tr>
        </table>
    </div>
    <div class="column">
        <table>
            <h5>DevTools</h5>
            <tr>
                <th class="nob"></th>
                <th><a href="https://kelseydake.com/" target="_blank">Sida-1</a></th>
                <th><a href="https://kelseydake.com/?tag=People" target="_blank">Sida-2</a></th>
                <th><a href="https://kelseydake.com/?tag=Animation" target="_blank">Sida-3</a></th>
            </tr>
            <tr>
                <th>Resurser</th>
                <td>137</td>
                <td>127</td>
                <td>121</td>
            </tr>
            <tr>
                <th>Storlek</th>
                <td>76.5 mb</td>
                <td>74 mb</td>
                <td>68.8 mb</td>
            </tr>
            <tr>
                <th>Laddningstid</th>
                <td>8,36 s</td>
                <td>10,15 s</td>
                <td>20,83 s</td>
            </tr>
        </table>
    </div>
</div>

#  

<a href="https://kelseydake.com/" target="_blank">KelseyDake</a> kan förbättras genom att man slår ihop och minskar CSS- och JS-filer, samt att man minskar onödiga filer och optimerar bilder för att minska sidans storlek. Och även genom optimering av resurscaching.

#  

Analys
-----------------------
Baserad för resultatet för <a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a>, <a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a> och <a href="https://kelseydake.com/" target="_blank">KelseyDake</a> så jag insett att dem vanliga åtgärgder som kan implementeras för att förbättra en webbplats prestanda är att komprimerar bilder så att överföringstiden kan minskas, att man minskar HTTP-begäran genom att slå ihop och minimera CSS- och JS-filer och att man implementerar resurscachning så att så att filer kan lagras lokalt på besökarens enhet.

#  

### Rangordning av resultat

<ul>
    <li> <a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a>
        <ul>
            <li>Resurser: 92, Storlek: 5.0 mb, Laddningstid: 2.44 s</li>
        </ul>
    </li>
    <li> <a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a>
        <ul>
            <li>Resurser: 129, Storlek: 26.4 MB, Laddningstid: 13.68 s</li>
        </ul>
    </li>
    <li> <a href="https://kelseydake.com/" target="_blank">KelseyDake</a>
        <ul>
            <li>Resurser: 137, Storlek: 76.5 MB, Laddningstid: 8.36 s</li>
        </ul>
    </li>
</ul>

#  

<h5>Kommentar</h5>

Som vi kan se så är <a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a> vinnaren i testet, enligt mig så beror det på att det här den sida som gör minst HTTP-begäran av alla tre sidor och den har minsta storleken.

#  

<h5>Laddningstid</h5>

Enligt mig så är gränsen för en anabb hemsidas absolut laddningstid 4 s, tar det längre än så så kanske man ska man försöka och göra lite optimering på sidan. 

#  
<a href="https://besthorrorscenes.com/" target="_blank">BestHorrorSpace</a> klarade gränsvärdet utan problem. medans <a href="https://www.golfspace.com.au/" target="_blank">GolfSpace</a> och <a href="https://kelseydake.com/" target="_blank">KelseyDake</a> låg väldigt långt ifrån det. Vilket gjorde att det blev lite jobbigt att navigerar igenom sidorna.

#  

<div class="embed-container">
    <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRjfPr9Z7yg3SYmDlIBa4KYnIX1vJdLVaKES_mLQiUPVgTwPmDB-rfb4AYWtfdX5yqmoxDbJINRrHsR/pubhtml?widget=true&amp;headers=false"></iframe>
</div>

#  
Referenser
-----------------------

<a href="https://moz.com/learn/seo/page-speed">Moz om Page Speed</a>

#  

Övrigt
-----------------------

skribent:<em>Teophil Ricardo Simao</em>
