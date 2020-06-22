<template>
    <v-list disabled class="text-left">
    <v-subheader>{{heading}}</v-subheader>
    <v-list-item-group v-model="item" color="green">
        <v-list-item
            v-for="(item, i) in items"
            :key="i"
        >
        <v-list-item-icon>
            <v-icon v-text="item.icon"></v-icon>
        </v-list-item-icon>
        <v-list-item-content>
            <v-list-item-title v-text="item.text"></v-list-item-title>
        </v-list-item-content>
        </v-list-item>
    </v-list-item-group>
    </v-list>
</template>

<script>
export default {
    props: ['heading'],
    data() {
        return {
            item: 1,
            items: [
                {
                    icon: 'mdi-calendar-text',
                    text: 'サイト名称決定',
                    // sort: 1,
                },
                {
                    icon: 'mdi-calendar-text',
                    text: '情報掲載',
                    // sort: 1,
                },
                {
                    icon: 'mdi-calendar-text',
                    text: 'UI・デザイン改善',
                    // sort: 2,
                },
                {
                    icon: 'mdi-calendar-text',
                    text: 'アイコン更新',
                    // sort: 2,
                },
            ]
        }
    }
}
</script>