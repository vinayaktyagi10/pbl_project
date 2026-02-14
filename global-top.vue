<template>
  <div class="header-logos">
    <img src="/sdc_logo.jpg" class="sdc-logo" />
    <img src="/muj_logo.png" class="muj-logo" />
  </div>
  <a href="../" class="back-home-link">
    🏠 Home
  </a>
</template>

<style>
.header-logos {
  position: absolute;
  top: 1.5rem;
  right: 1.5rem;
  display: flex;
  align-items: center;
  gap: 1rem;
  z-index: 100;
}
.sdc-logo {
  height: 40px;
  width: auto;
  border-radius: 0.25rem;
  border: 1px solid rgba(255, 255, 255, 0.1);
}
.muj-logo {
  height: 30px;
  width: auto;
  background: white;
  padding: 2px;
  border-radius: 0.25rem;
  border: 1px solid rgba(255, 255, 255, 0.1);
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