<script setup>
import { computed } from "vue";
import { InformationCircleIcon, XMarkIcon, CheckCircleIcon, ExclamationTriangleIcon, XCircleIcon } from "@heroicons/vue/24/solid";
import { cva } from "class-variance-authority";



const props =defineProps({
    intent: {
        type: String,
        validator(value){
            return ["info", "success", "warning", "danger"].includes(value)
        },
        default: "info"
    },
    title:String,
    show:{
        type:Boolean,
        default: true
    },
    onDismiss: Function,
})



const containerClass = computed(() => {
    return cva("flex p-4 space-x-3 w-[22rem] rounded-lg shadow my-2", {
        variants: {
            intent: {
                info: "bg-blue-100",
                success: "bg-green-100",
                warning: "bg-orange-100",
                danger: "bg-red-100",
            }
        }
    })({
        intent: props.intent
    })
})

const iconClass = computed(() => {
    return cva("w-6 h-6", {
        variants: {
            intent: {
                info: "text-blue-700",
                success: "text-green-700",
                warning: "text-orange-700",
                danger: "text-red-700",
            }
        }
    })({
        intent:  props.intent
    })
})

const titleClass = computed(() => {
    return cva("font-medium", {
        variants: {
            intent: {
                info: "text-blue-900",
                success: "text-green-900",
                warning: "text-orange-900",
                danger: "text-red-900",
            }
        }
    })({
        intent:  props.intent
    })
})

const contentClass = computed(() => {
    return cva("text-sm", {
        variants: {
            intent: {
                info: "text-blue-800",
                success: "text-green-800",
                warning: "text-orange-800",
                danger: "text-red-800",
            }
        }
    })({
        intent:  props.intent
    })
})

const closeButtonClass = computed(() => {
    return cva("rounded p-0.5 -m-1", {
        variants: {
            intent: {
                info: "text-blue-900/70 hover:bg-blue-200 hover:text-blue-900",
                success: "text-green-900/70 hover:bg-green-200 hover:text-green-900",
                warning: "text-orange-900/70 hover:bg-orange-200 hover:text-orange-900",
                danger: "text-red-900/70 hover:bg-red-200 hover:text-red-900",
            }
        }
    })({
        intent:  props.intent
    })
})

const iconComponent = computed(() => {
    const icons = {
        info: InformationCircleIcon,
        success: CheckCircleIcon,
        warning: ExclamationTriangleIcon,
        danger: XCircleIcon
    };
    return icons[props.intent];

    // switch (intent) {
    //     case "info":
    //         return InformationCircleIcon
    //     case "success":
    //         return CheckCircleIcon
    //     case "warning":
    //         return ExclamationTriangleIcon
    //     case "danger":
    //         return XCircleIcon
    // }
})


function dismiss() {
    if (props.onDismiss) {
        props.onDismiss()        
    }
}
</script>

<template>
    <transition leave-active-class="duration-300" leave-to-class="opacity-0">
    <div v-if="props.show" :class="containerClass">
            <div class="shrink-0">
                <component :is="iconComponent" :class="iconClass" />
            </div>
            <div class="flex-1 space-y-2">  
                <h2 :class="titleClass">{{ props.title }}</h2>
                <div :class="contentClass">
                    <slot/>
                </div>
            </div>
            <div class="shrink-0" v-if="props.onDismiss">
                <button @click="dismiss()" :class="closeButtonClass">
                    <XMarkIcon class="w-6 h-6" />
                </button>
            </div>
        </div>
    </transition>
</template>


<style lang="scss" scoped></style>