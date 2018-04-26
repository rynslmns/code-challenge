
# SteelHouse Code Challenge

Please do not spend more than an hour on this challenge and focus on clear readable code. Good Luck!!

### Strip Url Params


Complete the method so that it does the following:
-- Removes any duplicate query string parameters from the url
-- Removes any query string parameters specified within the 2nd argument (optional array)
###### Examples:
#
```javascript
stripUrlParams('www.steelhouse.com?a=1&b=2&a=2') // returns 'www.steelhouse.com?a=1&b=2'
stripUrlParams('www.steelhouse.com?a=1&b=2&a=2', ['b']) // returns 'www.steelhouse.com?a=1'
stripUrlParams('www.steelhouse.com', ['b']) // returns 'www.steelhouse.com'
```

### Word Break
In some languages, (i.e. Chinese and Japanese) there are no word breaks between words. This makes building search engines for these languages more complex, as it's difficult to break search terms into individual words.

Your task is:
-- given a list of known words and a sentence with no spaces, break it into a list of known words. 
-- When you can't find a word list to make the sentence, you should return undefined.
-- If there are duplicates, just return one of them.

###### Examples:
#
```javascript
const dictWords = [
    "american","four","i","john","may","mr","mrs","us","united","a",
    "about","act","after","again","against","all","almost","along","also","always",
    "am","among","an","and","another","any","are","around","as","asked",
    "at","away","back","be","because","steel", "house", "become","been","before","began","best",
    "better","between","big","both","business","but","by","called","came","can",
    "case","certain","change","child","children","church","city","close","come","company",
    "could","country","course","day","days","development","did","didn't","do","does",
    "don't","done","down","during","each","early","end","enough","even","ever",
    "every","eyes","face","fact","family","far","feel","felt","few","find",
    "first","for","form","from","general","get","give","given","go","god",
    "going","good","got","govern","government","great","group","had","hand","has",
    "have","he","head","help","her","here","high","him","himself","his",
    "home","house","how","however","if","important","in","interest","into","is",
    "it","its","just","keep","kind","knew","know","large","last","later",
    "law","least","leave","less","let","life","light","like","line","little",
    "long","look","looked","made","make","man","many","matter","me","mean",
    "means","members","men","might","mind","more","most","much","must","my",
    "name","national","need","never","new","next","night","no","not","nothing",
    "now","number","of","off","often","old","on","once","one","only",
    "open","or","order","other","others","our","out","over","own","part",
    "people","per","place","point","possible","power","present","president","problem","program",
    "public","put","question","rather","real","right","room","said","same","say",
    "school","second","see","seem","seemed","sense","service","set","several","she",
    "should","show","side","since","small","so","social","some","something","state",
    "states","still","such","system","take","tell","than","that","the","their",
    "them","then","there","these","they","thing","things","think","this","those",
    "though","thought","three","through","time","to","told","too","took","toward",
    "turn","turned","two","under","unite","until","up","upon","use","used",
    "very","want","war","was","water","way","we","week","well","went",
    "were","what","when","where","which","while","white","who","why","will",
    "with","within","without","word","work","would","year","yet","you","young",
    "your"
  ];
  
wordBreak(dictWords, "steelhouse") // returns ["steel", "house"]
wordBreak(dictWords, "tobeornottobethatisthequestion") // returns ["to", "be", "or", "not", "that", "is", "the" "question"]
```
