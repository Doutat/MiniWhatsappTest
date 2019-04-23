<template>

<f7-page name="disc" >


<f7-list class="searchbar-not-found">
    <f7-list-item title="Nothing found"></f7-list-item>
  </f7-list>

  <f7-list class="search-list searchbar-found" >
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
    <f7-list-item
    link="#"
    title="Henry"
    after="17:14"
    subtitle="Mon test de..." 
    no-chevron="true"
  
   >
  <img slot="media" src="../img/monkey.jpg" width="50" alt="">
   </f7-list-item>
  </f7-list>
 <f7-fab position="right-bottom" slot="fixed" color="green">
    <f7-icon ios="f7:chat_bubble" aurora="f7:chat_bubble" md="material:chat_bubble"></f7-icon>
    <f7-icon ios="f7:close" aurora="f7:close" md="material:close"></f7-icon>
   
  </f7-fab>
</f7-page>
</template>
<style>
img{
  border-radius:50%;
}
</style>

