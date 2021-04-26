<template>
    <header>
        <h2>Henlo me is shymi and this is my portfolio</h2>
    </header>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@keyframes typing {
  from { width: 0; white-space: nowrap; }
  to { width: 100%; white-space: normal; }
}

@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: #01A0E2; }
}

header {
    width: 100%;
    height: 30vh;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 1px solid #01A0E2;
    h2 {
        width: 80%;
        color: #222;
        font-family: 'Montserrat', sans-serif;
        overflow: hidden;
        border-right: 2px solid #01A0E2;
        //white-space: nowrap;
        margin: 0 auto;
        letter-spacing: .125em;
        animation: 
            typing 3.5s steps(32, end),
            blink-caret .75s step-end infinite;
    }
}

@media screen and (min-width: 1400px){
  @keyframes typing {
    from { width: 0 }
    to { width: 50% }
  }

  @keyframes blink-caret {
    from, to { border-color: transparent }
    50% { border-color: #01A0E2; }
  }

  header {
      width: 100%;
      height: 30vh;
      display: flex;
      align-items: center;
      justify-content: center;
      border-bottom: 1px solid #01A0E2;
      h2 {
          max-width: 630px;
          color: #222;
          font-family: 'Montserrat', sans-serif;
          overflow: hidden;
          border-right: 2px solid #01A0E2;
          white-space: nowrap;
          margin: 0 auto;
          letter-spacing: .125em;
          animation: 
              typing 3.5s steps(32, end),
              blink-caret .75s step-end infinite;
      }
  }
}
</style>