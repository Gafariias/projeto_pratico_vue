<template>
    <nav class="mx-auto flex">
        <button 
          @click="$i18n.locale = locales[0]"
          class="transition-all hover:brightness-90 mr-4 box-border w-32 h-12 bg-dark-500 flex items-center justify-center rounded-2xl text-white-900"
        >
            <img class="mr-1" src="@/assets/icons/brazil.svg" alt=""/>
            {{$t('portuguese')}}
        </button>

        <button 
          @click="$i18n.locale = locales[1]"
          class="transition-all hover:brightness-90 mr-4 box-border w-32 h-12 bg-dark-500 flex items-center justify-center rounded-2xl text-white-900"
        >
            <img class="mr-1" src="@/assets/icons/english.svg" alt=""/>
            {{$t('english')}}
        </button>

        <button 
          @click="$i18n.locale = locales[2]"
          class="transition-all hover:brightness-90 mr-4 box-border w-32 h-12 bg-dark-500 flex items-center justify-center rounded-2xl text-white-900"
        >
            <img class="mr-1" src="@/assets/icons/spanish.svg" alt=""/>
            {{$t('spanish')}}
        </button>
    </nav>
</template>

<script>
import { useI18n } from 'vue-i18n'

    export default {
        name: 'LocaleSwitcher',
        setup() {
            const { t } = useI18n({
            inheritLocale: true,
            useScope: 'local'
            })

            // Something todo ..

            return { t }
        },
        data() {
            return {
                locales: ["pt", "en", "es"],
            }
        }
    }
</script>