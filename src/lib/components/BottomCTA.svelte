<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="relative rounded-3xl overflow-hidden h-[500px]">
      <img 
        src="/generated/image-ethiopian-restaurant-staff-and-owner-cel-1765563394092-6.webp" 
        alt="Ethiopian restaurant owner" 
        class="absolute inset-0 w-full h-full object-cover"
      />
      <div class="absolute inset-0 bg-black/40"></div>
      
      <div class="absolute inset-0 flex flex-col justify-center px-8 md:px-16 max-w-3xl">
        <h2 class="text-4xl md:text-5xl font-bold text-white mb-8 leading-tight">
          Join Ethiopian restaurants eliminating unpaid orders with QR Anbessa.
        </h2>
        <div class="flex flex-col sm:flex-row gap-4">
          <Button variant="primary" size="lg" class="rounded-full px-8">Get started today</Button>
          <Button variant="outline" size="lg" class="rounded-full px-8 bg-white text-gray-900 border-none hover:bg-gray-100">Schedule demo</Button>
        </div>
      </div>
    </div>
  </div>
</section>
