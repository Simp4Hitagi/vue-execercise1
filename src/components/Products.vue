<template>
    <div>
        <div v-for="products in productsArray" :key="products">
            <p>{{products.productName}}</p>
            <p>{{products.id}}</p>
            <p>{{products.type}}</p>
            <img src={{products.img}} alt="">
        </div>
    </div>
</template>

<script>


export default {
  name: 'products',
  data() {
        return {
    productsArray: [
    {
    id: 1,
    productName: "Mustang",
    type: "car",
    img: "../assets/logo.png"

},
    {
    id: 2,
    productName: "Deno",
    type: "human",
    img: "../assets/logo.png"

},
    {
    id: 3,
    productName: "Mickey",
    type: "animal",
    img: "../assets/logo.png"

}
]
        }
    }
}

</script>