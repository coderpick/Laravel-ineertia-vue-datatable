<script setup>
import { ref } from "vue";
import Toaster from "@/Components/Toaster.vue";
const showAlert = ref(true);

</script>

<template>
    <div class="">
        <Toaster :show="showAlert" :on-dismiss="() => showAlert = false" intent="success" title="Success">
            This is a success toast.
        </Toaster>
        
        <Toaster :show="showAlert" :on-dismiss="() => showAlert = false" intent="warning" title="Success">
            This is a warning toast.
        </Toaster>

        <Toaster :show="showAlert" :on-dismiss="() => showAlert = false" intent="danger" title="Success">
            This is a danger toast.
        </Toaster>


        <Toaster :show="showAlert" :on-dismiss="() => showAlert = false" title="Info">
            This is a info toast.
        </Toaster> 
    </div>
</template>

