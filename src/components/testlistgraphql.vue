<template>
    <div>
        <testgraphql
                v-for="link in allLinks" :key="link.id" :link="link">
        </testgraphql>
    </div>
</template>

<script>
    import testgraphql from './testgraphql'

    export default {
        name: 'testlistgraphql',
        data () {
            return {
                allLinks: [
                    {
                        id: '1',
                        description: 'The Coolest GraphQL Backend 😎',
                        url: 'https://www.graph.cool'
                    }, {
                        id: '2',
                        description: 'The Best GraphQL Client',
                        url: 'http://dev.apollodata.com/'
                    }
                ]
            }
        },
        components: {
            testgraphql
        }
    }
</script>