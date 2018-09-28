
What do the data look like?
The localization table is saved in plain text (XML) files, organized into different categories that make sense, for example:


    Texts in the menu and main user interface
    Medical terms used in emergency department
    Medical terms used in orthopaedics department
    ...
    Names and descriptions of objects you can build


This will allow more people to translate one language.
The game directly reads these XML files, so it's possible to test the changes in the game without sending the files to the developers and waiting for a new version.

Some examples of the texts - the bold texts are the actual part to translate:

    <GameDBLocalizedString>      <LocID>CANCEL</LocID>                    <Text>Cancel</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>OCCUPATION_DOCTOR</LocID>         <Text>Doctor</Text>  </GameDBLocalizedString>
    <GameDBLocalizedString>      <LocID>OCCUPATION_NURSE</LocID>          <Text>Nurse</Text>  </GameDBLocalizedString>

    <GameDBLocalizedString>      <LocID>DIA_FLU1_DESCRIPTION</LocID>      <Text>Influenza is a common infectious disease caused by ...</Text>  </GameDBLocalizedString>


There are some formatting options available:
New line: \n 
Bold/italics:

    <![CDATA[Now <b><i>do something</i></b>.\nThis is on the next line.]]>
