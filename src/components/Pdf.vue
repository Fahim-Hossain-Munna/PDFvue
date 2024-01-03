<template>
    <div id='convertToPdf'>
        <h1>Hi,</h1>
        <h2>I'm Fahim Hossain Munna</h2>
        <h3>Asst. Faculty Member</h3>
        <h4>Web & Software Department</h4>
        <h5>Creative IT Institute</h5>
        <button @click="exportPdf()">Export PDF</button>
    </div>
</template>


<script setup>
import html2pdf from 'html2pdf.js'

function exportPdf(){
    let element = document.getElementById('convertToPdf')

    html2pdf(element),{
        margin : 1,
        filename: 'info.pdf'
    }
}

</script>

<style scoped>
#convertToPdf{
    text-align: center;
}
#convertToPdf button{

    background: #000;
    color: #fff;
}
</style>