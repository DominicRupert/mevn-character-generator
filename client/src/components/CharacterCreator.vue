<template>
    <div class="character-creator">
        <h1>Character Creator</h1>
        <label for="character-name">Character Name: </label>
        <input type="text" id="character-name" v-model="name" placeholder="Enter a name"/>
        <label for="professions-list">Professions: </label>
        <select id="professions-list" v-model="profession">
            <option value="Mage">Mage</option>
            <option value="Warrior">Warrior</option>
            <option value="Rogue">Rogue</option>

        </select>
        <p>{{name}}</p>
        <p>{{profession}}</p>

        
    </div>
</template>
<script>
    export default {
        name: 'CharacterCreator',
        data: function() {
            return {
                name: "dom",
                profession: ""
            }
        }
    }
</script>
<style scoped>
    
</style>