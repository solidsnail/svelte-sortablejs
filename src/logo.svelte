<script>

</script>

<style>
  #logo {
    display: flex;
    flex-flow: column;
    align-items: center;
    align-self: center;
    justify-content: center;
    height: 300px;
  }
  h1 {
    text-align: center;
    font-weight: 100;
    font-size: 40px;
    color: grey;
  }
  .segment {
    text-align: center;
    padding: 5px 10px;
    font-size: 35px;
    font-weight: 100;
    color: white;
    letter-spacing: 10px;
    user-select: none;
  }
  .segment:nth-of-type(1) {
    background: #ff3e00;
    transform: perspective(70px) rotateY(-5deg);
    top: 3px;
    z-index: 3;
    position: relative;
  }
  .segment:nth-of-type(2) {
    background: #d33906;
    transform: perspective(70px) rotateY(16deg);
    z-index: 2;
  }
  .segment:nth-of-type(2)::before {
    background: rgba(0, 0, 0, 0.1);
    content: "";
    position: absolute;
    top: -40px;
    left: 11px;
    width: 94px;
    height: 47px;
  }
  .segment:nth-of-type(3) {
    background: #b63409;
    z-index: 1;
    transform: perspective(70px) rotateY(-15deg);
    position: relative;
    top: -2px;
  }
</style>

<div id="logo">
  <div class="segment">SOR</div>
  <div class="segment">TAB</div>
  <div class="segment">LE</div>
  <h1>The sorting library for svelte</h1>
</div>
