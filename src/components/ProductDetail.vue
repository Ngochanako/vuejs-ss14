<template>
    <div>
        <v-container>
            <header style="display: flex; gap: 100px;">
                <div style="background-color: beige;" class="box">
                    <div><v-icon color="orange" size="x-large">mdi-cart</v-icon></div>
                    <div class="box-main">
                        <h4>Item Cart</h4>
                        <p>Product Summary</p>
                    </div>
                </div>
                <div class="box">
                    <div><v-icon color="orange" size="x-large">mdi-file</v-icon></div>
                    <div class="box-main">
                        <h4>Billing</h4>
                        <p>Billing Information</p>
                    </div>
                </div>
                <div class="box">
                    <div><v-icon color="orange" size="x-large">mdi-receipt</v-icon></div>
                    <div class="box-main">
                        <h4>Payment</h4>
                        <p>Add and Update Card</p>
                    </div>
                </div>
            </header>
            <div class="hr"></div>
    <v-table>
    <thead>
      <tr>
        <th class="text-left">
          Product
        </th>
        <th class="text-left">
          Price
        </th>
        <th class="text-left">
          Quantity
        </th>
        <th class="text-left">
          Total
        </th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      <tr style="height: 150px;">
        <td>
        <v-row class="align-center">
       <img style="width: 60px;height: 60px; border-radius: 5px;object-fit: cover;" src="https://i.pinimg.com/564x/7b/dd/6c/7bdd6c58504a16b5a17691518c41b5f2.jpg" alt="">
      <p>Cute shop Teddy Bear</p>
    </v-row>
    </td>
     <td>
        <p>$2000</p>
        <p style="font-size: smaller;color: gray;text-decoration: line-through;">$175</p>
     </td>
     <td>
        <v-btn>-</v-btn>
        <v-btn>1</v-btn>
        <v-btn>+</v-btn>
     </td>
     <td>
        $2000
     </td>
     <td>
        <v-icon> mdi-trash-can</v-icon>
     </td>
      </tr>

    </tbody>
  </v-table>
  <v-card style="width: 100%;margin-top: 50px;padding:20px 100px;">
    <v-card-item>
      <v-card-title>
        Order Summary
      </v-card-title>

      <v-card-subtitle style="font-size: 18px;display: flex;flex-direction: column;gap: 20px;margin-top: 50px;">
       <div style="display: flex; justify-content: space-between;">
        <p>Sub Total</p>
        <p style="font-weight: 600;">$2000</p>
       </div>
       <div style="display: flex; justify-content: space-between;">
        <p>Discount</p>
        <p style="color: orange;">5%</p>
       </div>
       <div style="display: flex; justify-content: space-between;">
        <p>Shipping Chart</p>
        <p style="color: orange;">-</p>
       </div>
       <div style="display: flex; justify-content: space-between;">
        <p style="color: black;font-weight: 600;">Total</p>
        <p>$190</p>
       </div>
      </v-card-subtitle>
    </v-card-item>
    </v-card>
    <footer style="display: flex;justify-content: space-between;padding: 50px;">
        <v-chip class="ma-2" color="orange" label>Continue Shopping</v-chip>
        <v-btn color="red">Checkout</v-btn>
    </footer>
        </v-container>
    </div>
</template>

<script setup>

</script>

<style scoped>
.box{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
    gap:10px;
}
.hr{
    width: 100%;
    height: 1px;
    background-color: #ccc;
    margin: 20px 0;
}
td{
    padding: 10px;
}
div.btn__content {
  padding: 0;
}

div.card__actions .btn {
  min-width: 0;
}
.v-btn--size-default{
    min-width: 40px;
}
</style>