**Before starting your translation, make sure it is not exists already!**

Check all commited language files [here](http://transmisson-remote-gui.googlecode.com/svn/trunk/lang/). Also check pending language files [here](http://code.google.com/p/transmisson-remote-gui/issues/detail?id=385).

Transmission Remote GUI language files are stored in the **`lang`** subfolder in the program's installation folder (or inside the application bundle on Mac OS X).

To create a new translation make a copy of the **`transgui.template`** file in the **lang** folder and rename the file copy to **`transgui.xx`** (where xx is a language code: **`fr`** - for French, **`it`** - for Italian, **`es`** - for Spanish, etc). Open the language file in a text editor, which can edit files in **UTF-8 encoding**. Set the **`TranslationLanguage`** parameter to the localized name of your language. Translate all strings.
To test your translation, run the program and choose your language in the program's options.

Post the finished translation on **[this page](http://code.google.com/p/transmisson-remote-gui/issues/detail?id=385)** page and it will be included in the next release of Transmission Remote GUI.

For example, here is a part of the Russian language file **`transgui.ru`**:

<pre>
TranslationLanguage=Русский<br>
About=О программе<br>
Active=Активные<br>
Add new torrent=Добавление нового торрента<br>
Add torrent=Добавить торрент<br>
Added on=Добавлен<br>
All=Все<br>
</pre>