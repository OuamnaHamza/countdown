<template>
  <footer>
    <h4>
      Made with ♡ by
      <a href="https://tmo.codes" target="”_blank”">Tyler Morales</a>
    </h4>

    <div id="bmc-button">
      <a
        class="bmc-button"
        target="_blank"
        href="https://www.buymeacoffee.com/tmorales"
        ><img
          src="https://cdn.buymeacoffee.com/buttons/bmc-new-btn-logo.svg"
          alt="Buy me a coffee"
        /><span style="margin-left:5px;font-size:18px !important;"
          >Buy me a coffee</span
        ></a
      >
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
footer {
  margin: 50px 0;
}
h4 {
  text-align: center;
  padding: 20px;
  font-weight: 400;

  a {
    display: inline-block;
    position: relative;

    &:after {
      background: none repeat scroll 0 0 transparent;
      bottom: 0;
      content: '';
      display: block;
      height: 2px;
      left: 50%; // expand from middle
      position: absolute;
      background: var(--color-primary);
      transition: width 0.3s ease 0s, left 0.3s ease 0s;
      width: 0;
    }

    &:hover:after {
      width: 100%;
      left: 0;
    }
  }
}
#bmc-button {
  text-align: center;
}

.bmc-button img {
  height: 34px !important;
  width: 35px !important;
  margin-bottom: 1px !important;
  box-shadow: none !important;
  border: none !important;
  vertical-align: middle !important;
}

.bmc-button {
  padding: 7px 15px 7px 10px !important;
  line-height: 35px !important;
  height: 51px !important;
  text-decoration: none !important;
  display: inline-flex !important;
  color: #ffffff !important;
  background-color: #bd5fff !important;
  border-radius: 8px !important;
  border: 1px solid transparent !important;
  font-size: 18px !important;
  letter-spacing: -0.08px !important;
  box-shadow: 0px 1px 2px rgba(190, 190, 190, 0.5) !important;
  -webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
  margin: 0 auto !important;
  font-family: 'Lato', sans-serif !important;
  -webkit-box-sizing: border-box !important;
  box-sizing: border-box !important;
}

.bmc-button:hover,
.bmc-button:active,
.bmc-button:focus {
  -webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
  text-decoration: none !important;
  box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
  opacity: 0.85 !important;
  color: #ffffff !important;
}
</style>
