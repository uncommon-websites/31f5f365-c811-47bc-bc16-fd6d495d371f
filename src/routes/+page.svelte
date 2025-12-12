<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Stats from "$lib/components/Stats.svelte";
  import Steps from "$lib/components/Steps.svelte";
  import FeatureSection from "$lib/components/FeatureSection.svelte";
  import CaseStudies from "$lib/components/CaseStudies.svelte";
  import Integrations from "$lib/components/Integrations.svelte";
  import Resources from "$lib/components/Resources.svelte";
  import BottomCTA from "$lib/components/BottomCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Header />

<main>
  <Hero />
  <Stats />
  <Steps />
  
  <!-- Feature 1: Multilingual QR Menus -->
  <FeatureSection 
    title="Multilingual QR menus that speak your customers' language"
    subtitle="REACH EVERY CUSTOMER"
    linkText="Learn about menu features"
    bullets={[
      "Support for Amharic, English, and multiple languages",
      "Beautiful menu layouts with dish photos and descriptions",
      "Instant updates across all QR codes when you change prices",
      "Mobile-optimized for seamless browsing on any device"
    ]}
  >
    <div slot="description">
      <p>Create professional digital menus that work for local and international guests—no printing costs, instant updates, and zero language barriers.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
      <!-- Mobile menu mockup -->
      <div class="bg-white rounded-2xl shadow-2xl p-4 w-64 relative">
        <div class="flex items-center justify-between mb-4 pb-3 border-b border-gray-100">
          <div class="text-xs font-semibold text-gray-900">Menu</div>
          <div class="flex gap-2">
            <span class="text-xs bg-primary-100 text-primary-700 px-2 py-1 rounded-full font-medium">አማርኛ</span>
            <span class="text-xs bg-gray-100 text-gray-600 px-2 py-1 rounded-full">EN</span>
          </div>
        </div>
        <div class="space-y-3">
          <div class="flex gap-3 p-2 bg-gray-50 rounded-lg">
            <div class="w-16 h-16 bg-primary-200 rounded-lg flex items-center justify-center text-2xl">🍲</div>
            <div class="flex-1">
              <div class="text-sm font-semibold text-gray-900">ዶሮ ወጥ</div>
              <div class="text-xs text-gray-500">Doro Wat</div>
              <div class="text-sm font-bold text-primary-600 mt-1">450 Birr</div>
            </div>
          </div>
          <div class="flex gap-3 p-2 bg-gray-50 rounded-lg">
            <div class="w-16 h-16 bg-primary-200 rounded-lg flex items-center justify-center text-2xl">🥘</div>
            <div class="flex-1">
              <div class="text-sm font-semibold text-gray-900">ክትፎ</div>
              <div class="text-xs text-gray-500">Kitfo</div>
              <div class="text-sm font-bold text-primary-600 mt-1">380 Birr</div>
            </div>
          </div>
        </div>
        
        <!-- QR Code indicator -->
        <div class="absolute -right-16 top-8 bg-white p-3 rounded-lg shadow-lg">
          <div class="w-12 h-12 bg-gray-900 rounded grid grid-cols-3 gap-[2px] p-1">
            {#each Array(9) as _}
              <div class="bg-white rounded-sm"></div>
            {/each}
          </div>
          <div class="text-[10px] text-gray-500 text-center mt-1">Scan me</div>
        </div>
      </div>
    </div>
  </FeatureSection>

  <!-- Feature 2: Payment-first ordering -->
  <FeatureSection 
    title="Payment-first ordering eliminates unpaid orders"
    subtitle="POWERED BY TELEBIRR"
    linkText="See payment integration"
    reversed={true}
    bullets={[
      "Customers pay via Telebirr before orders reach kitchen",
      "100% payment completion rate—no more unpaid bills",
      "Instant payment confirmation and order routing",
      "Secure transactions with Ethiopia's trusted payment platform"
    ]}
  >
    <div slot="description">
      <p>Transform payment uncertainty into guaranteed revenue. Every order is prepaid through Telebirr integration, giving you peace of mind and improving cash flow.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Payment flow diagram -->
       <div class="flex flex-col items-center gap-4">
         <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-primary-100 rounded flex items-center justify-center text-primary-600">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M7 7h.01M7 12h.01M7 17h.01M12 7h.01M12 12h.01M12 17h.01M17 7h.01M17 12h.01M17 17h.01"/></svg>
            </div>
            <div class="text-sm">
               <div class="font-semibold">Customer scans QR</div>
               <div class="text-xs text-gray-500">Views menu & selects items</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-white p-4 rounded-lg shadow-sm border border-primary-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-primary-600 rounded flex items-center justify-center text-white">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
            </div>
            <div class="text-sm">
               <div class="font-semibold">Pay via Telebirr</div>
               <div class="text-xs text-gray-500">Secure prepayment required</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-green-50 p-2 rounded-full text-xs text-green-700 font-medium px-4 border border-green-200 flex items-center gap-2">
            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
            Order confirmed
         </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 3: Real-time order management -->
  <FeatureSection 
    title="Real-time order management from table to kitchen"
    subtitle="STREAMLINE OPERATIONS"
    linkText="View order dashboard"
    bullets={[
      "Instant order notifications to kitchen staff",
      "Track order status from placement to completion",
      "Table management and order history",
      "Print or display orders on kitchen screens"
    ]}
  >
    <div slot="description">
      <p>Keep your kitchen running smoothly with instant order routing, status tracking, and seamless coordination between front and back of house.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Order dashboard mockup -->
       <div class="bg-white rounded-2xl shadow-lg p-4 w-72 space-y-3">
          <div class="flex items-center justify-between mb-2">
            <div class="text-sm font-bold text-gray-900">Active Orders</div>
            <div class="text-xs bg-primary-100 text-primary-700 px-2 py-1 rounded-full font-medium">3 pending</div>
          </div>
          <div class="flex items-start gap-3 p-3 bg-green-50 rounded-lg border border-green-200">
             <div class="w-10 h-10 bg-green-600 rounded-lg flex items-center justify-center text-white font-bold text-sm">12</div>
             <div class="flex-1">
                <div class="text-xs font-bold text-gray-900">Doro Wat × 2</div>
                <div class="text-[10px] text-gray-500">Paid: 900 Birr • 2 min ago</div>
             </div>
             <div class="text-xs text-green-700 font-medium">New</div>
          </div>
          <div class="flex items-start gap-3 p-3 bg-yellow-50 rounded-lg border border-yellow-200">
             <div class="w-10 h-10 bg-yellow-600 rounded-lg flex items-center justify-center text-white font-bold text-sm">8</div>
             <div class="flex-1">
                <div class="text-xs font-bold text-gray-900">Kitfo, Tibs</div>
                <div class="text-[10px] text-gray-500">Paid: 650 Birr • 8 min ago</div>
             </div>
             <div class="text-xs text-yellow-700 font-medium">Cooking</div>
          </div>
          <div class="flex items-start gap-3 p-3 bg-gray-50 rounded-lg border border-gray-200">
             <div class="w-10 h-10 bg-gray-400 rounded-lg flex items-center justify-center text-white font-bold text-sm">5</div>
             <div class="flex-1">
                <div class="text-xs font-bold text-gray-900">Shiro, Injera</div>
                <div class="text-[10px] text-gray-500">Paid: 320 Birr • 15 min ago</div>
             </div>
             <div class="text-xs text-gray-700 font-medium">Ready</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 4: Easy menu management -->
  <FeatureSection 
    title="Update your menu instantly across all tables"
    subtitle="SIMPLE MENU MANAGEMENT"
    linkText="Explore menu tools"
    reversed={true}
    bullets={[
      "Change prices, add dishes, or update descriptions in seconds",
      "Upload dish photos to make menus more appealing",
      "Mark items as sold out or unavailable in real-time",
      "Seasonal menus and special promotions made easy"
    ]}
  >
    <div slot="description">
      <p>No more reprinting menus or crossing out prices. Update your digital menu once and all QR codes reflect changes instantly.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Menu editor mockup -->
       <div class="bg-white rounded-xl shadow-lg w-[85%] overflow-hidden border border-gray-100">
          <div class="bg-gray-50 p-3 border-b border-gray-100 flex items-center justify-between">
             <div class="text-xs font-semibold text-gray-900">Menu Editor</div>
             <div class="flex gap-2">
               <div class="text-xs bg-primary-600 text-white px-3 py-1 rounded-md font-medium">Save changes</div>
             </div>
          </div>
          <div class="p-6 space-y-3">
             <div class="flex items-center gap-3 p-3 bg-gray-50 rounded-lg border border-gray-200">
                <div class="w-12 h-12 bg-primary-200 rounded flex items-center justify-center text-lg">🍲</div>
                <div class="flex-1">
                   <div class="text-sm font-semibold text-gray-900">Doro Wat</div>
                   <div class="flex items-center gap-2 mt-1">
                     <input type="text" value="450" class="w-16 text-xs border border-gray-300 rounded px-2 py-1" />
                     <span class="text-xs text-gray-500">Birr</span>
                   </div>
                </div>
                <div class="flex gap-1">
                  <button class="w-6 h-6 bg-gray-200 rounded flex items-center justify-center text-gray-600 text-xs">✎</button>
                  <button class="w-6 h-6 bg-red-100 rounded flex items-center justify-center text-red-600 text-xs">×</button>
                </div>
             </div>
             <div class="flex items-center gap-3 p-3 bg-yellow-50 rounded-lg border border-yellow-200">
                <div class="w-12 h-12 bg-yellow-200 rounded flex items-center justify-center text-lg">🥘</div>
                <div class="flex-1">
                   <div class="text-sm font-semibold text-gray-900">Kitfo</div>
                   <div class="text-xs text-yellow-700 font-medium">Sold out today</div>
                </div>
                <div class="text-xs bg-yellow-600 text-white px-2 py-1 rounded">Unavailable</div>
             </div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 5: Analytics and insights -->
  <FeatureSection 
    title="Understand what drives sales and optimize your menu"
    subtitle="DATA-DRIVEN DECISIONS"
    linkText="View analytics dashboard"
    bullets={[
      "Track best-selling dishes and peak ordering times",
      "Revenue analytics by day, week, and month",
      "Customer preferences and ordering patterns",
      "Identify underperforming menu items"
    ]}
  >
    <div slot="description">
      <p>Make smarter business decisions with real-time insights into what your customers love, when they order, and how to maximize revenue.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center px-8">
       <!-- Chart -->
       <div class="w-full h-64 flex items-end justify-between gap-2">
          {#each [65, 45, 70, 55, 80, 60, 75, 50, 85, 65, 70, 60] as height}
             <div class="w-full bg-primary-100 rounded-t-sm relative group">
                <div style="height: {height}%" class="absolute bottom-0 w-full bg-primary-500 rounded-t-sm transition-all duration-500 group-hover:bg-primary-600"></div>
             </div>
          {/each}
       </div>
       <!-- Legend overlay -->
       <div class="absolute top-12 right-12 bg-white p-4 rounded-lg shadow-sm border border-gray-100 text-xs">
          <div class="flex justify-between gap-8 mb-2">
             <span class="text-gray-500">Total Revenue</span>
             <span class="font-bold text-gray-900">245,000 Birr</span>
          </div>
          <div class="flex justify-between gap-8 mb-2">
             <span class="text-gray-500">Total Orders</span>
             <span class="font-bold text-gray-900">1,247</span>
          </div>
          <div class="flex justify-between gap-8">
             <span class="text-gray-500">Avg Order Value</span>
             <span class="font-bold text-gray-900">196 Birr</span>
          </div>
          <div class="mt-3 pt-3 border-t border-gray-100">
            <div class="text-xs font-semibold text-gray-900 mb-1">Top Dish</div>
            <div class="text-xs text-primary-600">Doro Wat (342 orders)</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 6: Security and reliability -->
  <FeatureSection 
    title="Built for reliability and secure payments"
    subtitle="TRUSTED PLATFORM"
    linkText="Learn about security"
    reversed={true}
    bullets={[
      "Secure payment processing through Telebirr integration",
      "99.9% uptime for uninterrupted service",
      "Data protection and customer privacy built-in",
      "Regular backups and disaster recovery"
    ]}
  >
    <div slot="description">
      <p>Trust QR Anbessa to keep your restaurant running smoothly with secure payments, reliable infrastructure, and data protection you can count on.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Security features grid -->
       <div class="grid grid-cols-2 gap-6">
          <div class="flex flex-col items-center gap-3 p-4 bg-white rounded-xl border border-gray-200">
            <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
            </div>
            <div class="text-sm font-bold text-gray-900 text-center">Secure Payments</div>
          </div>
          <div class="flex flex-col items-center gap-3 p-4 bg-white rounded-xl border border-gray-200">
            <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
            </div>
            <div class="text-sm font-bold text-gray-900 text-center">Data Protection</div>
          </div>
          <div class="flex flex-col items-center gap-3 p-4 bg-white rounded-xl border border-gray-200">
            <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600"><polyline points="23 6 13.5 15.5 8.5 10.5 1 18"></polyline><polyline points="17 6 23 6 23 12"></polyline></svg>
            </div>
            <div class="text-sm font-bold text-gray-900 text-center">99.9% Uptime</div>
          </div>
          <div class="flex flex-col items-center gap-3 p-4 bg-white rounded-xl border border-gray-200">
            <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-primary-600"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path><polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline><line x1="12" y1="22.08" x2="12" y2="12"></line></svg>
            </div>
            <div class="text-sm font-bold text-gray-900 text-center">Daily Backups</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <CaseStudies />
  <Integrations />
  <Resources />
  <BottomCTA />
</main>

<Footer />

