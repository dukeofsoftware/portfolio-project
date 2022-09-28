<template lang="">
    <div class="container">
        <form action="https://formsubmit.co/dukeofsoftware@gmail.com" method="POST">


            <div class="form-group m-3">
              <label for="exampleInputEmail1" autocomplete="off" class="text-sz text-black text-base">Email</label>
              <input type="email" class="form-control p-2" id="exampleInputEmail1" aria-describedby="emailHelp" autocomplete="off" placeholder="Mailinizi girin" required name="email">
              <small id="emailHelp" class="form-text text-muted"></small>
            </div>
            <div class="form-group m-3">
                <input type="hidden" name="_captcha" value="false" class="form-control">

              </div>
              <div class="form-group m-3">
                <input type="hidden" name="_subject" class="form-control">

              </div>
              <div class="form-group m-3">
                <input type="hidden" name="_next" class="form-control">

              </div>
              <div class="form-group m-3">
                <label for="exampleInputEmail1" autocomplete="off" class="text-sz text-black text-base">Mesaj</label>
                <input type="text" name="name" autocomplete="off" placeholder="Mesajınız" class="form-control p-2">
              </div>
          
            
            <button type="submit" class="btn btn-primary m-3 py-2">Gönder</button>
          </form>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    label{
        font-size:4rem ;
        font-family: Oswald;
        color:white;
    }
</style>