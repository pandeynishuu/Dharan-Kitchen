<template>
   <div>
      <vue-flux :options="fluxOptions" :images="fluxImages" :transitions="fluxTransitions" ref="slider">
         <flux-pagination slot="pagination"></flux-pagination>
      </vue-flux>
      <div class="search_panel">
         <div class="panel_area">
            <form action="" target="_blank" method="post">
               <div class="res_box">
                  <div class="res_row">
                     <div class="col_md4">
                        <p class="field_set" style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
                           <label for="" class="field_label">Arrival</label>
                           <input name="" type="text" id="" class="datepicker res_input" placeholder="dd-mm-yy"
                              readonly="readonly"
                              style="font-family: Arial, Helvetica, sans-serif; color: rgb(91, 91, 91); background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255);">
                           <button type="button" class="ui-datepicker-trigger" role="button"><span class="ui-button-text"></span></button>
                        </p>
                     </div>
                     <div class="col_md4">
                        <p class="field_set" style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
                           <label for="" class="field_label">Arrival</label>
                           <input name="" type="text" id="" class="datepicker res_input" placeholder="dd-mm-yy"
                              readonly="readonly"
                              style="font-family: Arial, Helvetica, sans-serif; color: rgb(91, 91, 91); background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255);">
                           <button type="button" class="ui-datepicker-trigger" role="button"><span class="ui-button-text"></span></button>
                        </p>
                     </div>
                     <div class="col_md4">
                        <p class="field_set res_btn"
                           style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
                           <input type="button" name="" id="resBtn" value="Book Now" class=""
                              onclick="valiDateFormData();"
                              style="background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255); font-family: Arial, Helvetica, sans-serif; font-size: 12px; margin-left: 80px;">
                        </p>
                     </div>

                  </div>
               </div>
            </form>
         </div>
      </div>
   </div>
</template>

<script>
import { VueFlux, FluxPagination, Transitions } from 'vue-flux';

export default {
   components: {
      VueFlux,
      FluxPagination
   },

   data: () => ({
      fluxOptions: {
         autoplay: true,
         height: "580px",
      },
      fluxImages: ['https://www.dharankitchen.com/img/slide2.jpg', 'https://www.dharankitchen.com/img/slide3.jpg', 'https://www.dharankitchen.com/img/slide1.jpg',],
      fluxTransitions: {
         transitionBook: Transitions.transitionBook
      }
   })
}
</script>
<style scoped>
.search_panel {
   width: 100%;
   box-sizing: border-box;
}

.panel_area {
   position: absolute;
   z-index: 1000;
   width: 100%;
   text-align: center;
   bottom: 10%;
}

.res_row {
   display: flex;
   flex-wrap: wrap;
   /* padding: 15px 220px 25px 0 !important; */
}

@media (min-width: 768px) {
   .col_md4 {
      flex: 0 0 auto;
      width: 33.33333333%;
   }
}

.col_md4 {
   padding: 10px;
}
.col_md4:last-child{
   padding: 2px;
}
@media (min-width: 576px) {
   .col_sm12 {
      flex: 0 0 auto;
      width: 100%;
   }
}

form {
   margin: 0;
}

@media (max-width: 1200px) {
   .res_box {
      width: 70% !important;
   }
}

.res_box {
      width: 100%;
    display: inline-block;
    max-width: 1000px;
}

.res_box {
      display: inline-block;
    position: relative;
    padding: 15px 0px 15px 0 !important;
}

.res_box {
   background: #e0e0e0;
   font-size: 14px !important;
   border: none;
   padding: 0px 0px 10px 0px;
   text-align: center;
}

p.field_set {
   padding: 0 !important;
   margin-right: 25px;
}

.res_box p {
   padding: 10px 6px 0px 6px;
   margin: 0px;
   position: relative;
   float: none;
   display: inline-block;
   width: auto;
   vertical-align: bottom;
   display: inline-block;
   line-height: normal;
}

.res_box label {
   color: #805a57 !important;
   font-weight: normal;
}

.res_box label {
   text-align: left;
   line-height: normal;
   clear: both;
   margin-bottom: 7px;
   width: 100%;
   display: block;
}
.res_box input[type="text"] {
    float: left;
    clear: both;
    padding: 7px 0px 7px 7px;
}
p.res_input input {
    width: 100%!important;
    padding: 10px!important;
    border: none;
}

button.ui-datepicker-trigger {
    padding: 6px 12px;
    font-size: 14px!important;
    font-weight: 400!important;
    line-height: 1!important;
    color: #555!important;
    text-align: center!important;
}

button.ui-datepicker-trigger {
    background: rgba(0, 0, 0, 0) url('../assets/lol.png') no-repeat scroll 0 0;
    border: medium none;
    float: left;
    height: 21px;
    width: 21px;
    margin: 5px;
}
.res_btn{
   width: 258px!important;
    border-radius: 0;
    cursor: pointer;
    border: 0 !important;
    font-size: 16px!important;
    height: 100%;
    margin: 0px!important;
    padding: 9px 13px !important;
    background: #805a57 !important;
    border: 1px solid #805a57 !important;
    color: #fff!important;
    text-transform: uppercase;
}
input#resBtn {
    margin: 0;
    width: 258px!important;
    border-radius: 0;
    cursor: pointer;
    border: 0 !important;
    font-size: 16px!important;
    height: 100%;
    margin: 0px!important;
    padding: 9px 13px !important;
    background: #805a57 !important;
    border: 1px solid #805a57 !important;
}

input#resBtn {
    width: 100%;
    padding: 7px 13px;
    border-radius: 0px;
    -moz-border-radius: 0px;
    -webkit-border-radius: 0px;
    transition: background 0.5s ease;
    -moz-transition: background 0.5s ease;
    -webkit-transition: background 0.5s ease;
    -o-transition: background 0.5s ease;
    text-transform: uppercase;
    font-size: 15px;
    cursor: pointer;
    color: #fff;
    border: 1px solid #43B8BE;
    background: #43B8BE;
}
</style>
