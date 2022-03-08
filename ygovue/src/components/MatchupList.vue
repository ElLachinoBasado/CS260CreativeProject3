<template>
    <div class = "main">
        <div class="matchups" v-for="matchup in matchups" :key="matchup.id">            
            <div class = "image">
                <img :src="'/Matchup/'+matchup.image">
            </div>
        </div>    
    </div>
</template>

<script>
export default {
    name: 'MatchupList',
    props: {
        matchups: Array
    },
}
</script>
