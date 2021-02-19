<template>
   <div class="content page_contain">
                <div class="bg">
                    <video poster="/img/cubes.jpg" playsinline="" autoplay="" muted="" loop="">
                        <source src="/video/cubes.mp4" type="video/mp4">
                    </video>
                </div>
                <div class="title m-b-md">
                    cube.io
                </div>
                <p>in the works..</p>

            </div>
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'

export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      required: true
    }
  },
  setup: () => {
    const count = ref(0)
    return { count }
  }
})
</script>

<style scoped>
            html, body {
                color: #636b6f;
                font-family: 'Raleway', sans-serif;
                font-weight: 100;
                height: 100vh;
                margin: 0;
            }

            .full-height {
                height: 100vh;
            }

            .flex-center {
                align-items: center;
                display: flex;
                justify-content: center;
            }

            .position-ref {
                position: relative;
            }

            .top-right {
                position: absolute;
                right: 10px;
                top: 18px;
            }

            .content {
                text-align: center;
            }

            .title {
                font-size: 84px;
            }

            .links > a {
                color: #636b6f;
                padding: 0 25px;
                font-size: 12px;
                font-weight: 600;
                letter-spacing: .1rem;
                text-decoration: none;
                text-transform: uppercase;
            }

            .m-b-md {
                margin-bottom: 30px;
            }
            .page_contain{
                position: relative;
                max-width: 100em;
                margin: 0 auto;
                padding: 0 5.5%;
            }
            .bg video {
                max-width: 100%;
            }
            @media (min-width: 50em){
                .bg {
                    display: block;
                    position: absolute;
                    z-index: -2;
                    top: 50%;
                    left: 0;
                    width: 180%;
                    -webkit-transform: translate(-50%,-50%);
                    transform: translate(-50%,-50%);
                }
            }
</style>