<template>
  <div>
    <!-- header -->
    <header>
      <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container">
          <a class="navbar-brand" href="#">Logo</a>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarNavDropdown"
            aria-controls="navbarNavDropdown"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav ms-auto">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#" @click.prevent="$router.push({name:'home'})">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#" @click.prevent="$router.push({name:'donate'})">Donate</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#" @click.prevent="$router.push({name:'team'})">Our Team</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Donors</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Our Team</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Blogs</a>
              </li>
              <!-- <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown link
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li> -->
            </ul>
          </div>
        </div>
      </nav>
    </header>
    <!-- Main -->
    <slot></slot>
    <!-- Footer -->
    <footer class="bg-dark text-white py-5">
       <div class="container">
          <div class="row">
            <div class="col-md-4">
              <h5>About us</h5>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas optio facere eaque voluptatibus quae, libero quibusdam est maiores blanditiis, hic minima illo laborum harum dolore similique nisi? Saepe, illum esse.</p>
            </div>

            <div class="col-md-4">
              <h5>Quick Links</h5>
              <ul>
                <li>Home</li>
                <li>About</li>
                <li>Team</li>
              </ul>
            </div>

            <div class="col-md-4">
              <h5>We accept</h5>
              <ul>
                <li>Bank Transfer</li>
                <li>eSewa</li>
                <li>Khalti</li>
              </ul>
            </div>
          </div>
       </div>
    </footer>
  </div>
</template>

<script>
export default {
    name:'TemplateView',
}
</script>
