<template>
    <div>
        <div class="content-section introduction">
            <div class="feature-intro">
                <h1>ToggleButton</h1>
                <p>ToggleButton is used to select a boolean value using a button.</p>
            </div>
        </div>

        <div class="content-section implementation">
            <h3 class="first">Basic</h3>
            <ToggleButton v-model="checked1" onIcon="pi pi-check" offIcon="pi pi-times" />
            <p>{{checked1}}</p>

            <h3>Customized</h3>
            <ToggleButton v-model="checked2" onLabel="I confirm" offLabel="I reject" onIcon="pi pi-check" offIcon="pi pi-times" style="width: 10em" />
            <p>{{checked2}}</p>
        </div>

        <ToggleButtonDoc/>
    </div>
</template>

<script>
import ToggleButtonDoc from './ToggleButtonDoc';

export default {
    data() {
        return {
            checked1: false,
            checked2: true
        }
    },
    components: {
        'ToggleButtonDoc': ToggleButtonDoc
    }
}
</script>