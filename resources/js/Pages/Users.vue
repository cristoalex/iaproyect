<template>
    <Navbar/>
    <div class="p-8 relative overflow-x-auto">
        <table class="w-full text-sm text-left text-gray-500 dark:text-gray-400">
            <thead class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-500">
                <tr>
                    <th scope="col" class="px-6 py-3">
                        Nombre de usuario
                    </th>
                    <th scope="col" class="px-6 py-3">
                        Email
                    </th>
                    <th scope="col" class="px-6 py-3">
                        Materias
                    </th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="usuario in usuarios" :key="usuario.index" class="bg-white border-b dark:bg-gray-800 dark:border-gray-700">
                    <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
                        {{ usuario.name }}
                    </th>
                    <td class="px-6 py-4">
                        {{ usuario.email }}
                    </td>
                    <td>
                        <span class="bg-gray-100 text-gray-800 text-xsfont-medium mr-2
                        px-2.5 py-0.5 rounded dark:bg-gray-700 dark:text-gray-300" v-for="subject in usuario.subjects" 
                        :key="subject.id">{{ subject.name }}
                        </span>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script>
import Navbar from '../Shared/Navbar.vue';
export default{
    components: {
    Navbar,
    Navbar
},
    props:{
        usuarios: Object
    }
}
</script>
<style>
</style>