Using our WordPress plug-in is very simple. Please use the sidesparks.php file.

There you can modify line 11-14:

$show_on_main_page = false; Do you want the SideSparks link to be placed on the main page?
$show_on_category = true; Or only in the articles?
$timeOffset = "1"; Please set your timezone here. For an overview click here.

If you want to modify the link to SideSparks Tagged Chat please change this line:
$sidesparksInitLink = '<img src = "http://channels.sidesparks.com/discuss.png" style = "border: 0px;">';

Once you have done this, simply upload sidesparks.php to your WordPress plug-ins folder.

If you want to have a textlink "Discuss Now" displayed next to "x Comments" on the mainpage please search for:
<?php comments_popup_link('No Comments &#187;', '1 Comment &#187;', '% Comments &#187;');
in your template. (actually this should generate the "x Comments" link)
Before that just include: <? echo generateSidesparksLink("Discuss Now", false)." | "; ?>

If you want to edit the button please feel free to modify our button with Photoshop: http://sidesparks.com/sidesparks_psd.zip
