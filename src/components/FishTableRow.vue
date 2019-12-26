<template>
    <div>
        <tr>
            <td className="fish-name">{{fish.name}}</td>
            <td>
                <img :src="fish.image"/>
            </td>
            {this.state.showDescription ?
            <td className="fish-description">Does anyone know where my dad is?</td>
            : null}
        </tr>
    </div>
</template>

<script>
    export default {
        name: "FishTableRow",
        props: ['fish']
    }
</script>

<style scoped>

</style>