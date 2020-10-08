<template>
  <main>

    <nav class="navbar navbar-expand-lg navbar-dark bg-info">
      <a class="navbar-brand" href="/">GOV.PK</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbar">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item"><router-link class="nav-link" :to="{ name: 'home' }">Home</router-link></li>
          <li class="nav-item"><router-link class="nav-link" :to="{ name: 'about' }">About</router-link></li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" name="q" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-light my-2 my-sm-0" type="submit">Go</button>
        </form>
      </div>
    </nav>
    
    <nav>
      <ol class="breadcrumb rounded-0">
        <li class="breadcrumb-item"><a href="#">Home</a></li>
        <li class="breadcrumb-item"><a href="#">Library</a></li>
        <li class="breadcrumb-item active" aria-current="page">Data</li>
      </ol>
    </nav>

    <section class="container-fluid">
      <router-view />
    </section>
    <footer class="py-3 bg-light">
      <ul class="nav">
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'help' }">Help</router-link></li>
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'terms' }">Terms</router-link></li>
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'privacy' }">Privacy</router-link></li>
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'cookies' }">Cookies</router-link></li>
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'accessibility' }">Accessibility</router-link></li>
        <li class="nav-item"><router-link class="nav-link" :to="{ name: 'contact' }">Contact</router-link></li>
      </ul>
    </footer>
  </main>
</template>

<style>
  html, body { height: 100%; }
</style>