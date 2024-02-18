# Scripts-T
SphereServer 0.56T Official Scripts

[![Source-T](https://github.com/UO-Portal/Source-T)](https://github.com/UO-Portal/Source-T) varsayılan Script Pack

Script pack içeriğindekiler bazı yerler emülatör ile entegre çalışmaktadır.

Not:

Script pack geliştirirken harici fonksiyon kullanımını minimum ölçüde kullanınız. Örneğin 

IF ( <FLAGS> & STATF_HIDDEN) sorgusu yapabiliyorken bunu yapan harici bir IsHide, IsInvıs vb gibi ek fonksiyon yazmayınız. Ne kadar çok fonksiyon kullanımı olursa sunucu ve bu fonksiyonlar ne kadar çok çağırılırsa sunucu performansı uzun uptimelerde düşebilir.


# CLASS
  - Char Class
    * Staff karakterler için class = Class_Staff [SKILLCLASS 0] (scripts/events/chars/class/sphere_events_char_class_staff.scp)
    * Oyuncu karakterler için class = Class_Player [SKILLCLASS 1] (scripts/events/chars/class/sphere_events_char_class_player.scp)

# EVENT
  - Char Events
    * Staff ve Oyuncuları için genel event = e_char_general (scripts/events/chars/sphere_events_char_general.scp)
    * Staff karakterler için genel event = e_char_staff (scripts/events/chars/sphere_events_char_staff.scp)
    * Oyuncu karakterler için genel event = e_char_player (scripts/events/chars/sphere_events_char_player.scp)

  - NPC Events
    * Tüm NPCler için genel event = e_npc_general (scripts/events/npcs/sphere_events_npc_general.scp)
    * Tüm monsterlar (Brain_Monster, Brain_Dragon, Brain_Bersek, Brain_Undead) için genel event = e_npc_monster (scripts/events/npcs/sphere_events_npc_monster.scp)
    * Tüm hayvanlar için genel event = e_npc_animal (scripts/events/npcs/sphere_events_npc_animal.scp)

  - Item Events
    * Tum eşyaların aldığı genel event = ei_item_general (scripts/events/items/sphere_events_item_general.scp)
    * Tum silahların aldığı genel event = ei_item_weapon (scripts/events/items/sphere_events_item_weapon.scp)

  - Region
    * Tum eşyaların aldığı genel event = r_regions (scripts/sphere_region.scp)

# SPEECH

Craft menüler emülatöre entegre edilmiştir. Örneğin craft araçlarına çift tıklandığında script pack içerisindeki dialog açılır. Bu işlem emülatör içerisinden yapılmıştır. Diğer bir örnek partye üye almak için /add komutu girildiğinde script pack içindeki d_party dialogu açılır. Eğer d_party script dialoghunu silerseniz Sphere normal şekilde davranıp /add komutu girince hedef çıkartır.

## Klasör yapısı

- [scripts](#scripts)
    - [add-on](#add-on)
    - [chardefs](#chardefs)
        - [animals](#animals)
        - [bodies](#bodies)
        - [mountables](#mountables)
    - [defnames](#defnames)
    - [dialogs](#dialogs)
        - [craft](#craft)
    - [events](#events)
