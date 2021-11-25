1. Use this command to move the theme into the grub theme folder:
   - sudo cp Zen /boot/grub/themes/
2. Edit /etc/default/grub and change the following line to:
   - #Uncomment one of them for the gfx desired, a image or background or gfxtheme
     #GRUB_THEME="I don't remember what the default is here"
     
   - TO:
     #Uncomment one of them for the gfx desired, a image or background or gfxtheme
     GRUB_THEME="/boot/grub/themes/Zen/theme.txt"
   
       - If there isn't any of the above listed then just add GRUB_THEME="/boot/grub/themes/Zen/theme.txt" to the end of the file.
3. Run sudo grub-mkconfig -o /boot/grub/grub.cfg
