<template>
    <div class="relative mb-16">
        <div class="w-full">
          <img
            src="../assets/factory-design-5-1219226.jpg"
            alt="Avatar"
            width="1250"
            height="230"
            class="w-full"
          />
          <div class="overlay absolute top-20 left-15 w-full md:flex md:justify-center font-semibold">Maintaining excellence within your engineering workforce</div>
        </div>
      </div>
  </template>
  
  <script>
  export default {};
  </script>
  
  <style scoped>
  div img { 
    background: #000000 !important;
    opacity: 0.5;
    height: 230px !important;

  }
  .overlay {
    background: rgb(0, 0, 0);
    background: rgba(0, 0, 0, 0.5); /* Black see-through */
    color: #f1f1f1;
    transition: 0.5s ease;
    opacity: 1;
    color: white;
    font-size: 20px;
    padding: 20px;
    text-align: center;
    z-index: 1;
  }
  
  .contain .overlay {
    opacity: 1;
  }
  </style>