<script>
        import { navigate } from "svelte-routing";
        import Login from "../authentication/Login.svelte";
        import Signup from "../authentication/Login.svelte";



        let showLogin = false;
        function handleLogin(){
          showLogin = !showLogin;

        }

      </script>
          <section class="flex flex-col md:flex-row h-screen items-center">
      
        <div class="bg-indigo-600 hidden lg:block w-full md:w-1/2 xl:w-2/3 h-screen">
          <!-- <img src="https://source.unsplash.com/random" alt="" class="w-full h-full object-cover"> -->
          <!-- <video autoplay muted loop class="w-full h-full object-cover">
            <source src="video/logo-biru.mp4" type="video/mp4">
          </video> -->
        </div>
      
        <div class="bg-white w-full md:max-w-md lg:max-w-full md:mx-auto md:mx-0 md:w-1/2 xl:w-1/3 h-screen px-6 lg:px-16 xl:px-12
              flex items-center justify-center">
      
          <div class="w-full h-100">
            <h1 class="text-xl md:text-2xl font-bold leading-tight mt-12">Log in to your account</h1>
            <hr class="my-6 border-gray-300 w-full">
            {#if showLogin}
              <Login />
              <p class="mt-8">Belum punya akun? <button on:click={handleLogin} class="text-blue-500 hover:text-blue-700 font-semibold">Create an
                account
        </button></p>
        {:else}
        <Signup />
        <p class="mt-8">Belum punya akun? <button on:click={handleLogin} class="text-blue-500 hover:text-blue-700 font-semibold">Create an
          account
  </button></p>
        {/if}
            

      
      
      
      
          </div>
        </div>
      
      </section>