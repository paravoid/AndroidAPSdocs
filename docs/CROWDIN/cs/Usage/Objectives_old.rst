Objectives as of Android APS 2.8.2.1
**************************************************
This is not the latest version of the Android APS Objectives.  This page details the Objectives that were in place prior to version 3.0.  Anyone using an older version of Android (i.e. prior to Android 9) and Android APS version 2.8.2.1 should refer to this page.  

Please see `this page <../Usage/Objectives.html>`_ for the current set of Objectives.

AndroidAPS má sadu Cílů, které musíte dokončit a které vás provedou jeho funkcemi a nastaveními tak, aby pro vás smyčka nebyla nebezpečná.  Zajistí vám, že jste nastavili všechny detaily z dříve uvedených sekcí správně, že rozumíte tomu, co váš systém dělá a proč, a že mu můžete důvěřovat.

Pokud měníte telefon, můžete si `exportovat své nastavení <../Usage/ExportImportSettings.html>`_ a váš postup (již splněné cíle) bude zachován. Kromě vašeho postupu se exportem/importem uloží řada jiných nastavení, například vaše bezpečnostní nastavení jako maximální bolus apod.  Pokud neabsolvujete export/import svých nastavení, pak budete muset začít plnit cíle znovu od začátku.  Je dobrý nápad `zálohovat Vaše nastavení <../Usage/ExportImportSettings.html>`_ často jen tak pro jistotu.

Pokud se chcete v cílech vrátit zpět, podívejte se na vysvětlení pod <../Usage/Objectives.html#go-back-in-objectives>`_.
 
Cíl 1: Nastavit vizualizaci a monitoring, analyzovat bazály a poměry
====================================================================================================
* Zvolte správný zdroj glykémie pro svou kombinaci zařízení.  Více informací viz `Zdroj glykémií <../Configuration/BG-Source.html>`_.
* Vyberte správnou pumpu na kartě Konfigurace (zvolte Virtuální pumpu, pokud používáte model pumpy bez ovladače v AndroidAPS – pouze pro otevřenou smyčku) a na kartě pumpy ověřte, že váš model pumpy dokáže komunikovat s aplikací AndroidAPS a přenášet do ní svůj stav.  
* Pokud používáte pumpu DanaR, ujistěte se, že jste postupovali podle pokynů v části `Inzulinová pumpa DanaR <../Configuration/DanaR-Insulin-Pump.html>`_ a že je propojená s AndroidAPS.
* Postupujte podle pokynů na stránce `Nightscout <../Installing-AndroidAPS/Nightscout.html>`_ a ověřte, že Nightscout může přijímat a zobrazovat tato data.
* Všimněte si, že adresa URL v NSClientu musí být ** BEZ /api/v1 /** na konci - viz `Nastavení NSClientu v předvolbách <../Configuration/Preferences.html#nsclient>`__.

*Možná bude nutné počkat na další odečet glykémie, než AndroidAPS změnu zaregistruje.*

Cíl 2: Naučte se ovládat AndroidAPS
==================================================
* Proveďte několik akcí v AndroidAPS, jak je popsáno v tomto cíli.
* Pro přístup k úkolům klikněte na oranžový text „Nedokončeno“.
* Odkazy budou poskytnuty jako vodítko pro případ, že dosud nejste obeznámeni se specifickou akcí.

  .. image:: ../images/Objective2_V2_5.png
    :alt: Screenshot cíl 2

Cíl 3: Prokázat své znalosti
==================================================
* Správně zodpovězte otázky s výběrem možných odpovědí a prokažte znalost AndroidAPS.
* Klikněte na oranžový text „Nedokončeno“ pro přístup na stránku s otázkou a možnými odpověďmi.

  .. image:: ../images/Objective3_V2_5.png
    :alt: Screenshot cíl 3

* Odkazy budou poskytnuty jako vodítko pro případ, že si nejste jisti odpovědí.
* Otázky pro cíl 3 byly od AAPS verze 2.8 kompletně přepsány rodilými mluvčími. Nové otázky pokrývají stejná témata a několik nových.
* Tyto nové otázky způsobí, že budete mít nezodpovězené otázky v cíli 3, přestože jste již dříve cíl 3 úspěšně dokončili.
* Nezodpovězené otázky budou mít na vás vliv pouze pokud budete startovat nový cíl. Jinými slovy: Pokud jste již dokončili všechny cíle, můžete počkat a odpovědět na nové otázky později bez ztráty funkcí AAPS.

Cíl 4: Začít s otevřenou smyčkou
==================================================
* Vyberte možnost Otevřená smyčka buď v Nastavení, nebo stisknutím a podržením tlačítka Smyčka v levém horním rohu hlavní obrazovky.
* Projděte si `Nastavení <../Configuration/Preferences.html>`_ a nastavte je tak, jak potřebujete.
* Ručně nařiďte alespoň 20 dočasných bazálních dávek, které vám systém navrhuje, a to během 7 dní; zadejte je do své pumpy a potvrďte v AndroidAPS, že jste návrhy přijali.  Ujistěte se, že se tyto údaje zobrazí v AndroidAPS a Nightscoutu.
* Povolte `dočasné cíle <../Usage/temptarget.html>`_ pokud je to nutné. Použijte dočasný cíl Hypoglykémie, abyste systému zabránili v příliš agresivních korekcích, pokud by glykémie po vyřešení hypoglykémie stoupala. 

Snížení počtu oznámení
--------------------------------------------------
Pro snížení počtu rozhodnutí, která mají být provedena v režimu otevřené smyčky, nastavte cílový rozsah na 90–150 mg/dl nebo 5,0–8,5 mmol/l.
* Možná budete chtít v noci zvýšit horní limit (nebo zakázat otevřenou smyčku). 
* V Předvolbách můžete nastavit minimální procento navrhované změny bazální dávky.

  .. image:: ../images/OpenLoop_MinimalRequestChange2.png
    :alt: Minimální změna pro požadavek Open Loop
     
* Navíc, nemusíte reagovat každých 5 minut na všechna doporučení…

Cíl 5: Porozumění otevřené smyčce, včetně doporučení pro dočasné bazály
====================================================================================================
* Začněte chápat úvahy, které vedou k doporučení dočasných bazálních dávek, tím, že si projdete `logiku <https://openaps.readthedocs.io/en/latest/docs/While%20You%20Wait%20For%20Gear/Understand-determine-basal.html>`_ a budete sledovat graf předpovědí na `domovské obrazovce AndroidAPS <../Getting-Started/Screenshots.html#prediction-lines>`_/ v Nightscoutu. Také si v aplikaci procházejte výstupy z výpočtů na záložce OpenAPS.
 
Cíl nastavte o něco výše než obvykle, dokud si nebudete jisti správností výpočtů a nastavení.  Systém umožňuje

* dolní cílová hodnota musí být minimálně 4 mmol (72 mg/dl) nebo nejvýše 10 mmol (180 mg/dl) 
* horní cílová hodnota musí být minimálně 5 mmol (90 mg/dl) nebo nejvýše 15 mmol (225 mg/dl)
* dočasný cíl jako jediná hodnota může být kdekoliv mezi 4 až 15 mmol (72 mg/dl až 225 mg/dl)

Cíl je hodnota, o kterou se opírá kalkulace, nikoliv hodnota, na které byste chtěli svou glykémii držet.  Pokud je váš cíl velmi široký (řekněme 3 nebo více mmol široký), často se objeví pouze málo AAPS akcí. To je proto, že predikovaná glykémie bude někde v tomto širokém rozmezí a proto není doporučováno mnoho dočasných bazálů. 

Můžete zkusit experimentovat a nastavit své cíle tak, aby nebyl rozptyl hodnot přílš velký (řekněme 1 mmol / 20 mg/l nebo méně) a přitom sledujte, jak se tím chování systému mění.  

Na grafu můžete zobrazit širší rozsah (zelené čáry) pro hodnoty, v nichž chcete udržet hladinu glukózy v krvi, zadáním různých hodnot do `Předvoleb <../Configuration/Preferences.html>`__ > Rozsah pro zobrazení.
 
.. image:: ../images/sign_stop.png
  :alt: Znaménko Stop

Zastavte se zde, pokud používáte otevřenou smyčku s virtuální pumpou – neklikejte na tlačítko Zkontrolovat na konci tohoto cíle.
------------------------------------------------------------------------------------------------------------------------------------------------------

.. obrázek:: ../images/blank.png
  :alt: prázdný

Cíl 6: Začátek uzavřené smyčky - s pozastavením pumpy při nízké glykémii
====================================================================================================
.. image:: ../images/sign_warning.png
  :alt: Varování
  
U 6. cíle nebude uzavřená smyčka korigovat vysokou glykémii, bude pouze zastavovat před nízkou. Na vysoké glykémie musíte ručně dopíchnout vy sami!
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
* Vyberte Uzavřená smyčka buď z `Nastavení <../Configuration/Preferences.html>`_, nebo stisknutím a přidržením tlačítka Otevřená smyčka z pravého horního rohu hlavní stránky.
* Nastavte cílový rozsah mírně vyšší, než který je pro vás běžný, jen pro jistotu.
* Sledujte, jak jsou aktivní dočasné bazální dávky buď prohlížením modrého textu bazálu na hlavní stránce anebo v modrém vykreslení bazálů na grafu.
* Ujistěte se, že AndroidAPS je teď nastavený tak, že po dobu 5 dní nemusíte řešit nízké glykémie.  Pokud stále řešíte časté nebo vážné výskyty nízkých glykémií, zvažte úpravu svého DIA, bazálů, citlivosti a sacharidových poměrů.
* Nemusíte měnit své nastavení. Při plnění cíle 6 je maxIOB nastaveno automaticky na nulu. Toto nastavení bude při přechodu na cíl 7 odstraněno.
* Systém přepíše vaše nastavení maxIOB na nulu, což znamená, že pokud glykémie klesá, může snížit bazál, ale pokud glykémie stoupá, pak zvýší bazál pouze v případě, že IOB je záporný (z předchozího sníženého bazálu nebo zastavené pumpy), jinak hodnoty bazálu budou stejné jako ty nastavené v profilu.  

  .. image:: ../images/Objective6_negIOB.png
    :alt: Příklad negativního IOB

* If your basal IOB is negative (see screenshot above) a TBR > 100% can be issued also in objective 6.
* Bez možnosti zvýšit bazál při srovnání křivky glykémie se vám dočasně může stávat, že po vyřešení hypoglykémie bude následovat přílišný vzestup glykémie.

Cíl 7: Vyladit uzavřenou smyčku, zvyšovat max IOB nad 0 a postupně snižovat cílovou glykémii
====================================================================================================
* Zvyšte hodnotu 'Maximální celkový IOB, který OpenAPS nemůže překročit' (v OpenAPS se tento parametr označuje jako 'max-iob') nad 0 po dobu 1 dne. Výchozím doporučením je použít "průměrnou hodnotu bolusu k jídlu + 3× maximální denní bazální dávku" (pro algoritmus SMB) nebo "3× maximální denní bazální dávku" (pro starší algoritmus AMA). Tyto hodnoty byste však měli zvyšovat postupně, dokud neověříte, že jsou nastaveny správně (maximální denní bazální dávka = maximální bazální dávka za hodinu během dne).

  Toto doporučení by mělo být považováno za výchozí bod. Pokud ho nastavíte na 3x a uvidíte kroky, které vás rychle stahují dolů, pak snižte toto číslo. Pokud jste velmi rezistentní na inzulín, pomalu ho zvyšujte.

  .. image:: ../images/MaxDailyBasal2.png
    :alt: max denní bazál

* Až si budete jistí množstvím IOB, které sedí vašemu vzoru smyčky, pak snižte své cílové glykémie na požadovanou úroveň.


Cíl 8: Upravit bazály a poměry, když bude potřeba, a povolit automatickou detekci citlivosti na inzulín
====================================================================================================
* Pro kontrolu správnosti nastavení bazálu můžete použít `autotune <https://openaps.readthedocs.io/en/latest/docs/Customize-Iterate/autotune.html>`_, nebo si udělejte klasický test bazálu.
* Povolte <a href="../Usage/Open-APS-features.md">automatickou detekci citlivosti</a> po dobu 7 dní a sledujte bílou křivku na grafu na hlavní stránce, jak se vaše citlivost na inzulín může snižovat a zvyšovat v důsledku cvičení nebo hormonů apod. Při tom sledujte na kartě OpenAPS výslednou zprávu, jak podle toho systém AndroidAPS upravil vaše bazály a/nebo cíle. a sledujte na záložce zpráv OpenAPS, jak AndroidAPS odpovídajícím způsobem upravuje bazály a/nebo cíle.

*Nezapomeňte zaznamenat své zkušenosti se smyčkou do* `tohoto formuláře <https://bit.ly/nowlooping>`_ *a označte tam AndroidAPS jako váš typ DIY softwaru uzavřené smyčky, pokud jste tak ještě neučinili.*


Objective 9: Try additional features for daytime use and gain confidence in your closed loop system
====================================================================================================
* Before AAPS version 2.7 meal assist (MA) was the basic algorithm for AAPS and completing objective 8 was necessary to activate `advanced meal assist (AMA) <../Usage/Open-APS-features.html#advanced-meal-assist-ama>`__.
* As `advanced meal assist (AMA) <../Usage/Open-APS-features.html#advanced-meal-assist-ama>`__ is the standard algorithm from AAPS version 2.7 onwards use the following 28 days to try features you haven't used yet and get more confident with you closed loop system.


Objective 10: Enabling additional oref1 features for daytime use, such as super micro bolus (SMB)
====================================================================================================
* Musíte si přečíst `Kapitolu o SMB zde na wiki<../Usage/Open-APS-features.html#super-micro-bolus-smb>`_ a `Kapitolu oref1 v dokumentaci k openAPS <https://openaps.readthedocs.io/en/latest/docs/Customize-Iterate/oref1.html>`_, abyste porozuměli tomu, jak SMB funguje, zejména na čem stojí princip nulových dočasných bazálů.
* Následně byste měli `zvýšit maxIOB <../Usage/Open-APS-features.html#maximum-total-iob-openaps-cant-go-over-openaps-max-iob>`_ tak, aby SMB správně fungovaly. maxIOB nyní zahrnuje veškerý IOB, nejen ten z bazálů. To znamená, že pokud byl vydán bolus 8 U na jídlo a maxIOB je 7 U, nebudou vydány žádné SMB, dokud IOB neklesne pod 7 U. Pro začátek je dobré nastavit hodnotu maxIOB jako „průměrný bolus k jídlu + 3× maximální denní bazální dávka“ (maximální denní bazální dávka = maximální bazální dávka za hodinu během dne – např. viz `<../Usage/Objectives2019.html#objective-7-tuning-the-closed-loop-raising-max-iob-above-0-and-gradually-lowering-bg-targets>Cíl 7`_)
* Výchozí hodnota absorpce „min_5m_carbimpact“ se při přechodu z AMA na SMB mění ze 3 na 8. Přecházíte-li z AMA na SMB, musíte to změnit ručně.


Objective 11: Automation
====================================================================================================
* You have to start objective 11 to be able to use `Automation <../Usage/Automation.html>`_.
* Ujistěte se, že jste splnili všechny zkoušky v cíli 3 `<../Usage/Objectives.html#cil-3-prokazat-sve-znalosti>`_.
* Dokončení předchozích cílů nebude mít vliv na další cíle, které jste již dokončili. Splněné cíle zůstanou zachovány!


Návrat k předchozímu cíli
====================================================================================================
Chcete-li se z jakéhokoliv důvodu vrátit k předchozímu cíli, stačí tak učinit kliknutím na „vymazat dokončené“.

.. image:: ../images/Objective_ClearFinished.png
  :alt: Návrat zpět
