<script setup>
import { ref, computed } from "vue";
import GlassTable from "../components/customTable.vue";

const headers = ["STT", "STT", "STT", "STT"];
const data = Array(3).fill(["1", "1", "1", "1"]);

const search = ref("");
const searchLength = computed(() => search.value.length);
</script>

<template>
  profile
  <div class="relative w-full mt-5">
    <!-- Banner -->
    <div class="w-full h-50 overflow-hidden rounded-lg">
      <img
        class="w-full h-full object-cover"
        src="../assets/img/3-loi-ich-cua-hoat-dong-dao-tao-nhan-vien.jpg"
        alt="Banner" />
    </div>

    <!-- Thẻ thông tin đè lên -->
    <div
      class="absolute bottom-[-80px] justify-left bg-white/90 left-1/2 transform -translate-x-1/2 w-[90%] md:w-[80%] lg:w-[70%] shadow-lg rounded-xl p-7 flex items space-x-10">
      <img
        src="/src/assets/img/R.jpg"
        class="w-20 h-20 rounded-xl object-cover" />
      <br />
      <div class="space-y-3">
        <p class="text-lg font-semibold text-black">User name</p>
        <p class="font-medium text-gray-500">CEO/Staff</p>
      </div>
    </div>
  </div>
  <div class="flex flex-row  relative w-full">
    <div class="ml-23 mt-31 w-md m-5 ">
      <!-- User Info Form -->
      <div class="bg-white p-11 rounded-lg shadow ">
        <input
          type="text"
          placeholder="ID"
          class="w-full p-2 mb-2 border rounded" />
        <input
          type="text"
          placeholder="Tên"
          class="w-full p-2 mb-2 border rounded" />
        <input
          type="email"
          placeholder="Email"
          class="w-full p-2 mb-2 border rounded" />
        <input
          type="tel"
          placeholder="Số điện thoại"
          class="w-full p-2 mb-2 border rounded" />
        <button
          class=" px-6 py-2 rounded-lg font-semibold text-white bg-gradient-to-r from-gray-900 to-gray-700 shadow-xl backdrop-blur-md bg-opacity-80 border border-white/30 transition-all duration-200 ease-out hover:bg-opacity-90 hover:scale-105 active:scale-95 active:shadow-md">
          + THÊM
        </button>
      </div>
    </div>

    <div class="w-150  mt-31 relative w-full">
      <div class="bg-white p-11 rounded-xl shadow ">
       <div> <input
          type="find"
          class="w-54 p-0.3 mb-2 border rounded rounded-xl" />
          <button
          class=" ml-1 px-2 py-0.3 rounded-xl font-semibold text-white bg-gradient-to-r from-gray-900 to-gray-700 shadow-xl backdrop-blur-md bg-opacity-80 border border-white/30 transition-all duration-200 ease-out hover:bg-opacity-90 hover:scale-105 active:scale-95 active:shadow-md">
         Tìm kiếm
        </button>
    
        <button
          class="float-right ml-5 px-5 py-0.3 rounded-xl font-semibold text-black  shadow-xl backdrop-blur-md bg-opacity-80 border border-black/30 transition-all duration-200 ease-out hover:bg-opacity-90 hover:scale-105 active:scale-95 active:shadow-md">
         End
        </button>
        <button
          class="float-right ml-5 px-4 py-0.3 rounded-xl font-semibold text-black  shadow-xl backdrop-blur-md bg-opacity-80 border border-black/30 transition-all duration-200 ease-out hover:bg-opacity-90 hover:scale-105 active:scale-95 active:shadow-md">
         Start
        </button>
        
</div>
        <table class="w-full border-collapse">
            <thead>
              <tr class="bg-gray-200">
                <th class="border p-2">MÃ HÓA ĐƠN</th>
                <th class="border p-2">NGƯỜI DÙNG</th>
                <th class="border p-2">SỐ ĐIỆN THOẠI</th>
                <th class="border p-2">DATE</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="border p-2">#1234</td>
                <td class="border p-2">Nguyễn Văn A</td>
                <td class="border p-2">0123456789</td>
                <td class="border p-2">10/03/2025</td>
              </tr>
            </tbody>
          </table>
      </div>
    </div>
  </div>
</template>
