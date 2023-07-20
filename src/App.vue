<script setup>
import { ref } from "vue";

let openit = ref(false);
let closeit = ref(true);
let pop = ref(false);
let openModal = ref(false)
let closemodal = ref(false)
let openmodalcard = ref(false)
let openmodalcard2 = ref(false)
let openmodalcard3 = ref(false)

</script>

<template>
  <body>
    <div>
      <div class="relative">
        <nav class="px-3 pt-3 flex justify-between absolute text-white w-full">
          <span class="pl-8 text-2xl text-white">crowdfund</span>

          <span class="pr-7 mb-12  ">
            <ul class="space-x-6 items-center hidden md:flex text-white">
              <li>About</li>
              <li>contact Us</li>
              <li>services</li>
            </ul>
            <div @click="closeit = !closeit">
              <button
                id="menu-btn"
                class="block hamburger md:hidden focus:outline-none"
                :class="{ open: openit }"
                @click="openit = !openit"
              >
                <span class="hamburger-top bg-white"></span>
                <span class="hamburger-middle  bg-white"></span>
                <span class="hamburger-bottom   bg-white"></span>
              </button>
            </div>
            <div class="md:hidden ">
        
      </div>
          </span>
        </nav>
        <div class="md:hidden">
        <div
          id="menu"
          class="absolute rounded-3xl  flex-col items-center flex self-end z-10 w-[60%]  py-8 mt-16 space-y-6 font-bold bg-white sm:w-auto sm:self-center left-6 right-6 drop-shadow-md"
          :class="{invisible: closeit}"
        >
          <a href="#">Pricing</a>
          <div class="w-[60%] mx-[20%] h-[1px] bg-gray-600"></div>
          <a href="#">Product</a>
          <div class="w-[60%] mx-[20%] h-[1px] bg-gray-600"></div>
          <a href="#">About Us</a>
          
        </div>
      </div>
        <img src="../img/1.jpg.jpg" alt="" class="sm:h-[20%] sm:w-[100%] " />
      </div>
      <div class="w-full bg-slate-300 absolute">
        <div class="relative bottom-9">
          <div
            class="md:w-6/12 md:mx-[25%] sm:w-[80%] sm:mx-[10%] bg-white ml-[25%]"
          >
            <img
              src="../img/icon.svg"
              class="relative bottom-6 left-[45%]"
              alt=""
            />
            <h1 class="sm:text-2xl font-bold pt-9 text-center text-xl">
              Mastercraft Bamboo Monitor Raiser
            </h1>
            <p class="text-gray-400 mt-4 text-center sm:text-lg">
              A beautiful handcrafted monitor stand to reduce ear and eye strain
            </p>

            <div class="flex justify-between pb-10 px-10 my-10 gap-10">
              <button
              @click="openModal = !openModal"
                class="bg-green-400 hover:bg-green-500 sm:w-[250px] sm:h-16 text-white py-2 px-4 rounded-full"
              >
                Back this project
              </button>
              <img src="../img/icon-bookmark.svg" class="h-16 w-16" alt="" />
            </div>
          </div>

          <div class="md:w-6/12 bg-white md:ml-[25%] sm:w-[80%] sm:mx-[10%]">
            <div class="md:flex md:justify-around md:px-16 sm:py-5 sm:block">
              <span class="text-center">
                <h2 class="font-bold text-lg">$89,914</h2>
                <p>Of $100,000 backed.</p>
              </span>

              <div
                class="md:hidden md:w-[1px] md:bg-gray-600 md:h-[50px] sm:w-[60%] sm:mx-[20%] sm:my-7 sm:h-[1px] sm:bg-gray-600"
              ></div>
              <div class="md:w-[2px] md:mx-8 bg-gray-500"></div>
              <span class="text-center">
                <h2 class="font-bold text-lg">5,007</h2>
                <p>Total backers.</p>
              </span>

              <div
                class="md:hidden md:bg-gray-600 md:h-[50px] sm:w-[60%] sm:mx-[20%] sm:my-7 sm:h-[1px] sm:bg-gray-600"
              ></div>
              <div class="md:w-[2px] md:mx-8 bg-gray-500"></div>
              <span class="text-center">
                <h2 class="font-bold text-lg">56</h2>
                <p>Days left.</p>
              </span>
            </div>
            <span class="relative bottom-6">
              <div class="h-4 w-[80%] bg-gray-300 rounded-md mx-[10%] my-[10%]">
                <div class="h-4 w-[80%] bg-green-500 rounded-md"></div>
              </div>
            </span>
          </div>

          <div
            class="md:w-6/12 bg-white my-4 md:ml-[25%] sm:w-[80%] sm:mx-[10%]"
          >
            <div class="hardbox1">
              <h2 class="relative top-6 px-7 text-xl font-bold mt-10 mb-12">
                About this project
              </h2>
              <p class="px-7 pb-6 text-gray-500">
                The Mastercraft Bamboo Monitor Riser is a sturdy and stylish
                platform that elevates your screen to a more comfortable viewing
                height. Placing your monitor at eye level has the potential to
                improve your posture and make you more comfortable while at
                work, helping you stay focused on the task at hand.
              </p>
              <p class="px-7 text-gray-500">
                Featuring artisan craftsmanship, the simplicity of design
                creates extra desk space below your computer to allow notepads,
                pens, and USB sticks to be stored under the stand.
              </p>

              <div>
                <div
                  class="border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5"
                >
                  <span
                    class="flex justify-between content-center pt-2 sm:block"
                  >
                    <h2 class="pl-7 font-bold text-lg">bamboo stand</h2>
                    <h2 class="pr-7 text-green-600 sm:pl-7">
                      pledge 25$ or more
                    </h2>
                  </span>
                  <p class="px-7 py-4">
                    You get an ergonomic stand made of natural bamboo. You've
                    helped us launch our promotional campaign, and you will be
                    added to a special Backer member list.
                  </p>
                  <span class="flex justify-between px-7 pt-2 pb-4"
                    ><span class="flex"
                      ><h2 class="text-lg font-bold align-bottom">101</h2>
                      <span class="text-gray-500">left</span></span
                    ><button
                    @click="pop = true"
                      class="bg-green-600 hover:bg-green-700 text-sm text-white py-2 px-4 rounded-full"
                    >
                      Select Reward
                    </button>
                  </span>
                </div>

                <div
                  class="border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5"
                >
                  <span
                    class="flex justify-between content-center sm:block pt-2"
                  >
                    <h2 class="pl-7 font-bold text-lg">Black Edition Standd</h2>
                    <h2 class="pr-7 text-green-600 sm:pl-7">
                      pledge 75$ or more
                    </h2>
                  </span>
                  <p class="px-7 py-4">
                    You get a Black Special Edition computer stand and a
                    personal thank you. Youll be added to our Backer member
                    list. Shipping is included.
                  </p>
                  <span class="flex justify-between px-7 pt-2 pb-4"
                    ><span class="flex"
                      ><h2 class="text-lg font-bold align-bottom">64</h2>
                      <span class="text-gray-500">left</span></span
                    ><button
                    @click="pop = true"
                      class="bg-green-600 hover:bg-green-700 text-sm text-white py-2 px-4 rounded-full"
                    >
                      Select Reward
                    </button>
                  </span>
                </div>

                <div
                  class="border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5"
                >
                  <span
                    class="flex justify-between content-center sm:block pt-2"
                  >
                    <h2 class="pl-7 font-bold text-lg">
                      Mahogany Special Edition
                    </h2>
                    <h2 class="pr-7 text-green-600 sm:pl-7">
                      pledge 200$ or more
                    </h2>
                  </span>
                  <p class="px-7 py-4">
                    You get two Special Edition Mahogany stands, a Backer
                    T-Shirt, and a personal thank you. Youll be added to our
                    Backer member list. Shipping is included.
                  </p>
                  <span class="flex justify-between px-7 pt-2 pb-4"
                    ><span class="flex"
                      ><h2 class="text-lg font-bold align-bottom">0</h2>
                      <span class="text-gray-500">left</span></span
                    ><button
                      @click="pop = true"
                      class="bg-gray-600 hover:bg-gray-700 text-sm text-white py-2 px-4 rounded-full"
                    >
                      Select Reward
                    </button>
                  </span>
                </div>
              </div>
            </div>
          </div>
          <div class=" popup   "
      :class="{openpopup: pop} "
      id="popup">
      <div class=" w-[400px] h-full p-7 rounded-[15px] bg-white  mx-auto ">
        <img
              src="../img/check.svg"
              alt=""
              width="40"
              height="40"
              class="mr-6"
            />
        <h2 class="text-start">Thank for your help</h2>
        <p>
          Thank you for backing this project. you shall reieve the items once launched
        </p>
        <button type="button" class=" bg-green-500 hover:bg-green-600" @click="pop = false">
          Got it
        </button>
      </div>
    </div>
          <!--modal-->
          <div id="modal" class="md:w-[40%] md:mx-[30%] absolute bottom-[600px]  sm:w-[80%] sm:mx-[10%] sm bg-gray-100  sm:bottom-[1700] "
          v-if="openModal"
          >
    <span class="flex justify-between px-7"><h2 class=" text-2xl font-bold py-4">Back this project</h2>  <img  id=" close" @click="openModal = false" src="../img/close.svg" class=" w-4 h-4 mt-[34px]" /></span>
    <p class="pl-7">Want to support us in bringing Mastercraft Bamboo Monitor Riser out in the world? </p>

    
        <div class="pb-4">
            <div class= "card border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5"
            @click="openmodalcard = !openmodalcard" >
                <span class="flex justify-between content-center  pt-2 sm:block">
                <h2 class="pl-7 font-bold text-lg">bamboo stand</h2>
                <h2 class="pr-7 text-green-600 sm:pl-7">pledge 25$ or more</h2>
            </span>
             <p class="px-7 py-4 text-sm">
                You get an ergonomic stand made of natural bamboo. You've helped us launch our promotional campaign, and you will be added to a special Backer member list.
            </p> 
            <span   v-if="openmodalcard" class="cardb ">
                <span  class="flex justify-between px-7 pt-2 pb-4"><span class="flex"><h2 class="text-lg font-bold align-bottom">101</h2><span class="text-gray-500">left</span></span><span @click="pop = !pop"><button  @click="openModal = !openModal" class="bg-green-600 hover:bg-green-700 text-sm text-white py-2 px-4 rounded-full">Collect</button></span>
            </span>
            </span>
             
        </div>
        <div class= "card1 border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5" @click="openmodalcard2 = !openmodalcard2" >
            <span class="flex justify-between content-center  pt-2 sm:block">
                <h2 class="pl-7 font-bold text-lg">Black Edition Standd</h2>
                <h2 class="pr-7 text-green-600  sm:pl-7">pledge 75$ or more</h2>
            </span>
             <p class="px-7 py-4">
                You get a Black Special Edition computer stand and a personal thank you. Youll be added to our Backer member list. Shipping is included.
            </p> 
           <span   v-if="openmodalcard2" class="cardb ">
            <span  class="flex justify-between px-7 pt-2 pb-4"><span class="flex"><h2 class="text-lg font-bold align-bottom">64</h2><span class="text-gray-500">left</span></span><span @click="pop = !pop"><button  @click="openModal = !openModal" class="bg-green-600 hover:bg-green-700 text-sm text-white py-2 px-4 rounded-full">Collect</button></span>
        </span>
        </span>
         
    </div>
    <div class= "card2 border-gray-500 border-2 w-[80%] rounded-md ml-[10%] my-5" @click="openmodalcard3 = !openmodalcard3" >
        <span class="flex justify-between content-center  pt-2 sm:block">
            <h2 class="pl-7 font-bold text-lg"> Mahogany Special Edition </h2>
            <h2 class="pr-7 text-green-600  sm:pl-7">pledge 200$ or more</h2>
        </span>
         <p class="px-7 py-4">
            You get two Special Edition Mahogany stands, a Backer T-Shirt, and a personal thank you. Youll be added to our Backer member list. Shipping is included.
        </p> 
        <span   v-if="openmodalcard3" class="cardb ">
        <span  class="flex justify-between px-7 pt-2 pb-4"><span class="flex"><h2 class="text-lg font-bold align-bottom">0</h2><span class="text-gray-500">left</span></span><span @click="pop = !pop"><button  @click="openModal = !openModal" class="bg-gray-600 hover:bg-gray-700 text-sm text-white py-2 px-4 rounded-full">Collect</button></span>
    </span>
    </span>
     
</div>
        
        
    </div>
</div>
        </div>
      </div>
    </div>
  </body>
</template>

<style scoped>
.hamburger {
  cursor: pointer;
  width: 24px;
  height: 24px;
  transition: all 0.25s;
  position: relative;
}

.hamburger-top,
.hamburger-middle,
.hamburger-bottom {
  position: absolute;
  top: 0;
  left: 0;
  width: 24px;
  height: 2px;
  background: #000;
  transform: rotate(0);
  transition: all 0.5s;
}
.invisible {
  display: none;
}
.visible {
  display: block;
}

.hamburger-middle {
  transform: translateY(7px);
}

.hamburger-bottom {
  transform: translateY(14px);
}

.open {
  transform: rotate(90deg);
  transform: translateY(0px);
}

.open .hamburger-top {
  transform: rotate(45deg) translateY(6px) translate(6px);
}

.open .hamburger-middle {
  display: none;
}

.open .hamburger-bottom {
  transform: rotate(-45deg) translateY(6px) translate(-6px);
}
.popup{



border-radius: 15px;
position: fixed;
top: 0%;
left: 50%;
transform: translate(-50%, -50%) scale(0.1);
text-align: center;
padding: 0 30px 30px;
visibility: hidden;
transition: transform 0.4s, top 0.4s;



}

.popf{
  padding: 0 30px 30px;
}


.popup h2{
font-size: 34px;
font-weight: bold;
margin: 30px 0px 10px;
}
.pbold{
font-weight: bold;
}
.popup button{
width: 100%;
margin-top: 50px;
padding: 10px 0px;

color: #fff;
border: 0;
outline: none;
font-size: 18px;
border-radius: 4px;
cursor: pointer;
box-shadow: 0 5px 5px rgba(0,0,0,0.2);

}
.popup img{
padding-top: 15px;
}

.openpopup{
visibility: visible;
top:50%;
transform: translate(-50%, -50%) scale(1);

}
</style>
