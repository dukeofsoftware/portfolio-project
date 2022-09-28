<template lang="">
 <div class="flex justify-center items-center pt-12 m-12">
    <label for="my-modal" class="btn btn-lg	 btn-ghost	active:bg-none modal-button w-96 h-48 text-2xl">Hakkımda</label>

<!-- Put this part before </body> tag -->
<input type="checkbox" id="my-modal" class="modal-toggle" />
<div class="modal">
  <div class="modal-box">
    <h3 class="font-bold text-lg">Merhaba!!</h3>
    <p class="py-4">Merhaba ben Emre 9.sınıfa gidiyorum yazılımla ilgileniyorum ve bu siteyi vue tailwind ve daisy ui kullanarak yaptım.</p>
    <p class="py-4">Bana ulaşmak için <a href="/contact" class="link">iletişim</a> bölümünden bana mail atabilirsiniz.</p>
    <div class="modal-action">
      <label for="my-modal" class="btn">Kapat</label>
    </div>
  </div>
</div>
 </div>
</template>
<script>
export default {
    
}
</script>
<style>
    h1{
        /*background: -webkit-linear-gradient(rgb(195, 27, 27), rgb(35, 21, 223));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;*/
        background: #0D4DFF;
        background: linear-gradient(to right, #0D4DFF 8%, #14FF14 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }


</style>