<script setup>
    import {
        miaMeaning,
        miaLearned,
        miaExperience,
        liveExperience,
        mostLikeModule,
        unlikeModule,
        addictionMeaning,
        drugsMeaning,
        alcoholHealthAdolescents,
        alcoholDriving
    } from '../FormularioSalida/formularioSalida.js';
    import RadioButton from '../../components/radioButton/RadioButton.vue';
</script>

<template>
    <div class="container">
        <div class="row">
            <img 
            class="col-12 w-50 h-50 d-block my-0 mx-auto"
            src="/src/assets/MIA.webp" 
            alt="MIA"
            >
            <h3 class="col-12 text-center mt-4">Formulario de salida</h3>
        </div>
    </div>
    <div class="container">
        <!--Sección 1 de 5-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 1 de 5</legend>
            <div>
                <label for="encuentaSalida">Encuesta de salida</label>
                <input class="form-control" type="text" name="encuentaSalida" id="">
            </div>
            <div>
                <label for="codigoGrupo">El código de mi grupo es:</label>
                <input class="form-control" type="text" name="codigoGrupo" id="">
            </div>
        </fieldset>
        <!--Sección 2 de 5-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 2 de 5</legend>
            <RadioButton 
            :title="'1. Para ti, MIA significa:'"
            :nameChecked="'miaMeaningOptions'"
            :radioOptions="miaMeaning"
            />
            <RadioButton 
            :title="'2. Lo que aprendiste en MIA te parece:'"
            :nameChecked="'miaLearnedOptions'"
            :radioOptions="miaLearned"
            />
            <RadioButton 
            :title="'3. ¿Qué aprendiste durante la experiencia MIA?'"
            :nameChecked="'miaExperienceOptions'"
            :radioOptions="miaExperience"
            />
            <RadioButton 
            :title="'4. ¿A quién invitarías a vivir la experiencia?'"
            :nameChecked="'liveExperienceOptions'"
            :radioOptions="liveExperience"
            />
            <RadioButton 
            :title="'5. ¿Cuál fue el módulo que más te gustó?'"
            :nameChecked="'mostLikeModuleOptions'"
            :radioOptions="mostLikeModule"
            />
        </fieldset>
        <!--Sección 3 de 5-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 2 de 5</legend>
            <RadioButton 
            :title="'6. ¿Cuál fue el módulo que menos te gustó?'"
            :nameChecked="'unlikeModuleOptions'"
            :radioOptions="unlikeModule"
            />
            <RadioButton 
            :title="'7. ¿Adicción significa?'"
            :nameChecked="'addictionMeaningOptions'"
            :radioOptions="addictionMeaning"
            />
            <RadioButton 
            :title="'8. El usar drogas es:'"
            :nameChecked="'drugsMeaningOptions'"
            :radioOptions="drugsMeaning"
            />
            <RadioButton 
            :title="'9. ¿Un adolescente puede dañar su desarrollo y salud por consumir alcohol?'"
            :nameChecked="'alcoholHealthAdolescentsOptions'"
            :radioOptions="alcoholHealthAdolescents"
            />
            <RadioButton 
            :title="'10. ¿Te subirías a un automóvil con alguien que recién haya consumido 3 cervezas o 3 copas de bebidas con alcohol y vaya a manejar, o conducirías tú después de haber tomado alcohol?'"
            :nameChecked="'alcoholDrivingOptions'"
            :radioOptions="alcoholDriving"
            />
        </fieldset>
    </div>
</template>