<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';

</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
      <div class="py-12 fade-in">
        <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
          <div class="bg-white dark:bg-gray-800 overflow-hidden shadow-sm sm:rounded-lg">

            <!-- Header -->
            <div class="p-6 text-gray-900 dark:text-gray-100">
              <h2 class="text-2xl font-semibold">Motor Dashboard</h2>
            </div>

            <hr>

            <!-- Motor Shop Stats -->
            <div class="p-6">
              <div class="grid grid-cols-2 gap-4">
                <div class="bg-blue-200 dark:bg-blue-800 p-4 rounded-lg">
                  <h3 class="text-xl font-semibold text-blue-700 dark:text-blue-300">Total Sales</h3>
                  <p class="text-2xl font-bold text-blue-900 dark:text-blue-400">$10,000</p>
                </div>
                <div class="bg-green-200 dark:bg-green-800 p-4 rounded-lg">
                  <h3 class="text-xl font-semibold text-green-700 dark:text-green-300">Inventory</h3>
                  <p class="text-2xl font-bold text-green-900 dark:text-green-400">100 vehicles</p>
                </div>
                <!-- Add more stats here -->
              </div>
            </div>

            <!-- Recent Orders -->
            <div class="p-6">
              <h3 class="text-xl font-semibold">Recent Orders</h3>
              <ul class="mt-4">
                <li class="mb-2">
                  <span class="text-gray-600 dark:text-gray-300">Order #12345</span> - $500
                </li>
                <li class="mb-2">
                  <span class="text-gray-600 dark:text-gray-300">Order #12346</span> - $750
                </li>
                <!-- Add more recent orders here -->
              </ul>
            </div>

            <!-- Additional Dashboard Widgets -->
            <!-- Add more widgets and content here -->

          </div>
        </div>
      </div>
    </AuthenticatedLayout>
  </template>


<style>
    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
    }

    .fade-in {
        animation: fadeIn 0.3s ease-in-out; /* Adjust the duration and timing function as needed */
    }
</style>
