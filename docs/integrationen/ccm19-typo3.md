# Typo3

Um unseren Cookie [Consent](https://www.ccm19.de/integration/glossar/10-Consent.html#10) Manager für Ihre Typo3-Seite zu installieren, führen Sie einfach die folgenden Schritte aus:

## Dashboard in CCM19 anwählen

Nach der erfolgreichen Installation von CCM19 auf Ihrem Server bzw. der Einrichtung bekommen Sie einen Javascript-Code.

![CCM19 Backend Screen](../assets/10-01.png)

## Typo3 Backend

Anschließend, melden Sie sich normal im Typo3 Backend an. Dort angekommen, öffnen Sie den Menüpunkt "Template".

Im Menüpunkt "Template", öffnen Sie das Template, was derzeit für Ihrer Webseite aktiv ist.

In diesem Template angekommen, bearbeiten Sie das Setup.

In dem Setup fügen Sie nun folgenden Code ein (Achtung: Dieser Code kann mit verschiedenen Typo3 Version nicht korrekt sein):

```html
page.headerData.1 = TEXT
page.headerData.1.value (
    <script src="https://www.lsb-sportmanagement.de/ccm19/public/ccm19.js?apiKey=8a2eeaf1c09cf6dee716f99f56ac8b19e8f696a289827c2a&amp;domain=96d3b6a&amp;lang=de_DE" referrerpolicy="origin"></script>
)
```

Nun speichern Sie diese Änderung einfach und leeren den Cache Ihrer Typo3 Seite.

Damit ist die Einrichtung abgeschlossen und CCM19 sollte nun in Ihrem Shop aktiv sein.