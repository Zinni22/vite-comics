<script>

export default {
    name: 'CardElement',

    props: {
        src: String,
        title: String,
    }
}

</script>


<template>

    <div class="card">

        <div>
            <img :src="src" :alt="title">
        </div>

        <p>
            {{ title }}
        </p>

    </div>

</template>


<style scoped>
.card div{
    width: 100%;
    height: 70%;
}
img{
      width: 100%;
      height: 100%;
}

p{
    margin-top: 10px;
    color: white;
    font-size: 0.8rem;
}

</style>