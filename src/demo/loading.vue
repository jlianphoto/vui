<template>
    <div class="demo-loading">
        <ul>
            <li>
                <button class="btn" @click="show">show loading</button>
            </li>
            <li>
                <button class="btn" @click="hide">hide loading</button>
            </li>
        </ul>
    </div>
</template>


<script type="text/javascript">
    import loading from '../packages/loading';

    export default {
        methods: {
            show() {
                loading.show();
            },
            hide() {
                loading.hide();
            }
        }
    };

</script>

<style lang="scss">
    @import '../scss/_common';
    .demo-loading {
        background: $white;
    }

    .demo-loading ul {
        padding: 10px;
    }

    .demo-loading li {
        margin-top: 10px;
    }
</style>