<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<footer class="bg-white pt-24 pb-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 mb-16">
      <!-- Column 1 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Product</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">QR Menus</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Payment Integration</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Order Management</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Analytics</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Pricing</a>
      </div>

      <!-- Column 2 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Solutions</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">For Hotels</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">For Restaurants</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">For Cafes</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">For Bars</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Enterprise</a>
      </div>

      <!-- Column 3 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Resources</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Help Center</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Documentation</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Blog</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Case Studies</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Video Tutorials</a>
      </div>

      <!-- Column 4 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Company</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">About Us</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Careers</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Contact</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Partners</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Press Kit</a>
      </div>

       <!-- Column 5 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Support</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Get Started</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">FAQs</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Contact Support</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">System Status</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">API Docs</a>
      </div>

       <!-- Column 6 (Newsletter) -->
      <div class="flex flex-col gap-4 lg:col-span-1">
        <h4 class="font-semibold text-gray-900 text-sm">Newsletter</h4>
        <p class="text-sm text-gray-500">Get tips on growing your restaurant business delivered to your inbox.</p>
        <div class="flex flex-col gap-2">
           <Button variant="secondary" size="sm" class="w-full !bg-black !text-white !rounded-lg">Sign up</Button>
        </div>
      </div>
    </div>

    <!-- Bottom -->
    <div class="pt-8 border-t border-gray-100 flex flex-col md:flex-row justify-between items-center gap-4">
      <div class="flex items-center gap-2">
         <div class="w-6 h-6 bg-primary-600 rounded flex items-center justify-center text-white">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" width="14" height="14">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M9.61185 4.17065C8.2158 4.17065 6.92581 4.91543 6.22779 6.12444L3.72109 10.4662C3.02307 11.6752 3.02307 13.1647 3.72109 14.3737L6.22779 18.7155C6.92581 19.9245 8.2158 20.6693 9.61185 20.6693H14.6252C16.0213 20.6693 17.3113 19.9245 18.0093 18.7155L20.516 14.3737C21.214 13.1647 21.214 11.6752 20.516 10.4662L18.0093 6.12444C17.3113 4.91543 16.0213 4.17065 14.6252 4.17065H9.61185ZM14.6252 6.77569H11.4919C10.9905 6.77569 10.6773 7.31837 10.9283 7.75232C11.7029 9.09123 12.4793 10.4291 13.2527 11.7687C13.4854 12.1717 13.4854 12.6682 13.2527 13.0712C12.4793 14.4108 11.7029 15.7487 10.9283 17.0876C10.6773 17.5215 10.9905 18.0642 11.4919 18.0642H14.6252C15.0906 18.0642 15.5206 17.8159 15.7533 17.4129L18.26 13.0712C18.4927 12.6682 18.4927 12.1717 18.26 11.7687L15.7533 7.42695C15.5206 7.02395 15.0906 6.77569 14.6252 6.77569Z"
                fill="currentColor"
              />
            </svg>
         </div>
         <span class="text-sm text-gray-500">© 2025 QR Anbessa</span>
      </div>

      <div class="flex flex-col md:flex-row items-center gap-4 text-xs text-gray-500 text-center md:text-right">
        <p class="max-w-md">
           By clicking "Accept", you agree to the use of cookies on your device or browser to enhance site navigation, analyze site usage, and assist in our marketing efforts.
        </p>
        <div class="flex gap-4">
           <Button variant="primary" size="sm" class="!text-xs !py-1 !h-8">Accept all cookies</Button>
           <Button variant="outline" size="sm" class="!text-xs !py-1 !h-8">Cookie settings</Button>
        </div>
      </div>
    </div>
    
    <div class="mt-4 flex justify-end gap-6 text-xs text-gray-500">
       <a href="#" class="hover:text-gray-900">Privacy Statement</a>
       <a href="#" class="hover:text-gray-900">Terms of Service</a>
    </div>
  </div>
</footer>
