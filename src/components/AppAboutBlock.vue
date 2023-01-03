<template>
    <div class="flex flex-col md:flex-row justify-center items-center w-full p-2">
      <div class="flex flex-col place-content-center text-start text-sm space-y-4 p-2 text-black font-semibold">
        <!-- <p>"Commitment" (Noun) - Meaning - the state or quality of being dedicated to a cause or activity.</p> -->
        <h4 class="w-full">"Commitment" (Noun) - Meaning - the state or quality of being dedicated to a cause or activity.</h4>
        <p>
          Here at MSW, we fundamentally believe our role as a recruitment provider is to create a conduit between both clients and candidates actively seeking assistance within the engineering maintenance and manufacturing sector.  
        </p>
        <p>We therefore take immense pride in ensuring the client/candidate experience is at the forefront of all of our daily actions. We primarily do this by operating in an ethical and responsible manner, continually challenging ourselves in a quest to promote transparency on all fronts. This we feel engenders both enthusiasm and commitment. Your career matters to us; We care.</p>
        <p>By listening we are capable of understanding. By understanding we able to deliver. Through consistently meeting your expectations, our reputation in the sector can only be enhanced.</p>
        <!-- <p>When you decide to engage us, rest assured that you have our total commitment from day one. </p> -->
      </div>
      <div class="w-full sm:w-50">
        <img
          src="../assets/work-on.jpg"
          width="300"
          height="200"
          alt="Image of person working in industry"
          class="w-full p-2"
        />
      </div>
    </div>
  </template>
  
  <script scoped>
  export default {};
  </script>
  
  <style scoped>
  img {
    width: 100%;
    max-width: 600px !important;
    height: 350px;
  }
  p {
    text-align: left !important;
  }
    @media only screen and (max-width: 600px) {
    img {
      height: 300px !important;
    }
  }
  </style>