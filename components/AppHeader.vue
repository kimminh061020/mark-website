<template>
<div class="header">
<div class="nav-wrap">
  <b-navbar>
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <div class="logo-name">MARK NGUYEN</div>
            </b-navbar-item>
        </template>
        <template #end>
            <b-navbar-item tag="div">
                <a href = "mailto: kimminh061020@gmail.com">
                <div class="buttons rounded">
                    <b-button hovered rounded type="is-light">Contact me</b-button>
                </div>
                </a>
            </b-navbar-item>
        </template>
    </b-navbar>
    </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.navbar-item img {
    max-height: 5rem;
}

.nav-wrap {
    width: 85%;
background: black;
}

.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    background: black;
}
.navbar {
    background: black;
}

.navbar-item {
    color: white;
    padding: 10%
}

.navbar-link {
    color: white;
}
.navbar-dropdown {
    background: black;
}

.logo-name {
    font-size: 30px;
    font-weight: 500;
}

.button.is-light:hover, .button.is-light.is-hovered {
    background-color: #ffffff;
    border-color: transparent;
    color: rgb(0, 0, 0);
    font-weight: 500;
}
</style>