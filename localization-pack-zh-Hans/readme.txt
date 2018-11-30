中文汉化说明：

想要贡献翻译的朋友可以访问 https://paratranz.com/projects/119
会定期将文本同步至 GitHub
另外也可以加入QQ群 950675466

ParaTranz 是一个公开的汉化平台，当前主要是用于汉化 Paradox 出品的游戏，如王国风云2、欧陆风云4、钢铁雄心4及群星等游戏的汉化平台社区，现已有52汉化组、星海续命录翻译组、牧有汉化组及一些P社相关游戏Mod的汉化组和个人入驻，平台理论上也可以用于汉化其他任何游戏。

==========================

What do the data look like?
The localization table is saved in plain text (XML) files, organized into different categories that make sense, for example:


    Texts in the menu and main user interface
    Medical terms - diagnoses
    Medical terms - examinations
    Texts for tutorials and campaign
    ...
    Names and descriptions of objects you can build


This will allow more people to translate one language.
The game directly reads these XML files, so it's possible to test the changes in the game without sending the files to the developers and waiting for a new version.

File heading
============
This is an example for Czech. Each file has to have a unique ID (change language code!). Values that need to be filled in each file are the language code in lower case (like en, fr, pt_br etc) and localized name (that's what will show in game).
Feel free to add you name to the list of contributors for any file you've made changes to!

<Database>
    <GameDBStringTable ID="LOC_CZ_ACHIEVEMENTS">

        <LanguageCode>cz</LanguageCode>
        <LanguageNameLocalized>Čeština</LanguageNameLocalized>

        <Contributors>
            <Name>Oxymoron Games</Name>
        </Contributors>


Some examples of the texts
==========================

    <GameDBLocalizedString>      <LocID>CANCEL</LocID>                    <Text>Cancel</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>OCCUPATION_DOCTOR</LocID>         <Text>Doctor</Text>  </GameDBLocalizedString>
    <GameDBLocalizedString>      <LocID>OCCUPATION_NURSE</LocID>          <Text>Nurse</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>DIA_FLU1_DESCRIPTION</LocID>      <Text>Influenza is a common infectious disease caused by ...</Text>  </GameDBLocalizedString>


There are some formatting options available:
New line: \n
Bold/italics:

    <![CDATA[Now <b><i>do something</i></b>.\nThis is on the next line.]]>
