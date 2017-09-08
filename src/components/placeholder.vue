<template>
	<div class="hello">
	    <div class="animated-background" v-bind:class="message">
	    </div>
    </div>
</template>

<script>
export default {
	name: 'placeholder',
	props: ['message'],
	created: function () {
		var item = document.getElementsByClassName('animated-background');
		console.log(item)
	}
}
	

</script>
<style>
	.hello {
    background: #fff;

    margin: 0 auto;
}
@keyframes placeHolderShimmer{
    0%{
        background-position: -468px 0
    }
    100%{
        background-position: 468px 0
    }
}

.animated-background {
    animation-duration: 1s;
    animation-fill-mode: forwards;
    animation-iteration-count: infinite;
    animation-name: placeHolderShimmer;
    animation-timing-function: linear;
    background: #f6f7f8;
    background: linear-gradient(to right, #eeeeee 8%, #dddddd 18%, #eeeeee 33%);
    background-size: 800px 104px;
    position: relative;
}
</style>