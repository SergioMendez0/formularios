<template>
    <h3 class="text-cenTer">Progreso {{porcentaje}} %</h3>
      
    <div class="progress">
        <div class="progress-bar progress-bar-striped progress-bar-animated
         bg-success" role="progressbar" 
         aria-valuenow="porcentaje"
        aria-valuein="0"
         aria-valuemax="100"
         :style="`width: ${porcentaje}%`">***
        </div>
      </div>
</template>

<script>
    export default {
        props: {
            porcentaje: Number,

        }
    }
</script>