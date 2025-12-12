<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="pt-32 pb-16 overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="max-w-4xl mx-auto text-center mb-16">
      <h1 class="text-5xl md:text-6xl font-semibold tracking-tight text-gray-900 mb-6 leading-[1.1]">
        Turn restaurant tables into instant sales with QR menus
      </h1>
      <p class="text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
        QR Anbessa powers Ethiopian restaurants and hotels with multilingual QR menus, payment-first ordering via Telebirr, and zero unpaid orders.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <Button variant="primary" size="lg" class="rounded-full px-8">Get started</Button>
        <Button variant="outline" size="lg" class="rounded-full px-8">See demo</Button>
      </div>
    </div>

    <!-- Logos Strip -->
    <div class="mb-12">
      <p class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-6 text-left sm:ml-4">Trusted by leading Ethiopian<br>hotels and restaurants</p>
      <div class="flex flex-wrap items-center justify-center gap-12 opacity-60 grayscale px-4">
        <span class="text-2xl font-bold font-sans tracking-tight">Sheraton Addis</span>
        <span class="text-2xl font-bold font-sans tracking-tight">Hyatt Regency</span>
        <span class="text-2xl font-bold font-sans tracking-tight">Radisson Blu</span>
        <span class="text-2xl font-bold font-sans tracking-tight">Yod Abyssinia</span>
        <span class="text-2xl font-bold font-sans tracking-tight">Habesha 2000</span>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative rounded-2xl overflow-hidden shadow-2xl bg-gray-100">
      <img 
        src="/generated/image-ethiopian-restaurant-interior-with-custo-1765563375765-0.webp" 
        alt="Ethiopian restaurant with QR menu on table" 
        class="w-full h-[600px] object-cover object-center"
      />
      
      <!-- Floating UI Elements -->
      <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 flex flex-col gap-4">
        <!-- Notification 1 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 animate-in fade-in slide-in-from-bottom-4 duration-700">
          <div class="w-10 h-10 bg-primary-600 rounded-full flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">Order confirmed</div>
            <div class="text-xs text-gray-500">Table 12 • 850 Birr paid via Telebirr</div>
          </div>
        </div>

        <!-- Notification 2 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 ml-12 animate-in fade-in slide-in-from-bottom-4 duration-1000 delay-300">
          <div class="w-10 h-10 bg-primary-600 rounded-full flex items-center justify-center text-white">
             <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path><polyline points="9 22 9 12 15 12 15 22"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">New order received</div>
            <div class="text-xs text-gray-500">Table 5 • Doro Wat + Injera</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
