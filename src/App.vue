<template>
  <div>
    
    <div class="h-screen" id="d0" ref="d0">

      <div class="flex justify-center h-screen items-center">

        <div class="m-4">

          <h1 class="text-4xl font-mono tracking-tighter">The new <span class="bg-gradient-to-r from-rose-400 via-violet-500 to-indigo-600 text-transparent bg-clip-text">World</span>!</h1>

          <h2 class="font-mono font-bold text-gray-500">is here...</h2>

          <div class="flex justify-center m-8">

            <div class="p-3 bg-slate-700 rounded-full border-2 cursor-pointer border-slate-900 shadow-xl" @click="scrollTo('d1')">

              <svg xmlns="http://www.w3.org/2000/svg" @click="scrollTo('d1')" class="bi bi-arrow-down  w-8 h-8 hover:fill-emerald-400 transition-all ease-in duration-150 fill-white" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M8 1a.5.5 0 0 1 .5.5v11.793l3.146-3.147a.5.5 0 0 1 .708.708l-4 4a.5.5 0 0 1-.708 0l-4-4a.5.5 0 0 1 .708-.708L7.5 13.293V1.5A.5.5 0 0 1 8 1z"/>
              </svg>

            </div>

          </div>

        </div>

      </div>

    </div>

    <div class="h-screen" id="d1" ref="d1">

      <div class="flex justify-center h-screen items-center">

        <div class="m-4">

          <h1 class="text-4xl font-mono tracking-tighter">It's <span class="bg-gradient-to-r from-emerald-400 via-teal-400 to-cyan-500 text-transparent bg-clip-text">free</span></h1>
          <div class="flex justify-center">

            <h2 class="text-2xl font-mono mr-4">and <span class="bg-gradient-to-r from-cyan-400 via-sky-400 to-blue-500 text-transparent bg-clip-text">open</span></h2>

          </div>
          <div class="flex justify-end">

            <h3 class="text-xl font-mono tracking-tighter">for <span class="bg-gradient-to-r from-violet-500 via-purple-600 to-fuchsia-700 text-transparent bg-clip-text">everyone</span></h3>

          </div>

          <div class="flex justify-center m-8">

            <div class="p-3 bg-slate-700 rounded-full border-2 cursor-pointer border-slate-900 shadow-xl" @click="scrollTo('d2')">

              <svg @click="scrollTo('d2')" xmlns="http://www.w3.org/2000/svg" class="bi bi-arrow-down  w-8 h-8 hover:fill-emerald-400 transition-all ease-in duration-150 fill-white" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M8 1a.5.5 0 0 1 .5.5v11.793l3.146-3.147a.5.5 0 0 1 .708.708l-4 4a.5.5 0 0 1-.708 0l-4-4a.5.5 0 0 1 .708-.708L7.5 13.293V1.5A.5.5 0 0 1 8 1z"/>
              </svg>

            </div>

          </div>

        </div>

      </div>

    </div>

    <div class="h-screen" id="d2" ref="d2">

      <div class="flex justify-center h-screen items-center">

        <div class="m-4">

          <h1 class="text-5xl font-mono tracking-tighter">It's the <span class="bg-gradient-to-r from-blue-400 via-indigo-500 to-purple-600 text-transparent bg-clip-text">Internet</span>!</h1>
          
          <div class="flex justify-end mr-16">

            <h3 class="text-xl">By <a href="https://github.com/aixoio" target="_blank" class="font-bold bg-gradient-to-r from-pink-400 via-purple-500 to-indigo-500 bg-clip-text text-transparent cursor-pointer">aixoio</a></h3>

          </div>

        </div>
        
      </div>

    </div>

  </div>
</template>

<script>

export default {

  methods: {

    scrollTo(ref) {

      const elem = this.$refs[ref];

      elem.scrollIntoView({

        behavior: "smooth"

      })

    }

  }

}

</script>
