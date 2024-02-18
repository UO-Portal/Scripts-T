[COMMENT DIALOG_HELP_SECTION]
dorigin x,y                                     // sets a dynamic origin point
nomove                                          // The gump cannot be moved around.
noclose                                         // The gump cannot be closed with a right click.
nodispose
page id                                         // For multi tab dialogs.
checkertrans x,y,width,height                   // add a transparent layer (only for clients >= 3)
resizepic x,y,backgroundgump,width,height       // can come first if multi page. puts up some background gump
gumppic x,y,gump,hue                            // put gumps in the dlg. (hue only for clients >= 3, otherwise ignored)
gumppictiled x,y,width,height,gump              // tile a gump
tilepic x,y,item                                // put item tiles in the dlg.
tilepichue x,y,item,hue                         // put colored item tiles in the dlg.
text x,y,color,stringindex                      // put some text here.
dtext x,y,color,text                            // put some text here.
croppedtext x,y,width,height,color,stringindex  // put some cropped text here.
dcroppedtext x,y,width,height,color,text        // put some cropped text here.
htmlgump x,y,width,height,stringindex,hasbackground,hasscrollbar                // add an html gump that shows a text
dhtmlgump x,y,width,height,hasbackgroud,hasscrollbar,text                       // add an html gump that show a text
xmfhtmlgump x,y,width,height,clilocid,hasbackground,hasscrollbar                // add an html gump that shows a cliloc text
xmfhtmlgumpcolor x,y,width,height,clilocid,hasbackground,hasscrollbar,color     // add an html gump that shows a colored cliloc text (color should be RGB value, not hue)
xmfhtmltok x,y,width,height,hasbackground,hasscrollbar,color,clilocid,@args@    // add an html gump that shows a cliloc text with arguments (Args seperator=@ -> @arg1@arg2@etc@)
button x,y,down_gump,up_gump,ispressable,pagedest,id                            // add a button
buttontileart x,y,down_gump,up_gump,ispressable,pagedest,id,tileid,tilehue,tilex,tiley      // add a button with a tilepic on top
textentry x,y,widthpix,widthchars,color,id,startstringindex                     // add an input text box
textentrylimited x,y,widthpix,widthchars,color,id,startstringindex,limit        // add an input text box with a "limit" maxchar (only for clients >= 5)
dtextentrylimited x,y,width,height,color,id,limit,text                          // textentry with a limit of characters
tooltip clilocid                                            // Popup a tooltip over a gump object (only for clients >= 4)
group id                                                    // Group a bunch of radios/checkboxes
radio x,y,gump1,gump2,starting_state,id                     // Add a radio button
checkbox x,y,gumpcheck,gumpuncheck,starting_state,checkid   // Add a checkbox
