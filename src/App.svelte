<script>
  import Navbar from './lib/Navbar.svelte'
  import 'animate.css';


function topScroll() {
  window.scrollTo({
    top: 0,
    left: 0,
    behavior: 'smooth'
  });
}

</script>

<main>
  <Navbar />
  <div class="h1container">
  <h1 class=" animate__animated animate__bounceInLeft">HOLY GRAIL</h1>
</div>
  <div class="imgcontainer">
  <img on:click={topScroll} src="https://www.freeiconspng.com/thumbs/trophy-png/trophy-png-23.png" class="trophy animate__animated animate__bounceInUp" alt="trophy">
</div>
</main>
  <style>

@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@100;400&display=swap');


.imgcontainer {
  display: flex;
  justify-content: center;
  transform: translateY(-430px);
}

    .trophy {
      transform: rotate(-20deg);
      z-index: 2;
      height: 30rem;
    }

    h1 {
      transform: translateY(500%);
      font-size: 32rem;
      font-family: 'Bebas Neue', cursive;
      text-align: center;
      justify-content: center;
    }

    .h1container {
    display:flex;
    align-items: center;
    justify-content: center;
}

.trophy:hover {
  scale: 1.1;
  transition: 200ms;
  cursor: pointer;
}

  </style>