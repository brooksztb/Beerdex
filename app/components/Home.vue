<script>
    import * as utils from "utils/utils";
    import Map from './Map'

    export default {
        methods: {
        },
        components: {
            Map
        }
    }
    
    
</script>

<template>
    <page>
        <ActionBar class="action-bar" title="Beerdex">
        </ActionBar>
        <TabView :selectedIndex="selectedIndex" androidTabsPosition="bottom">
            <TabViewItem title="Beer Map">
                <map></map>
            </TabViewItem>
            <TabViewItem title="Beer List">
                <label text="This is where the List view Goes" />
            </TabViewItem>
            <TabViewItem title="Account">
                <label text="These are where the user settings are" />
            </TabViewItem>
        </TabView>
    </page>
</template>

<style scoped>
    .sideStackLayout {
        z-index: 1;
    }
</style>