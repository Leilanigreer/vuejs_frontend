<script>
export default {
  props: {
    product: Object,
  },
};
</script>

<template>
  <div>
    <h1>Product information</h1>
    <h2>{{ product.name }}</h2>
    <p>price: {{ product.price }}</p>
    <p>description: {{ product.description }}</p>
    <p>supplier_id: {{ product.supplier_id }}</p>
  </div>
</template>

<style></style>