<template>
  <f7-page name="home" >
<f7-list class="searchbar-not-found">
    <f7-list-item title="Nothing found"></f7-list-item>
  </f7-list>
  <f7-list media-list  class="search-list searchbar-found" >
    <f7-list-item
    link="#"
    title="Elisabeth"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
   >
     <img slot="media" src="../img/img_avatar2.png" width="50" alt="">
    </f7-list-item>

     <f7-list-item
    link="#"
    title="Jean"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
   >
  <img slot="media" src="../img/img_avatar.png" width="50" alt="">
   </f7-list-item>

    <f7-list-item
    link="#"
    title= "Paul"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
    
   >
  <img slot="media" src="../img/beach.jpg" width="50" alt="">
  

   </f7-list-item>
<f7-list-item
    link="#"
    title="Orlane"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
   >
  <img slot="media" src="../img/f7-icon.png" width="50" alt="">
   </f7-list-item>
   <f7-list-item
    link="#"
    title="Henry"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
  
   >
  <img slot="media" src="../img/monkey.jpg" width="50" alt="">
   </f7-list-item>

    <f7-list-item
    link="#"
    title="Marie"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
   >
  <img slot="media" src="../img/img_avatar2.png" width="50" alt="">
   </f7-list-item>
    <f7-list-item
    link="#"
    title="Ribal"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
   >
  <img slot="media" src="../img/f7-icon.png" width="50" alt="">
   </f7-list-item>
  </f7-list>


  </f7-page>
</template>

<style>
img{
  border-radius:50%;
}
</style>