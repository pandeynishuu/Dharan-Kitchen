<template>
    <div>
        <vue-flux
        :options="fluxOptions"
        :images="fluxImages"
        :transitions="fluxTransitions"
        ref="slider" >
           <flux-pagination slot="pagination"></flux-pagination>
     </vue-flux>
     <div class="fixed">
      <div class="text-block">
        <form name="_resBBBox" action="https://live.ipms247.com/booking/book-rooms-hotelverandah" target="_blank" method="post">
          <div class="bb_resbox" id="bb_resBookingBox" style="width: 100%; background: rgb(234, 236, 237); font-family: Arial, Helvetica, sans-serif; font-size: 12px; border: none;">
            <p class="bbres_fieldset bbres_fieldset3" style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
              <label class="cilabel">Arrival</label>
              <input name="eZ_chkin" type="text" id="eZ_chkin" class="bbres_fieldset datepicker res_chkin2 hasDatepicker" placeholder="dd-mm-yy" readonly="readonly" style="font-family: Arial, Helvetica, sans-serif; color: rgb(91, 91, 91); background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255);">
              <button type="button" class="ui-datepicker-trigger ui-button ui-widget ui-state-default ui-corner-all ui-button-text-only" role="button" style="background-position: 1px -131px;">
                <span class="ui-button-text">...</span>
              </button>
            </p>
            <p class="bbres_fieldset bbres_fieldset4" style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
              <label class="cilabel">Departure</label>
              <input name="eZ_chkout" type="text" id="eZ_chkout" class="bbres_fieldset datepicker res_chkout2 hasDatepicker" placeholder="dd-mm-yy" readonly="readonly" style="font-family: Arial, Helvetica, sans-serif; color: rgb(91, 91, 91); background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255);">
              <button type="button" class="ui-datepicker-trigger ui-button ui-widget ui-state-default ui-corner-all ui-button-text-only" role="button" style="background-position: 1px -131px;">
                <span class="ui-button-text">...</span>
              </button>
            </p>
            <input name="eZ_Nights" id="eZ_Nights" type="hidden" class="txtbox res_nights2" value="1">
            <input name="eZ_adult" id="eZ_adult" type="hidden" class="txtbox" value="1">
            <input name="eZ_child" id="eZ_child" type="hidden" value="0" class="txtbox">
            <input name="eZ_room" id="eZ_room" type="hidden" class="txtbox" value="1">
            <input name="hidBodyLanguage" id="hidBodyLanguage" type="hidden" class="txtbox" value="en">
            <p class="bbres_fieldset bbres_fieldset10 bb_btn" style="font-family: Arial, Helvetica, sans-serif; color: rgb(255, 255, 255);">
              <input type="button" name="bb_resBtn" id="bb_resBtn" value="Book Now" class="bbres_booknow bb_resBtn resbtn234" onclick="BB_valiDateFomData();" style="background: rgb(255, 255, 255); border: 1px solid rgb(255, 255, 255); color: rgb(91, 91, 91); font-family: Arial, Helvetica, sans-serif; font-size: 12px; margin-left: 80px;">
            </p>
            <input name="calformat" id="calformat" type="hidden" class="txtbox" value="dd-mm-yy">
            <input type="hidden" name="ArDt" id="ArDt" value="10-04-2023">
            <input type="hidden" name="acturl" id="acturl" value="https://live.ipms247.com/booking/book-rooms-hotelverandah">
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
      fluxImages: [ 'https://www.dharankitchen.com/img/slide2.jpg','https://www.dharankitchen.com/img/slide3.jpg', 'https://www.dharankitchen.com/img/slide1.jpg', ],
      fluxTransitions: {
         transitionBook: Transitions.transitionBook
      }
   })
}
</script>

<style scoped>

	.bb_resbox
	{
		width: 60%!important; 
		display: inline-block;
	}
@media (max-width: 1200px) {
	.bb_resbox{
		width: 70%!important;
	}}
	@media (max-width: 991px) {
	.bb_resbox{
		width: 100%!important;
	}}
    .entry-header{
    background:#805a57 !important;
    }
    p.bbres_fieldset.bbres_fieldset10.bb_btn{
    position: absolute;
    padding: 0 !important;
    right: 0;
    top: 0;
    height: 100%;
    }
    .bb_resbox  label{
    color: #805a57 !important;
    font-weight: normal;
    }
    .footer-menu{
    opacity: 0.9;
    /*background:linear-gradient(0deg,#805a57,#805a57),url(https://verandah-hotel.com/wp-content/themes/hotelverandah/images/ftr.png);   */
    }
  /*  #rooms::after {
    background:url(); 
    }*/
    .footer {
  /*  background:#805a57 ;*/
    }
    input#bb_resBtn
    {
    margin: 0;
    width: 258px!important;
    border-radius: 0;
    cursor: pointer;
    border: 0 !important;
    font-size: 16px!important;
    height: 100%;
    margin:0px!important;
    padding:9px 13px !important;
    background:#805a57 !important;
    border:1px solid #805a57 !important;
    }
    /*input#bb_resBtn:hover
    {
    background:#805a57 !important;
    border:1px solid #805a57 !important;
    }*/
    input#bb_resBtn:hover
    {
    background:#49201c !important;
    border:1px solid #49201c  !important;
    }
    .ui-datepicker .ui-datepicker-header {
    background:#805a57 !important;
    }
    .ui-datepicker td a.ui-state-active, .ui-datepicker td a.ui-state-hover {
    background:#805a57 !important;
    border:1px solid #805a57 !important;
    }
    .contactadd{
    border:1px solid #805a57 !important;
    }

    @media(max-width: 991px){
    input#bb_resBtn{
        width: 100%!important;
    }
   
         .bb_resbox  label{ color: #fff !important; }
         input#bb_resBtn{
          border: 1px solid #fff !important;
          margin-top: 15px !important;
         }
        
    }


.bbres_fieldset5,.bbres_fieldset6 {
width:49%!important
}

.fixed {
position:relative;
width:100%;
margin:0;
padding:20px
}

div#bb_resBookingBox {
    background: #403938!important;
    padding: 30px 0 10px !important;
}

.bb_resbox p {
line-height:1
}

.fixed {
padding: 0;
}
 
</style>