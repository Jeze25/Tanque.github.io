<script setup>
import { RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
</script>

<template>
  <div class="min-h-screen bg-black text-slate-200 font-mono relative overflow-x-hidden">
      <!-- Navbar global HUD -->
          <Navbar />
              
                  <!-- Renderizador dinámico de vistas (Home o Juego) -->
                      <RouterView />
                        </div>
                        </template>
                        