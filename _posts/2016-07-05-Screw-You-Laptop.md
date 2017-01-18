---
layout:     post
title:      "Screw you laptop!"
subtitle:   " Literally!"
date:       2016-07-05 09:37:00
author:     "Shikher Verma"
header-img: "img/posts/screw-laptop-bg.jpg"
comments: true
tags: [ CodeMonkey, Robotics ]
---
<pre>
Данный код производит условие 
<!--условие хит распродажа-->
   <div class="tovar_img" >
     <img src="<?=$arResult["PREVIEW_PICTURE"]["UNSAFE_SRC"]?>" />
<?if ($arResult['PROPERTIES']['HIT']['VALUE'] == 'Y' ):?>
	<span class="tovars_marker reds" >hit</span>
<?elseif ($arResult['PROPERTIES']['SALE']['VALUE'] == 'Y'):?>
<span class="tovars_marker yellow" >sale</span>
<?endif;?>
	</div>						
								
<!--Подсчет элементов-->								
<h2 class="block_content_head" >Сравнение товаров<span>показано  <?=count($arResult["ITEMS"])?> из <?=count($arResult["ITEMS"])?> товаров</span></h2>
<!--Ограничение по символам в анонсе-->
<?echo TruncateText($arItem["PREVIEW_TEXT"], 130); ?>
	
</pre>
