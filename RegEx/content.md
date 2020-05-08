# Inhalsverzeichnis
1. Was sind Regex?
    1. generelles
    2. Syntax (Verweis auf Übersicht)
        https://www.debuggex.com/cheatsheet/regex/pcre
    3. Relevanz?
2. re Modul
    1. import
    2. Methodenübersicht
        1. search/match/matchall (Unterschied)
        2. findall/finditer (Unterschied)
            - aus E-Mail-Adressen Namen/vorderen Teil extrahieren
        3. split
            - Text an beliebige Whitespace aufspalten
        4. sub
            - Pseudonymisierung von E-Mails (mit RegEx von oben E-Mails durch \<E-Mail\> oder so ersetzen)
    3. compile()/Unterschied im Gebrauch
    4. Capture Groups
        - URL in Teile zerlegen (http://sub.test.de/bla/blubb -> [['http'], ['sub', 'test'], ['de'], ['bla', 'blubb']])
    5. lazy/greedy Matching
        - Klammerstrukturen wie XML-Tags richtig erkennen/bereinigen
    6. lookaround?
        - Text an Whitespace aufspalten, der auf ein Satzzeichen folgt
3. Anwendungen/Übungen
    1. Mentions, Hashtags, URLs aus Twitterdaten extrahieren (Twitter-Input-Modul)
        - liste an Mentionts, Hashtags, URLs im tweet
    2. Datenbereinigung (XML-Tags mit greedy/lazy)(HTML-Input-Modul)
        - Input sind HTML-Schnippsel
        - HTML-Tags werden herausgefiltert
    3. Grep/Suchfunktion
        - alle Vorkommnisse einer gegebenen RegEx werden in einem gegebenen Text hervorgehoben ausgegeben
    4. Tokenizer
        - Wörter
        - Zahlen
        - Satzzeichen werden abgespaltet
        - URLs, E-Mail-Adressen, Twitter-Mentions/-Hashtags werden nicht zerlegt
4. Ausblick/weiterführende Links
    1. weitere Bibliotheken (z.B. regex, pyre2)