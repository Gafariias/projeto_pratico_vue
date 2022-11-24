<template>
    <button @click="$i18n.locale = locales[0]">Português</button>
    <button @click="$i18n.locale = locales[1]">Inglês</button>
    <button @click="$i18n.locale = locales[2]">Espanhol</button>
</template>

<script>
    export default {
        name: 'LocaleSwitcher',
        data() {
            return {
                locales: ["pt", "en", "es"],
            }
        }
    }
</script>