<template>
    <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-success py-3">
        <div class="container">
            <router-link :to="{ name: 'home' }" class="navbar-brand" aria-current="page"> <img
                    src="../../public/img/unidaicon.png" class="img justify-content-center" alt="" />
                Al-Qur'an online
            </router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse"
                aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarCollapse">
                <ul class="navbar-nav me-auto mb-2 mb-md-0">
                    <li class="nav-item">
                        <router-link :to="{ name: 'home' }" class="nav-link text-bold">Beranda</router-link>
                    </li>
                    
                    <li class="nav-item">
                        <router-link :to="{ name: 'website' }" class="nav-link text-bold">Website</router-link>
                    </li>
                    
                    <li class="nav-item">
                        <router-link :to="{ name: 'pmb' }" class="nav-link text-bold">Daftar jadi Mahasiswa</router-link>
                    </li>
                    <!-- dropdown -->
                    <!-- <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                            data-bs-toggle="dropdown" aria-expanded="false">
                            KATEGORI
                        </a>
                        <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDropdown">
                            <li>
                                <router-link :to="{ name: 'home' }" class="dropdown-item">SURAH</router-link>
                            </li>
                            <li>
                                <router-link :to="{ name: 'juz' }" class="dropdown-item">JUZ</router-link>
                            </li>
                        </ul>
                    </li> -->
                </ul>
            </div>
        </div>
    </nav>
</template>

<style scoped>
.navbar-brand {
    font-weight: bold;
}

img {
    width: 35px;
    height: 35px;
}

@media only screen and (max-width: 768px) {
    .navbar {
        text-align: center;
    }

    .btn-custom {
        width: 100%;
    }
}
</style>

<script>
export default {
    name: 'NavbarVue',
}
</script>