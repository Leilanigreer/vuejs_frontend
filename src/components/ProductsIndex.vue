<script>
 export default {
   props: {
     products: Array,
   },
 };
  </script>

  <template>
    <div>
      <h1>All products</h1>
     <div v-for="product in products" v-bind:key="product.id">
       <h2>{{ product.name }}</h2>
       <p>price: {{ product.price }}</p>
       <p>description: {{ product.description }}</p>
       <p>supplier_id: {{ product.supplier_id }}</p>
       <button v-on:click="$emit('showProduct', product)">More info</button>
     </div>
    </div>
  </template>

  <style></style>