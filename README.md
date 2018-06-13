# OpenText.org annotation of Various Non-NT Texts

* These are various bits of annotation applied to non-NT texts at various times in the project's history

* Initial commit has texts _as is_ using the original namespaced XML vocabulary. For example:

```
<?xml version="1.0" encoding="UTF-8"?>
<chapter book="Did" num="1">
    <cl:clause xmlns:cl="http://www.opentext.org/ns/clause" id="Did.c1_1" level="primary">
        <gloss>Two ways exist</gloss>
        <cl:S>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w1"/>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w2"/>
        </cl:S>
        <cl:P>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w3"/>
        </cl:P>
    </cl:clause>
    <cl:clause xmlns:cl="http://www.opentext.org/ns/clause" id="Did.c1_2" level="primary" connect="Did.c1_1">
        <gloss>one of life</gloss>
        <cl:S>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w4"/>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w5"/>
            <w xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="AF:Did.w6"/>
        </cl:S>
    </cl:clause>
 
    ...
```

and

```
<?xml version="1.0" encoding="UTF-8"?>
<chapter xmlns:wg="http://www.opentext.org/ns/word-group" xmlns:pl="http://www.opentext.org/ns/paragraph" xmlns:cl="http://www.opentext.org/ns/clause" xmlns:xlink="http://www.w3.org/1999/xlink" book="Did" num="1">
    <wg:groups>
        <wg:group id="AF:Did.wg1_188">
            <wg:head>
                <wg:word xlink:href="AF:Did.w1">
                    <wg:modifiers>
                        <wg:definer>
                            <wg:word xlink:href="AF:Did.w2"/>
                        </wg:definer>
                    </wg:modifiers>
                </wg:word>
            </wg:head>
        </wg:group>

   ...

```

* The annotation is incomplete (especially for word group level) but could be useful for future work and corpus building.

