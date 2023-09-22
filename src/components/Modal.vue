<template>
    <div class="backdrop">
        <div class="model">
            <p>modal content</p>
        </div>
    </div>
</template>

<style>
.backdrop {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal {
  background: white;
  width: 400px;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
  text-align: center;
}

.modal p {
  font-size: 18px;
  margin-bottom: 20px;
}

/* Add any additional styles or customizations here */
</style>