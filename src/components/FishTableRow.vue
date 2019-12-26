<template>
    <div>
        <tr>
            <td className="fish-name">Nemo</td>
            <td>
                <img src="http://tinyurl.com/h8o5szh"/>
            </td>
            {this.state.showDescription ?
            <td className="fish-description">Does anyone know where my dad is?</td>
            : null}
        </tr>
    </div>
</template>

<script>
    export default {
        name: "FishTableRow"
    }
</script>

<style scoped>

</style>