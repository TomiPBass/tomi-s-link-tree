<template>
    <div class="form_container">
        <form action="">
        <div class="form_left">
            <label for="submit_question">Submit your question:</label>
            <input type="text" name="question" id="question" />
            <p>Example: "What's your vocal range?"</p>
        </div>

        <div class="form_right">
            <input type="button" value="Submit Question" />
        </div>
        </form>
    </div>
</template>

<script setup>
</script>

<style>
.form_container{
    background-color: white;
    margin: 2em -1em 0 -1em;
    padding: 2em;
}

label{
    color: #151515;
    font-weight: bold;
    display: block;
    margin-bottom: 1em;
    font-size: 1.2em;
}

input[type=text]{
    border: 1px solid black;
    width: 100%;
    padding: 1em;
    box-sizing: border-box;
    border-radius: 1em;
    margin-top: 1.2em;
}

.form_container p{
    color: gray;
    margin-bottom: 1.5em;
    font-weight: normal;
    font-size: .8em;
    margin-top: .5em;
}

input[type=button] {
    background-color: black;
    border: none;
    width: 100%;
    color: white;
    font-weight: bold;
    padding: .5em 0;
    border-radius: .5em;
    font-size: 1.5em;
    margin-top: 0em;
}

input[type=button]:hover{
    background-color: rgb(59, 59, 59);
    font-size: 1.4em;   
    margin-bottom: .15em;
}

@media (min-width: 667px) {
.form_container{
    border-radius: 3em;
}
}


</style>