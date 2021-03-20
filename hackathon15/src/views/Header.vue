<template>
  <header>
      <div class="contenedor Header">
            <a class="Header-Logo-Texto-Link" href="#">
                <img class="Header-Logo-Texto-Link-Logo" src="../assets/aits-logo.png"> 
                <div>
                    <span class="Header-Logo-Texto-Link__Texto1">Alva</span> <span class="Header-Logo-Texto-Link__Texto2">IT Solutions</span> 
                </div>
            </a>
            <div class="Header-Menu">
                <ul class="Header-ListItem">
                    <li class="Header-Item"><a class="Header-Link Header-Selected" href="#">Inicio</a></li>
                    
                </ul>
            </div>
        </div>
        <section class="Header-About">
            <h1 class="About texto-centro">HACKATHON 14</h1>
        </section>  
  </header>
</template>

<script>
export default {

}
</script>

<style>
    .Header {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
    background: white;
    padding: 10px 0px;
    }

    .Header-Logo-Texto-Link {
  text-decoration: none;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}

.Header-Logo-Texto-Link-Logo {
  padding-right: 10px;
}

.Header-Logo-Texto-Link__Texto1 {
  font-family: 'Georgia Pro Black', Georgia, serif;
  font-size: 1.8em;
  font-weight: 600;
  color: #233985;
}

.Header-Logo-Texto-Link__Texto2 {
  font-family: 'Verdana Pro Black', Verdana, Tahoma;
  font-size: 1.1em;
  font-weight: 800;
  color: #4BBDE0;
}

.Header-Menu {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.Header-ListItem {
  padding: 0;
  margin: 0;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}

.Header-Item {
  padding: .5em;
  list-style-type: none;
}

.Header-Link {
  text-decoration: none;
  font-size: 1.1em;
  color: black;
}

.Header-Selected {
  font-weight: bold;
  color: #28476E;
}

.Header-About {
  background: #233985;
}

.About {
  padding: 3rem 0 3rem 0;
  margin: 0 auto;
  text-align: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  color: #fff;
}
</style>