<template>
              <div id="payment" class="card-block p-0 col-12 show">
                     <b-row class="align-item-center">
                        <b-col lg="8">
                           <iq-card>
                              <template v-slot:headerTitle>
                                    <h4 class="card-title">Payment Options</h4>
                                 </template>
                              <template v-slot:body>
                                 <div class="d-flex justify-content-between align-items-center">
                                    <div class="d-flex justify-content-between align-items-center">
                                       <img src="../../assets/images/booking/cart.png" alt="" height="40" width="50">
                                       <span>US Unlocked Debit Card 12XX XXXX XXXX 0000</span>
                                    </div>
                                    <span>Nik John</span>
                                    <span>28/2020</span>
                                 </div>
                                 <form class="mt-3">
                                    <div class="d-flex align-items-center">
                                       <span>Enter CVV: </span>
                                       <div class="cvv-input ml-3 mr-3">
                                          <input type="text" class="form-control" required="">
                                       </div>
                                       <button type="submit" class="btn btn-primary">Continue</button>
                                    </div>
                                 </form>
                                 <hr>
                                 <div class="card-lists">
                                    <div class="form-group">
                                       <div class="custom-control custom-radio">
                                          <input type="radio" id="credit" name="customRadio" class="custom-control-input">
                                          <label class="custom-control-label" for="credit"> Credit / Debit / ATM Card</label>
                                       </div>
                                       <div class="custom-control custom-radio">
                                          <input type="radio" id="netbaking" name="customRadio" class="custom-control-input">
                                          <label class="custom-control-label" for="netbaking"> Net Banking</label>
                                       </div>
                                       <div class="custom-control custom-radio">
                                          <input type="radio" id="emi" name="emi" class="custom-control-input">
                                          <label class="custom-control-label" for="emi"> EMI (Easy Installment)</label>
                                       </div>
                                       <div class="custom-control custom-radio">
                                          <input type="radio" id="cod" name="cod" class="custom-control-input">
                                          <label class="custom-control-label" for="cod"> Cash On Delivery</label>
                                       </div>
                                    </div>
                                 </div>
                                 <hr>
                                 <div class="add-card">
                                    <a href="#"><span><i class="ri-add-box-line mr-2 font-size-18"></i>Add Gift Card</span></a>
                                 </div>
                              </template>
                           </iq-card>
                        </b-col>
                        <b-col lg="4">
                           <iq-card>
                              <template v-slot:body>
                                 <h4 class="mb-2">Price Details</h4>
                                 <div class="d-flex justify-content-between">
                                    <span>Price 3 Items</span>
                                    <span><strong>$1000.00</strong></span>
                                 </div>
                                 <div class="d-flex justify-content-between">
                                    <span>Delivery Charges</span>
                                    <span class="text-success">Free</span>
                                 </div>
                                 <hr>
                                 <div class="d-flex justify-content-between">
                                    <span>Amount Payable</span>
                                    <span><strong>$1000.00</strong></span>
                                 </div>
                              </template>
                           </iq-card>
                        </b-col>
                     </b-row>
              </div>
</template>
<script>
import { core } from '../../config/pluginInit'
import { mapGetters } from 'vuex'
export default {
  name: 'Payment',
  mounted () {
    core.index()
  },
  computed: {
    ...mapGetters({
      lang: 'Setting/langState'
    })
  },
  watch: {
  },
  methods: {
  },
  data () {
    return {
    }
  }
}
</script>
