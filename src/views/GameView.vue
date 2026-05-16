import { createRouter, createWebHistory } from 'vue-router'
import HomeView from '../views/HomeView.vue'
import GameView from '../views/GameView.vue'

const routes = [
      {
            path: '/',
                name: 'home',
                    component: HomeView,
                        meta: { title: 'OPERATOR // PORTAFOLIO 3D' }
      },
        {
                path: '/tank-arena',
                    name: 'game',
                        component: GameView,
                            meta: { title: 'CYBER_CORE // TANK ARENA' }
        }
]

const router = createRouter({
      history: createWebHistory(),
        routes,
          scrollBehavior() {
                return { top: 0, behavior: 'smooth' }
          }
})

// Guardia de navegación para actualizar el título de la pestaña dinámicamente
router.beforeEach((to, from, next) => {
      document.title = to.meta.title || 'CYBER_PORTFOLIO'
        next()
})

export default router

})
          }
})
        }
      }
]