<template>
    <nav class="bg-indigo-400 flex justify-evenly p-4">
        <div>
            <Link href="/" class="text-xl text-white">
                logo
            </Link>
        </div>

        <div>

            <Link href="/chat" class="ext-xl text-white mr-6 hover:bg-white hover:text-indigo-400 px-4 py-2 rounded-3xl">
                Chat
            </Link>

            <Link href="/contacto" class="ext-xl text-white mr-6 hover:bg-white hover:text-indigo-400 px-4 py-2 rounded-3xl">
                Contacto
            </Link>

            <Link href="/nosotros" class="ext-xl text-white mr-6 hover:bg-white hover:text-indigo-400 px-4 py-2 rounded-3xl">
                nosotros
            </Link>

            <Link href="/usuarios" class="ext-xl text-white mr-6 hover:bg-white hover:text-indigo-400 px-4 py-2 rounded-3xl">
                usuarios
            </Link>
            
        </div>

    </nav>
</template>

<script>
import {Link} from "@inertiajs/vue3";
export default {
    components: {
        Link,
    }
}

</script>

<style>

</style>