<template>
    <div class="backdrop">
        <div class="model">
            <h1> {{ header }}</h1>
            <p>modal content</p>
            
        </div>
    </div>
</template>
<script>

export default {
    props:['header']
}
</script>
<style scoped>
.modal {
    width: 400px;
    padding: 20px;
    margin: 100px auto;
    background: white;
    border-radius: 10px;

}
.backdrop {
    top: 1;
    position: fixed-top;
    background:rgba(5, 160, 244, 0.5);
    width: 100%;
    height: 100%;
}
h1 {
  color: #03cfb4;
  border: none;
  padding: 0;
}
</style>