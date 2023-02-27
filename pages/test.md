---
title: test
permalink: /test/
description: ""
---
<script>   const lightboxLink = document.querySelector('.lightbox-link');   const lightbox = document.querySelector('#lightbox');   const lightboxImage = document.querySelector('.lightbox-image');   const lightboxClose = document.querySelector('.lightbox-close');      lightboxLink.addEventListener('click', (event) => {     event.preventDefault(); // prevent default link behavior          lightboxImage.src = event.target.src; // set the lightbox image to the clicked image     lightbox.style.display = 'block'; // display the lightbox   });      lightboxClose.addEventListener('click', () => {     lightbox.style.display = 'none'; // hide the lightbox   }); </script>

<style> .lightbox { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.5); z-index: 9999; } .lightbox-content { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center; } .lightbox-image { max-width: 90%; max-height: 90%; } .lightbox-close { background-color: transparent; border: none; color: #fff; font-size: 16px; font-weight: bold; padding: 10px 20px; cursor: pointer; } </style>

<a href="/images/0027-scaled.jpg" class="lightbox-link"> <img src="/images/0027-scaled.jpg" alt="Image description"> </a> 
<div id="lightbox" class="lightbox"> 
	<div class="lightbox-content"> <img src="" alt="Image description" class="lightbox-image"> <button class="lightbox-close">Close</button\> 
 </div> 
</div>