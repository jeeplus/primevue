<template>
    <div>
        <div class="content-section introduction">
            <div class="feature-intro">
                <h1>ProgressSpinner</h1>
                <p>ProgressSpinner is a process status indicator.</p>
            </div>
        </div>

        <div class="content-section implementation">
            <h3 class="first">Basic</h3>
            <ProgressSpinner />

            <h3>Custom</h3>
            <ProgressSpinner style="width:50px;height:50px" strokeWidth="8" fill="#EEEEEE" animationDuration=".5s"/>
        </div>

        <ProgressSpinnerDoc />
    </div>
</template>

<script>
import ProgressSpinnerDoc from './ProgressSpinnerDoc';

export default {
    components: {
        'ProgressSpinnerDoc': ProgressSpinnerDoc
    }
}
</script>