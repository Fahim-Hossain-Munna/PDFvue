# Html To PDF Convert using vue.js 3

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/)

### Step 1: Start Application server Vue 3

```
npm install
npm run dev
```
### Step 2: How To Install html2pdf

```
npm i html2pdf.js@0.9.0
```
### Step 3: How To import html2pdf

```
import html2pdf from 'html2pdf.js'
```

### Step 4 : Main Html To PDF code

```
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
```

