<template>
  <div class="landing-page min-h-screen bg-[#070a10] text-slate-100 relative overflow-hidden flex flex-col items-center justify-center p-2 sm:p-2 lg:p-2">
    <div class="flex benefit-card glass-card glass-card-hover rounded-xl p-3.5 flex gap-3.5 items-center text-center">
          <div>
            <h3 class="text-sm font-bold text-white">No page found</h3>

          </div>
        </div>
    
    <!-- Ambient Dynamic Lighting & Radar Background --cmt
    <div class="pointer-events-none absolute inset-0 overflow-hidden">
      Glow Orbs --cmt
      <div class="absolute -top-40 left-1/2 -translate-x-1/2 w-[600px] h-[600px] bg-emerald-500/15 rounded-full blur-[140px] animate-pulse-glow"></div>
      <div class="absolute top-1/3 -left-40 w-[450px] h-[450px] bg-blue-600/10 rounded-full blur-[120px]"></div>
      <div class="absolute bottom-10 -right-40 w-[500px] h-[500px] bg-cyan-500/10 rounded-full blur-[130px]"></div>
      
      Tech Grid Lines --cmt
      <div 
        class="absolute inset-0 opacity-[0.035]"
        style="background-image: linear-gradient(rgba(255, 255, 255, 0.2) 1px, transparent 1px), linear-gradient(90deg, rgba(255, 255, 255, 0.2) 1px, transparent 1px); background-size: 40px 40px;"
      ></div>

      Radar Concentric Rings in Background --cmt
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[700px] h-[700px] rounded-full border border-emerald-500/5 pointer-events-none"></div>
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[1000px] h-[1000px] rounded-full border border-blue-500/5 pointer-events-none"></div>
    </div>


    Main Glassmorphic Card Container --cmt
    <main class="landing-card relative z-10 w-full max-w-lg rounded-3xl bg-[#0d1322]/85 border border-slate-700/50 p-6 sm:p-8 backdrop-blur-xl shadow-2xl shadow-black/80 transition-all">
      
      Top Decorative Accent Bar --cmt
      <div class="absolute top-0 left-1/2 -translate-x-1/2 w-48 h-[2px] bg-gradient-to-r from-transparent via-emerald-400 to-transparent"></div>

      Avatar & Brand Hero Section --cmt
      <header class="brand-header flex flex-col items-center text-center">
        
        Profile Circle with Concentric Radar Wave Effect --cmt
        <div class="profile-link relative mb-2 group cursor-pointer" @click="redirectToTg" title="Click to join Telegram">
          Animated Outer Ripple Ring --cmt
          <div class="absolute -inset-2 rounded-full border border-emerald-500/30 animate-ping opacity-25"></div>
          Glowing Radial Backdrop --cmt
          <div class="absolute -inset-1.5 rounded-full bg-gradient-to-tr from-emerald-500 via-cyan-500 to-blue-600 opacity-70 blur-sm group-hover:opacity-100 transition duration-500"></div>
          
          Profile Logo Container --cmt
          <div class="brand-logo relative w-25 h-25 sm:w-30 sm:h-30 rounded-full bg-black border-2 border-slate-700/80 overflow-hidden flex items-center justify-center shadow-xl group-hover:scale-[1.02] transition-transform duration-300">
            <img 
              src="/profit-logo.jpeg" 
              alt="Profit Radar Logo" 
              class="w-full h-full object-cover"
              loading="eager"
            />
          </div>

          Verified Checkmark Badge --cmt
          <div class="absolute bottom-1 right-1 w-8 h-8 rounded-full bg-gradient-to-tr from-blue-600 to-cyan-400 border-2 border-[#0d1322] flex items-center justify-center text-white shadow-md">
            <svg class="w-4 h-4 fill-current" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
            </svg>
          </div>
        </div>

       

        <h1 class="brand-title text-2xl sm:text-4xl font-extrabold tracking-tight text-white mb-1 font-heading">
          PROFIT <span class="bg-gradient-to-r from-emerald-400 via-teal-300 to-cyan-400 bg-clip-text text-transparent">RADAR</span>
        </h1>

        <p class="brand-subtitle text-slate-400 text-sm sm:text-base font-medium tracking-wide max-w-xs sm:max-w-sm mb-0">
          Market Analysis. Simplified.
        </p>

        Social Proof Stats Banner --cmt
        <div class="social-proof w-full gap-2 py-3 px-4 rounded-2xl">
          <div class="flex flex-col items-center">
            <div class="flex items-center gap-1.5">
              <span class="text-xl sm:text-2xl font-extrabold text-white font-heading">5,025+</span>
              <span class="text-[10px] font-bold px-1.5 py-0.5 rounded bg-emerald-500/20 text-emerald-400">Subscribers</span>
            </div>
            <span class="text-xs text-slate-400 mt-0.5">Active Subscribers</span>
          </div>

        </div>

      </header>

      
      Key Features Section (4 Elevated Glass Cards) --cmt
      <section class="benefit-list space-y-2.5 mb-6" aria-label="Key Benefits">
        
        Feature 1: All Segments --cmt
        <div class="flex benefit-card glass-card glass-card-hover rounded-xl p-3.5 flex gap-3.5 items-center text-center">
          <div>
            <h3 class="text-sm font-bold text-white">✅ Works Across All Segments</h3>

          </div>
        </div>

        Feature 2: Trend Based Analysis --cmt
        <div class="flex benefit-card glass-card glass-card-hover rounded-xl p-3.5 flex items-center gap-3.5 text-center">
          <div>
            <h3 class="text-sm font-bold text-white">✅ Trend Based Advanced Analysis</h3>
          </div>
        </div>

        Feature 3: Trading Concepts --cmt
        <div class="flex benefit-card glass-card glass-card-hover rounded-xl p-3.5 flex items-center gap-3.5 text-center">
          <div>
            <h3 class="text-sm font-bold text-white">✅ Trading & investing concepts</h3>
          </div>
        </div>

        Feature 4: Accuracy Insights --cmt
        <div class="flex benefit-card glass-card glass-card-hover rounded-xl p-3.5 flex items-center gap-3.5 text-center">
          <div>
            <div class="flex items-center gap-2">
              <h3 class="text-sm font-bold text-white">✅ Indicator-Based upto 90% Accurate Insights</h3>
            </div>
          </div>
        </div>

      </section>


      Action Area: Primary CTA Button --cmt
      <div class="cta-area flex flex-col items-center">
        
        <p class="text-sm font-medium text-slate-300 mb-3 flex items-center justify-center gap-2">
          <span>👇</span>
          <span>Join Our Free Channel Now</span>
          <span>👇</span>
        </p>

        <button 
          id="telegram-join-btn"
          @click="redirectToTg"
          class="cta-button relative w-full overflow-hidden rounded-2xl bg-gradient-to-r from-blue-600 via-blue-500 to-cyan-500 p-0.5 text-white font-bold text-base sm:text-lg shadow-xl shadow-blue-600/30 hover:shadow-blue-500/50 hover:scale-[1.02] active:scale-[0.98] transition-all duration-300 group cursor-pointer"
        >
          Shimmer Animation Layer --cmt
          <div class="shimmer-sweep pointer-events-none"></div>

          Button Content Layer --cmt
          <div class="relative z-10 w-full py-4 px-6 rounded-[14px] bg-gradient-to-r from-blue-600 to-blue-700 group-hover:from-blue-500 group-hover:to-cyan-600 flex items-center justify-center gap-3 transition-colors">
            
            Telegram Airplane SVG ---cmt
            <svg class="w-6 h-6 fill-current text-white transition-transform group-hover:rotate-12 duration-300" viewBox="0 0 24 24">
              <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.15 1.58-.8 5.42-1.13 7.19-.14.75-.42 1-.68 1.03-.58.05-1.02-.38-1.58-.75-.88-.58-1.38-.94-2.23-1.5-.99-.65-.35-1.01.22-1.59.15-.15 2.71-2.48 2.76-2.69a.2.2 0 00-.05-.18c-.06-.05-.14-.03-.21-.02-.09.02-1.49.95-4.22 2.79-.4.27-.76.41-1.08.4-.36-.01-1.04-.2-1.55-.37-.63-.2-1.12-.31-1.08-.66.02-.18.27-.36.74-.55 2.92-1.27 4.86-2.11 5.83-2.52 2.77-1.16 3.35-1.36 3.73-1.36.08 0 .27.02.39.12.1.08.13.19.14.27-.01.06.01.24 0 .38z"/>
            </svg>

            <span class="tracking-wide">JOIN NOW</span>
            
            Arrow icon ---cmt
            <svg class="w-5 h-5 transition-transform group-hover:translate-x-1 duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M13 7l5 5m0 0l-5 5m5-5H6"/>
            </svg>
          </div>
        </button>

        
        
      </div>
      Urgency Bar with Dynamic Countdown --cmt
        <div class="mb-1 mt-2 p-3 flex items-center justify-between">
        <div class="flex items-center gap-2">
            <p class="text-xs font-semibold text-amber-200">Invitation link expires in</p>
        </div>
        <div class="px-3 py-1 rounded-xl bg-black/60 border border-amber-500/40 text-amber-400 font-mono font-bold text-sm tracking-wider shadow-inner">
          00:{{ countdown < 10 ? '0' + countdown : countdown }}s
        </div>
      </div>
      
      Regulatory Disclaimer (Preserved & Cleanly Styled) --cmt
      <footer class="legal-disclaimer mt-2 pt-4 border-t border-slate-800/60 text-center">
        <p class="text-[11px] text-slate-500 leading-relaxed max-w-sm mx-auto">
          <strong class="text-slate-400 font-semibold">Disclaimer:</strong> For educational and informational purposes only. 
          This is not investment or financial advice. Investments in securities and financial markets are subject to market risks. 
          No returns or profits are guaranteed.
        </p>
        
      </footer>

    </main> -->

  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

// Urgency Countdown Loop (Preserved exact functionality)
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
  if (timer) {
    clearInterval(timer);
  }
});

// Primary Telegram Redirect Function (Preserved link & enriched with Meta Pixel tracking if active)
const redirectToTg = () => {
  if (typeof window !== 'undefined' && window.fbq) {
    window.fbq('track', 'Lead');
  }
 // window.open('https://t.me/+IguweYFxOtc3NDQ1', '_blank');
};

// PRESERVED COMMENTED UTM CAMPAIGN LOGIC FOR FUTURE REFERENCE:
// const redirectToTg = () => {
//     const params = new URLSearchParams(window.location.search)
//     const campaign = params.get('utm_campaign')
//
//     let telegramLink = "https://t.me/+rjxI_6nSGWEzMzll"  // default (original link)
//
//     if (campaign === "camp1") {
//         telegramLink = "https://t.me/+rjxI_6nSGWEzMzll"
//     } else if (campaign === "camp2") {
//         telegramLink = "https://t.me/+ByqRz_MgVJs4NmZl"
//     } else if (campaign === "camp3") {
//         telegramLink = "https://t.me/+Ey1TxP6PQ6w5YWY1"
//     } else if (campaign === "camp4") {
//         telegramLink = "https://t.me/+WYfZXeGRrY85ZjRl"
//     }
//
//     if (window.fbq) {
//         window.fbq('track', 'Subscribe', {
//             campaign: campaign || "default"
//         })
//     }
//
//     window.open(telegramLink, '_blank')
// }

const patternIcons = ['📊', '💰', '📈', '🎯', '⚡', '💹', '📋', '⏰', '🔔', '💎'];
</script>

<style scoped>
@media (max-width: 639px) {
  .landing-page {
    min-height: 100svh;
    height: 100svh;
    padding: 10px 12px;
  }

  .landing-card {
    max-width: 430px;
    padding: 18px 16px;
    border-radius: 24px;
  }

  .profile-link { margin-bottom: 10px; }

  .brand-logo {
    width: 80px;
    height: 80px;
  }

  .brand-title {
    font-size: 1.75rem;
    line-height: 1.1;
    margin-bottom: 6px;
  }

  .brand-subtitle { margin-bottom: 10px; }

  .social-proof {
    padding: 8px 12px;
    margin-bottom: 12px;
  }

  .benefit-list {
    margin-bottom: 16px;
    row-gap: 8px;
  }

  .benefit-card { padding: 10px 12px; }

  .benefit-card h3 {
    font-size: 0.875rem;
    line-height: 1.35;
  }

  .cta-area > p { margin-bottom: 8px; }

  .cta-button > div {
    padding-top: 12px;
    padding-bottom: 12px;
  }

  .legal-disclaimer {
    margin-top: 14px;
    padding-top: 10px;
  }
}

@media (max-width: 639px) and (max-height: 700px) {
  .landing-card {
    padding-top: 12px;
    padding-bottom: 12px;
  }

  .brand-logo {
    width: 68px;
    height: 68px;
  }

  .legal-disclaimer { display: none; }
}
</style>
