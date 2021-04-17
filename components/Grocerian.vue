<template>
  <div class="bg-green-50 px-10 py-20 my-32">
    <div class="max-w-screen-xl mx-auto">
      <div class="flex flex-col lg:flex-row items-center justify-between">
        <img
          src="~/assets/images/basket.svg"
          alt="grocery basket"
          class="sm:w-7/12 md:w-5/12 lg:w-4/12 pointer-events-none"
        />
        <div
          class="sm:w-10/12 md:w-8/12 text-center mt-12 lg:text-left lg:mt-0 lg:w-6/12"
        >
          <h1 class="font-extrabold font-rale text-2xl sm:text-4xl md:text-5xl">
            Ready to become a
            <span class="text-green-400">grocerian</span>?
          </h1>
          <p
            class="text-sm xs:text-base font-inter font-medium text-black mt-5 text-opacity-50"
          >
            Join Groceri and recieve unlimited 30-min delivery. Coming to your
            neighbourhoods soon!
          </p>
          <form
            @submit.prevent="submitEmail"
            class="my-10 md:mb-5 md:mt-10 lg:mt-16"
          >
            <input
              type="email"
              placeholder="Enter your email"
              required
              class="bg-white-100 focus:outline-none shadow-input rounded-l-xl w-7/12 xs:w-8/12 sm:w-7/12 md:w-7/12 lg:w-8/12 font-medium placeholder-black placeholder-opacity-50 text-xs sm:text-sm md:text-base lg:text-base font-inter py-3 px-3 md:px-4 lg:py-3 lg:px-10"
            />
            <button
              class="hover:opacity-90 focus:outline-none text-white-100 font-bold font-inter ml-i5 bg-green-800 text-xs sm:text-sm md:text-base lg:text-base rounded-r-xl rounded-l-none py-3 px-4 md:px-5 lg:py-3 lg:px-6"
            >
              Notify Me
            </button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    submitEmail() {
      console.log("Click!");
    },
  },
};
</script>

