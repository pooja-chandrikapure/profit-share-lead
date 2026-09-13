<template>
    <div class="min-h-screen bg-black relative overflow-hidden flex items-center justify-center">
        <!-- Background Pattern -->
        <div class="absolute inset-0 opacity-10">
            <div class="grid grid-cols-12 gap-4 transform rotate-12 scale-150">
                <div v-for="i in 144" :key="i"
                    class="w-8 h-8 border border-green-500 rounded flex items-center justify-center text-green-500 text-xs">
                    {{ patternIcons[(i - 1) % 10] }}
                </div>
            </div>
        </div>

        <!-- Main Card -->
        <div
            class="relative z-10 bg-gray-900 rounded-2xl py-8 px-4 w-full max-w-md mx-4 shadow-2xl border border-gray-800">
            <!-- Profile Circle -->
            <div class="flex justify-center mb-6">
                <div @click="redirectToTg"
                    class="cursor-pointer w-30 h-30 bg-black rounded-full border-2 border-white flex items-center justify-center">
                    <img src="/profit-logo.jpeg" class="rounded-full" alt="">
                </div>
            </div>

            <!-- Title -->
            <h1 class="text-white uppercase text-2xl font-extrabold text-center mb-2 leading-tight">
                🚀 Profit Radar 📊
            </h1>

            <!-- Subtitle -->
            <h2 class="text-white uppercase text-[11px] font-bold text-center mb-4 leading-tight">
                Market Analysis. Simplified.
            </h2>

            <div class="text-white my-4 text-center">
            <p class="mt-4 text-base text-md">
                5025+ <span class="font-semibold">Subscribe</span>
            </p>
            </div>

            <!-- Key Features Header -->
            <div class="text-white text-sm mb-3 text-center">
                <p class="mt-4 text-lg font-semibold flex items-center justify-center gap-2">
                    ✅ Works Across All Segments
                </p>
                <p class="mt-4 text-lg font-semibold flex items-center justify-center gap-2">
                    ✅ Trend Based Advanced Analysis
                </p>
                <p class="mt-4 text-lg font-semibold flex items-center justify-center gap-2">
                    ✅ Trading & investing concepts
                </p>
                <p class="mt-4 text-lg font-semibold flex items-center justify-center gap-2">
                    ✅ Indicator-Based upto 90% Accurate Insights
                </p>
                

            </div>

            <!-- Features List -->
            <!-- <div class="space-y-3 text-white text-sm justify-center text-center">
                    <p class="  ">
                    ✅ Trend Based Advanced Analysis 
                    </p>
                    <p class="">
                    ✅ Trading & investing concepts
                    </p>
                    <p class=" ">
                    ✅ Indicator-Based upto 90% Accurate Insights
                    </p>
                   

            </div> -->

            <!-- Join Channel Text -->
              <p class="text-white text-center my-6 font-medium">
                    👇 Join Our Free Channel Now 👇
              </p>
              <!-- <p class="text-white text-center my-6 font-medium">
                  🚀Join our FREE Channel to see the Magic unfold! 🚀
                </p> -->
                
                <!-- Join Button with Shine Effect -->
                <div class="flex justify-center">
                    <button @click="redirectToTg"
                    class="join-button bg-blue-600 hover:bg-blue-700 text-white border border-white font-semibold py-3 px-8 rounded-full transition-all duration-300 overflow-hidden transform hover:scale-105">
                    <span class="relative z-10">Join Now</span>
                    <!-- Shine Effect -->
                    <div
                    class="shine-overlay absolute inset-0 bg-gradient-to-r from-transparent via-white/30 to-transparent transform -translate-x-full skew-x-12">
                </div>
            </button>
        </div>
        <!-- <p class="text-center my-6 font-medium text-red-400 text-2xl">
              Invitation closes in {{ countdown }}s
        </p> -->

            <!-- Updated Content -->
            <div class="text-[12px] text-white/40 leading-tight mt-4 text-center">
                Disclaimer - For educational and informational purposes only. 
                This is not investment advice. Investments in securities markets are subject to market risks. 
                No returns or profits are guaranteed.
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";


const START_TIME = 10; // seconds
const countdown = ref(START_TIME);
let timer = null;

onMounted(() => {
  timer = setInterval(() => {
    if (countdown.value > 0) {
      countdown.value--;
    } else {
      countdown.value = START_TIME; // 🔁 reset (loop)
    }
  }, 1000);
});
onUnmounted(() => {
    clearInterval(timer);
});
const redirectToTg = () => {
    window.open('https://t.me/+S71wdMVrWpsxYjJl', '_blank')
}
// const redirectToTg = () => {
//     const params = new URLSearchParams(window.location.search)
//     const campaign = params.get('utm_campaign')

//     let telegramLink = "https://t.me/+rjxI_6nSGWEzMzll"  // default (original link)

//     if (campaign === "camp1") {
//         telegramLink = "https://t.me/+rjxI_6nSGWEzMzll"
//     } else if (campaign === "camp2") {
//         telegramLink = "https://t.me/+ByqRz_MgVJs4NmZl"
//     } else if (campaign === "camp3") {
//         telegramLink = "https://t.me/+Ey1TxP6PQ6w5YWY1"
//     } else if (campaign === "camp4") {
//         telegramLink = "https://t.me/+WYfZXeGRrY85ZjRl"
//     }

//     if (window.fbq) {
//         window.fbq('track', 'Subscribe', {
//             campaign: campaign || "default"
//         })
//     }

//     window.open(telegramLink, '_blank')
// }
const patternIcons = ['📊', '💰', '📈', '🎯', '⚡', '💹', '📋', '⏰', '🔔', '💎']
</script>

<style scoped>
@keyframes shine {
    0% {
        transform: translateX(-100%) skewX(-15deg);
    }

    100% {
        transform: translateX(200%) skewX(-15deg);
    }
}

.join-button:hover .shine-overlay {
    animation: shine 0.8s ease-in-out;
}

.join-button {
    position: relative;
    background: linear-gradient(45deg, #0f46bd, #286ddd);
    box-shadow: 0 4px 15px rgba(37, 99, 235, 0.3);
}

.join-button:hover {
    box-shadow: 0 6px 20px rgba(37, 99, 235, 0.4);
    transform: scale(1.05) translateY(-1px);
}

.join-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
    animation: shine-continuous 3s infinite;
    z-index: 1;
}

@keyframes shine-continuous {
    0% {
        left: -100%;
    }

    50% {
        left: 100%;
    }

    100% {
        left: 100%;
    }
}

/* Background animation */
.bg-black {
    background: radial-gradient(ellipse at center, #1a1a2e 0%, #000000 70%);
}
</style>
