<template>
  <img src="./sdc_logo.jpg" class="sdc-logo" />
  <a href="../" class="back-home-link">
    🏠 Home
  </a>
</template>

<style>
.sdc-logo {
  position: absolute;
  top: 1.5rem;
  right: 1.5rem;
  width: 50px;
  z-index: 100;
}
.back-home-link {
  position: absolute;
  bottom: 1rem;
  left: 1rem;
  font-size: 0.8rem;
  opacity: 0.5;
  text-decoration: none;
  color: inherit;
  z-index: 100;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
.back-home-link:hover {
  opacity: 1;
}
</style>
