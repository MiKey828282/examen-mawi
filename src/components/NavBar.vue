<template>
    <div class="container-fluid" id="nav">
      <div class="row">
        <div class="col" style="text-align: start">
          <a href="#" ><span>SHOP</span></a>
          <a href="#" ><span>ABOUT US</span></a>
          <a href="#" ><span>GLASS SKIN DUO</span></a>
        </div>
        <div class="col">
          <img class="logo"
            src="https://i0.wp.com/beautyfeed.org/wp-content/uploads/2024/08/0-02-05-49d2ac187d2d7f767ae6122638d9714c0d32759cc6b44e9bcd74fe742e3619ab_f9b359a9a4080609.png?fit=1553%2C685&ssl=1"
            alt="logo"
          />
        </div>
        <div class="col" style="text-align: end">
          <a href="#" ><span>CART</span></a>
          <a href="#" ><span>SEARCH</span></a>
        </div>
      </div>
    </div>
  </template>

<style scoped>
#nav {
  top: 0%;
  width: 100vw;
  padding: 30px;
  box-sizing: border-box;
  text-align: center;
  margin-bottom: 20px;
  position: fixed;
}

.logo {
  text-align: center;
  justify-content: center; 
  margin: 0 auto;
  width: 170px;
  max-height: 200px;
  overflow: hidden;
}

a{ 
  font-size: 18px;
  padding: 6px 20px;
  margin: 5px;
  position: relative;
  display: inline-block;
  border: 2px solid #1e1e1e;;
  text-transform: uppercase;
  text-decoration: none;
  color: #1e1e1e;
  font-weight: 600;
  z-index: 3;
}

a::before {
  content: '';
  position: absolute;
  top: 6px;
  left: -2px;
  width: calc(100% + 4px);
  height: calc(100% - 12px);
  background-color: #ffffff;
  
  transition: 0.2s ease-in-out;
  transform: scaleY(1);
}

a:hover::before {
  transform: scaleY(0);
}

a::after {
  content: '';
  position: absolute;
  left: 6px;
  top: -2px;
  height: calc(100% + 4px);
  width: calc(100% - 12px);
  background-color: #ffffff;
  
  transition: 0.2s ease-in-out;
  transform: scaleX(1);
  transition-delay: 0.2s;
}

a:hover::after {
  transform: scaleX(0);
}

a span {
  position: relative;
  z-index: 3;
}

.row {
  display: flex;
  margin-bottom: 10px;
}

.col {
  flex: 1;
  padding: 20px;
  margin-right: 10px;
  text-align: center;
}

.col:last-child {
  margin-right: 0;
}

</style>
