# Simple document search engine 
Searching through Wikipedia dump files

Wikipedia document starts with
```sh
<doc id="9160" url="https://en.wikipedia.org/wiki?curid=9160" title="De jure">
```    
and ends with 
```sh
</doc>
```
This simple implementation uses [term frequency–inverse document frequency](https://en.wikipedia.org/wiki/Tf-idf).

The script loads Wikipedia dump files into a corpus (dictionary) and searches can be done subsequently. Multiple dumps can be loaded. A search in the corpus returns only files containing ALL the keywords given and list the result in order of relevance (more relevant first).
