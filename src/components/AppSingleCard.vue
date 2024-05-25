<script>
export default {
    props: ["card"],
}
</script>

<template>
    <div class="mycard">
        <div class="myimgcard">
            <img class="object-fit-cover" :src="card.thumb" alt="">
        </div>
        <div>
            <span>{{ card.series }}</span>
        </div>
    </div>
</template>

<style>
.mycard {
    width: calc(100% / 6 - 2rem);
    height: auto;
    margin:  1rem;

}

    .myimgcard {
    width: 100%;
    height: 12rem;
}

img {
    width: 100%;
    height: 100%;
    object-position: top;
}


</style>