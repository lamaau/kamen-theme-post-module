<template>
  <div class="flex flex-col">
    <kamen-heading title="Category" />

    <ul class="flex flex-col bg-white rounded-2xl shadow">
      <li
        v-for="(category, index) in $page.props.categories"
        :key="index"
        class="p-3 border-b"
      >
        <div class="flex flex-row justify-between items-center">
          <a
            href="#"
            class="
              font-semibold
              text-gray-800
              hover:text-pink-500
              transition-all
            "
          >
            {{ category.name }}
          </a>
          <span class="bg-pink-500 text-pink-200 px-2 py-1 rounded-md">
            {{ category.posts_count }}
          </span>
        </div>
      </li>
    </ul>
  </div>
</template>
