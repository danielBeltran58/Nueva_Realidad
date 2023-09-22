<script setup>
    import { 
        genderRadioOptions,
        visitCompanion,
        ageRange,
        actualState,
        schoolLevel,
        responsibleAdults,
        responsibleAdultsIsRules,
        parentsRelationship,
        studiesImportance,
        wellPaidJob,
        noStudyDrugUsers,
        meaningOfAddiction,
        preventAddictions,
        acquaintancesDrugs,
        freeDrugs,
        alcoholCup,
        tobacco,
        dope,
        cocaine,
        methamphetamines,
        substanceStarted,
        tobaccoStarted,
        substanceCrime,
        useDrugs,
        teenHealthUseDrugs
    } from '../FormularioEntrada/formularioEntrada';
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
            <h3 class="col-12 text-center mt-4">Formulario de entrada</h3>
        </div>
    </div>
    <!--Secciones-->
    <div class="container">
        <!--Seccion 1 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 1 de 8</legend>
            <div>
                <label for="encuentaEntrada">Encuesta de entrada</label>
                <input class="form-control" type="text" name="encuentaEntrada" id="">
            </div>
            <div>
                <label for="codigoGrupo">El código de mi grupo es:</label>
                <input class="form-control" type="text" name="codigoGrupo" id="">
            </div>
        </fieldset>
         <!--Seccion 2 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 2 de 8</legend>
            <RadioButton 
            :title="'1. ¿Soy?'"
            :nameChecked="'genderOptions'"
            :radioOptions="genderRadioOptions"
            />
            <RadioButton 
            :title="'2. ¿Quién te acompaña en tu visita?'"
            :nameChecked="'visitCompanionOptions'"
            :radioOptions="visitCompanion"
            />
            <RadioButton 
            :title="'3. Selecciona tu rango de edad:'"
            :nameChecked="'ageRangeOptions'"
            :radioOptions="ageRange"
            />
            <RadioButton 
            :title="'4. Actualmente:'"
            :nameChecked="'actualStateOptions'"
            :radioOptions="actualState"
            />
            <RadioButton 
            :title="'5. Tu nivel escolar es:'"
            :nameChecked="'schoolLevelOptions'"
            :radioOptions="schoolLevel"
            />
        </fieldset>
        <!--Seccion 3 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 3 de 8</legend>
            <RadioButton 
            :title="'6. Marca la opción que describa quiénes son los adultos responsables de ti:'"
            :nameChecked="'responsibleAdultsOptions'"
            :radioOptions="responsibleAdults"
            />
            <RadioButton 
            :title="'7. Los adultos responsables de ti: ¿Te han puesto reglas claras sobre el consumo del alcohol, tabaco u otras drogas?'"
            :nameChecked="'responsibleAdultsIsRulesOptions'"
            :radioOptions="responsibleAdultsIsRules"
            />
            <RadioButton 
            :title="'8. ¿Cómo describes la relación con tus padres?'"
            :nameChecked="'parentsRelationshipOptions'"
            :radioOptions="parentsRelationship"
            />
            <RadioButton 
            :title="'9. ¿Qué tan importante es terminar tus estudios hasta el grado universitario?'"
            :nameChecked="'studiesImportanceOptions'"
            :radioOptions="studiesImportance"
            />
            <RadioButton 
            :title="'10. ¿Cuál es la posibilidad de que tengas un trabajo bien remunerado?'"
            :nameChecked="'wellPaidJobOptions'"
            :radioOptions="wellPaidJob"
            />
        </fieldset>
        <!--Seccion 4 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 4 de 8</legend>
            <RadioButton 
            :title="'11. Las personas de tu edad que abandonan la escuela. ¿Qué tan probable es que lleguen a consumir drogas?'"
            :nameChecked="'noStudyDrugUsersOptions'"
            :radioOptions="noStudyDrugUsers"
            />
            <RadioButton 
            :title="'12. Adicción significa:'"
            :nameChecked="'meaningOfAddictionOptions'"
            :radioOptions="meaningOfAddiction"
            />
            <RadioButton 
            :title="'13. De los siguientes ejemplos ¿Cuáles son las acciones que puedes realizar para alejarte de las adicciones?'"
            :nameChecked="'preventAddictionsOptions'"
            :radioOptions="preventAddictions"
            />
            <RadioButton 
            :title="'14. ¿Conoces a alguien que use drogas?'"
            :nameChecked="'acquaintancesDrugsOptions'"
            :radioOptions="acquaintancesDrugs"
            />
            <RadioButton 
            :title="'15. Alguna vez, ¿Te han ofrecido droga gratis?'"
            :nameChecked="'freeDrugsOptions'"
            :radioOptions="freeDrugs"
            />
        </fieldset>
        <!--Seccion 5 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 5 de 8</legend>
            <RadioButton 
            :title="'16. ¿Has tomado una copa completa de alguna bebida con alcohol, como cerveza, tequila, ron, whisky o vodka?'"
            :nameChecked="'alcoholCupOptions'"
            :radioOptions="alcoholCup"
            />
            <RadioButton 
            :title="'17. ¿Has fumado o probado tabaco?'"
            :nameChecked="'tobaccoOptions'"
            :radioOptions="tobacco"
            />
            <RadioButton 
            :title="'18. Alguna vez en tu vida ¿has tomado usado o probado marihuana?'"
            :nameChecked="'dopeOptions'"
            :radioOptions="dope"
            />
            <RadioButton 
            :title="'19. Alguna vez en tu vida ¿has tomado usado o probado cocaína?'"
            :nameChecked="'cocaineOptions'"
            :radioOptions="cocaine"
            />
            <RadioButton 
            :title="'20. Alguna vez en tu vida ¿has tomado usado o probado mentafetaminas (cristal, foco, tachas)?'"
            :nameChecked="'methamphetaminesOptions'"
            :radioOptions="methamphetamines"
            />
        </fieldset>
        <!--Seccion 6 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 6 de 8</legend>
            <RadioButton 
            :title="'16. ¿Has tomado una copa completa de alguna bebida con alcohol, como cerveza, tequila, ron, whisky o vodka?'"
            :nameChecked="'alcoholCupOptions'"
            :radioOptions="alcoholCup"
            />
            <RadioButton 
            :title="'17. ¿Has fumado o probado tabaco?'"
            :nameChecked="'tobaccoOptions'"
            :radioOptions="tobacco"
            />
            <RadioButton 
            :title="'18. Alguna vez en tu vida ¿has tomado usado o probado marihuana?'"
            :nameChecked="'dopeOptions'"
            :radioOptions="dope"
            />
            <RadioButton 
            :title="'19. Alguna vez en tu vida ¿has tomado usado o probado cocaína?'"
            :nameChecked="'cocaineOptions'"
            :radioOptions="cocaine"
            />
            <RadioButton 
            :title="'20. Alguna vez en tu vida ¿has tomado usado o probado mentafetaminas (cristal, foco, tachas)?'"
            :nameChecked="'methamphetaminesOptions'"
            :radioOptions="methamphetamines"
            />
        </fieldset>
        <!--Seccion 7 de 8-->
        <fieldset class="border p-2">
            <legend class="fs-5 float-none w-auto p-2">Sección 7 de 8</legend>
            <RadioButton 
            :title="'21. Si contestaste Sí en alguna de las preguntas anteriores ¿Cuál fue la sustancia con la que iniciaste?'"
            :nameChecked="'alcoholCupOptions'"
            :radioOptions="alcoholCup"
            />
            <RadioButton 
            :title="'17. ¿Has fumado o probado tabaco?'"
            :nameChecked="'tobaccoOptions'"
            :radioOptions="tobacco"
            />
            <RadioButton 
            :title="'18. Alguna vez en tu vida ¿has tomado usado o probado marihuana?'"
            :nameChecked="'dopeOptions'"
            :radioOptions="dope"
            />
            <RadioButton 
            :title="'19. Alguna vez en tu vida ¿has tomado usado o probado cocaína?'"
            :nameChecked="'cocaineOptions'"
            :radioOptions="cocaine"
            />
            <RadioButton 
            :title="'20. Alguna vez en tu vida ¿has tomado usado o probado mentafetaminas (cristal, foco, tachas)?'"
            :nameChecked="'methamphetaminesOptions'"
            :radioOptions="methamphetamines"
            />
        </fieldset>
    </div>
</template>