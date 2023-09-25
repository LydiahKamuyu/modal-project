<template>
    <div class="backdrop">
        <div class="model">
            <h1> Modal title</h1>
            <p>modal content</p>
            
        </div>
    </div>
</template>

<style>
.modal {
    width: 400px;
    padding: 20px;
    margin: 100px auto;
    background: white;
    border-radius: 10px;

}
.backdrop {
    top: 0;
    position: fixed-top;
    background:rgba(5, 160, 244, 0.5);
    width: 100%;
    height: 100%;
}
.modal h1 {
  color: #03cfb4;
  border: none;
  padding: 0;
}
</style>