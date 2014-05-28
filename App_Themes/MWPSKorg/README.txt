MWPSKorg Theme Guide


HOMEPAGE EDITING

As MWPSK display all the sections one after another inside a particular part of the theme (e.g. in the MWPSKorg theme, the sections are inserted in the <div id="home_content_container" style="float: left;">), to separate the contents of one HTML section you have to use some tricks with CSS. As the homepage in the MWPSKorg theme looks a bit different than the other themes, you have to pay attention on how to place the contents. Please read on.

Inside the HTML section (you have to create one, from the CMS Administration, if not done already) you have to insert different DIVs, as follows:


FAST AND EASY HOMEPAGE EDITING

To have an homepage with the same look and feel as the site www.mwpsk.org, just create an HTML Section in the Homepage (if not done already), edit it and switch from the "Design" mode to the "HTML" one. Copy and paste there the following HTML code, then save, have a look at it and modify it according to your needs. To understand exactly how does it work, please read on also chapters 1) 2) and 3).

<div class="3boxes">

<a href="#">
<div class="bottom_box box_use">
<h1>MWPSK<br></h1>
<p>Aliquam varius, neque nec mollis ultrices, sapien enim tincidunt dolor, 
et vehicula turpis quam nec justo. Vivamus in metus erat. Vivamus lacus 
arcu, luctus non dignissim quis, auctor id tortor. Cras volutpat aliquet
 imperdiet.<br></p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;">
<img id="imgArrowUse" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

<a href="#">
<div class="bottom_box box_develop">
<h1>ORG</h1>
<p>Nulla pretium nulla ac neque ultricies sed suscipit justo convallis. 
Nulla nec dolor erat, eget varius dolor. Integer metus metus, egestas ut
 fermentum vel, tincidunt eget justo. Vestibulum venenatis nunc non quam
 sagittis sodales.</p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;"><img id="imgArrowDev" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

<a href="#">
<div class="bottom_box box_contribute">
<h1>THEME</h1>
<p>Sed nec sem id ante rhoncus molestie. Maecenas tortor sapien, hendrerit 
at feugiat a, placerat vel velit. Integer sem magna, volutpat quis 
tempor sed, rutrum in sem.</p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;"><img id="imgArrowCont" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

</div><!--end 3 boxes-->

<div class="home_bottomText">

<h1>Welcome to the My Web Pages Starter Kit</h1>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus 
varius quam augue, sed placerat quam. Suspendisse pretium, metus eu 
consectetur varius, augue orci tincidunt justo, vitae pretium diam lorem
 in arcu.<br><br>Duis posuere diam nisl, vitae tempor felis. Aenean ut mi quis 
ligula congue consequat. Etiam vulputate sodales vulputate. Phasellus 
nibh augue, blandit ut bibendum in, consectetur et nisi.<br>Donec placerat,
 tortor id semper feugiat, ipsum sapien iaculis nibh, at consectetur 
libero augue at dolor. Integer sed lectus elit.<br>

</div><!--end home_bottomText-->



STEP BY STEP HOMEPAGE EDITING

1) Put contents inside the topBox

To edit the contents in the topBox you have to edit the Skin.skin file. Open it with your favorite Text or HTML editor.

Check the div with class="home_topBox". To edit just the contents, check and edit the contents of the div with class="home_topBox_contentText".

If you do not want the top box, just remove the div with class="home_topBox" and all its contents.


2) Add 3 colored boxes like in mwpsk.org

The theme comes with the boxes graphics and you can customize how they are placed by modifying the home.css file.
To have them like in mwpsk.org just insert (always using the HTML mode from the WYSIWYG editor in MWPSK) a DIV, as follows:

<div class="3boxes">

<a href="#">
<div class="bottom_box box_use">
<h1>MWPSK<br></h1>
<p>Aliquam varius, neque nec mollis ultrices, sapien enim tincidunt dolor, 
et vehicula turpis quam nec justo. Vivamus in metus erat. Vivamus lacus 
arcu, luctus non dignissim quis, auctor id tortor. Cras volutpat aliquet
 imperdiet.<br></p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;">
<img id="imgArrowUse" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

<a href="#">
<div class="bottom_box box_develop">
<h1>ORG</h1>
<p>Nulla pretium nulla ac neque ultricies sed suscipit justo convallis. 
Nulla nec dolor erat, eget varius dolor. Integer metus metus, egestas ut
 fermentum vel, tincidunt eget justo. Vestibulum venenatis nunc non quam
 sagittis sodales.</p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;"><img id="imgArrowDev" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

<a href="#">
<div class="bottom_box box_contribute">
<h1>THEME</h1>
<p>Sed nec sem id ante rhoncus molestie. Maecenas tortor sapien, hendrerit 
at feugiat a, placerat vel velit. Integer sem magna, volutpat quis 
tempor sed, rutrum in sem.</p>
<div class="bottombox_getmore">                                
<div class="getMoreText">Get More</div>
<div style="float: right;"><img id="imgArrowCont" src="App_Themes/MWPSKorg/_images/img_arrow.png"></div>                                 
</div>
</div>
</a>

</div><!--end 3 boxes-->


3) Add text after the 3 colored boxes.

To make things appear nicely, the home.css file has already a preconfigured style (feel free to edit it) to properly show the contents placed inside a div with class = home_bottomText.

Just place all the bottom text inside such a div, as follows (put this after the <div class="3boxes"></div><!--end 3 boxes-->):

<div class="home_bottomText">
Put here the text to display after the 3 colored boxes.
</div><!--end home_bottomText-->


4) PAGES EDITING

For the other pages, just edit them normally. Please note, as the top bar hasn't a lot of space, it's recommended to either change the logo picture (see CHANGING LOGO) with a smaller one, or to add few pages and many subpages instead.
For the subpages navigation, there is a menu column on the left.


5) CHANGING THE LOGO

To change the "MY WEB PAGES STARTER KIT" image with your one, just overwrite the image inside the MWPSKorg/App_Themes/_images/logo.png with your one. If you want to rename it, then rename it also in the MWPSKorg/App_Themes/Skin.skin file.


6) VARIOUS

Please note that this or other MWPSK Themes may NOT render the menu separators properly when using different IIS Versions. IIS Express was reported to show the menu differently.