<template>
  <div class="nav">
    <div class="left-side-nav">
      <button class="menu-button">
        <div><svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24" focusable="false"><path d="M21 6H3V5h18v1zm0 5H3v1h18v-1zm0 6H3v1h18v-1z"/></svg></div>
      </button>
    </div>
    <div class="center-bar-nav">
      <input class="input-search" placeholder="Search">
      <button class="search-button">
        <div><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" height="24" viewBox="0 0 24 24" width="24" focusable="false"><path clip-rule="evenodd" d="M16.296 16.996a8 8 0 11.707-.708l3.909 3.91-.707.707-3.909-3.909ZM18 11a7 7 0 11-14 0 7 7 0 0114 0Z" fill-rule="evenodd"/></svg></div>
      </button>
    </div>
    <div class="right-side-nav">
      <p class="p-menu">Menu</p>
      <p class="p-menu">Menu</p>
      <p class="p-menu">Menu</p>
    </div>
  </div>
  <div class="footer">
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque architecto praesentium quidem ipsa aspernatur ipsam assumenda eligendi? Rem maxime voluptatibus numquam inventore quisquam temporibus nesciunt, ipsa, architecto magni culpa ullam in qui repellat magnam a! Explicabo unde ipsa incidunt delectus fugiat earum tempore laudantium quasi, quae cupiditate velit voluptatum, iusto provident a asperiores, ipsum recusandae obcaecati minus! Dolorem amet, est vitae in ab perferendis tempore maxime aut quis excepturi molestiae esse libero repellendus voluptatibus. Non ducimus dicta provident magnam id ad hic quis laborum? Exercitationem ex quidem animi distinctio minima. Repellat quibusdam laudantium alias nulla quia quam dolores itaque! Assumenda.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati, voluptatibus consequatur. Recusandae delectus autem beatae sequi deserunt labore? Voluptates necessitatibus illo ex! Blanditiis similique vel temporibus beatae voluptas. Deleniti obcaecati nulla quaerat nihil sequi alias, qui vero eos. Vitae eligendi quam repellat libero quo commodi ex dolor tempora fuga praesentium!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur nisi excepturi quo voluptatem, ab voluptatum omnis corrupti cum corporis. Asperiores debitis in ea numquam, maiores laborum, quae quia, totam dolorum nostrum velit? Autem, veritatis! Temporibus quis assumenda, nisi fuga pariatur natus itaque ducimus ipsum in illo reprehenderit nostrum tempora, consequuntur labore commodi esse obcaecati eaque quo porro quidem provident asperiores officiis. Facilis numquam culpa ullam facere, perferendis nulla debitis aperiam, quod accusantium id deserunt. Delectus, amet cumque porro voluptatum iusto veniam ullam. Consequuntur maxime beatae tempora similique ut fuga, praesentium numquam cum repudiandae impedit, vel incidunt neque, doloremque ad deleniti.</p>
  </div>

</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

.nav {
  display: flex;
  flex-direction: row;
  background-color: black;
  color: gray;
  justify-content: space-between;
  width: 100%;
}

.left-side-nav {
  display: flex;
  align-items: center;
  padding: 10px;
}

.menu-button {
  width: 40px;
  height: 40px;
  background-color: transparent;
  border: none;
  cursor: pointer;
  border-radius: 20px;
  transition: 0.5s;
  display: flex;
  justify-content: center;
  align-items: center;
}

.menu-button:hover {
  background-color: rgb(48,48,48);
}

.center-bar-nav {
  display: flex;
  align-items: center;
  padding: 10px;
}

.input-search {
  flex: 1;
  width: 300px;
  height: 40px;
  color: white;
  border-radius: 2px;
  border: 1px solid rgb(48,48,48);
  outline: none;
  padding-left: 10px;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  background-color: transparent;
  min-width: 40px;
}

.search-button {
  height: 40px;
  width: 40px;
  background-color: transparent;
  color: white;
  border: 1px solid rgb(48,48,48);
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  transition: 0.5s;
}

.search-button:hover {
  background-color: rgb(48,48,48);
}

.right-side-nav {
  display: flex;
  align-items: center;
  margin-right: 10px;
}

.p-menu {
  margin: 10px;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 3px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.5s;
}

.p-menu:hover {
  color: rgb(200,0,0);
}

.footer {
  margin-top: 500px;
  background-color: black;
  color: gray;
  padding: 30px;
  letter-spacing: 3px;
  text-transform: uppercase;
  display: flex;
  flex-direction: row;
  text-align: center;
  width: 100%;
  font-size: 8px;  
  flex:1;
}
.side-bar {
  position: fixed;
  top:0;
  right: 0;
  height: 200px;
  width: 100px;
  z-index: 999;
  background-color: black;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
}


@media (max-width: 600px) {
  .nav {
    flex-direction: row;
  }
  
  .center-bar-nav {
    flex: 1;
  }
  
  .right-side-nav {
    margin-top: 10px;
    margin-right: 0;
    align-items: center;
    justify-content: center;
  }
  .input-search {
    width: 10%;
  }
  .search-button {
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
  
  }
  .left-side-nav {
    display: none;
  }
  .search-button {
    display: none;
  }
  
}
</style>


<script setup>



</script>