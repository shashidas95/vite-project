<template>
  <div>
    <head>
      <meta charset="utf-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
      <title>{{ seo.title }}</title>
      <meta name="description" content="{{ seo.description }}" />
      <meta name="keywords" content="{{ seo.keywords }}" />
      <meta name="og:site_name" content="{{ seo.ogSiteName }}" />
      <meta name="og:url" content="{{ seo.ogUrl }}" />
      <meta name="og:title" content="{{ seo.ogTitle }}" />
      <meta name="og:description" content="{{ seo.ogDescription }}" />
      <meta name="og:Image" content="{{ seo.ogImage }}" />
      <meta name="author" content="" />
      <link rel="icon" type="image/x-icon" :href="assetUrl('assets/favicon.ico')" />
      <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css" rel="stylesheet" />
      <link :href="assetUrl('css/bootstrap.min.css')" rel="stylesheet" />
      <link :href="assetUrl('css/style.css')" rel="stylesheet" />
      <script :src="assetUrl('js/axios.min.js')"></script>
    </head>
    <body>
      <navbar></navbar>
      <loader></loader>
      <div id="content-div">
        <slot></slot>
      </div>
      <footer-component></footer-component>
      <!-- Uncomment the following lines if you want to include the Bootstrap JavaScript files -->
      <!-- <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script> -->
      <script :src="assetUrl('js/bootstrap.bundle.min.js')"></script>
      <script :src="assetUrl('js/scripts.js')"></script>
    </body>
  </div>
</template>

<script setup>



  
</script>
