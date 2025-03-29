<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PORTFOLIO</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <style>
    body {
        font-family: 'Arial', sans-serif;
        background-color: #FAF3E0; /* Beige pastel */
        color: #5D5D5D;
        margin: 0;
    }
    
    .navbar {
        background-color: #FFD1DC; /* Rosa pastel */
    }
    
    .navbar-brand, .nav-link {
        color: #5D5D5D !important;
        font-weight: bold;
    }
    
    .hero {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 50vh; /* Cambiado de 70vh a 50vh para hacerla más delgada */
    text-align: center;
    background-color: #FFEBB7; /* Amarillo pastel */
   }

    
    .hero img {
        max-width: 50%;
        border-radius: 10px;
    }
    
    .hero-text {
        max-width: 40%;
        padding: 20px;
    }
    
    .portfolio {
        padding: 50px 20px;
    }
    
    .item {
        background-color: #FFD1DC; /* Rosa pastel */
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0 2px 5px rgba(255, 255, 255, 0.1);
        text-align: center;
        transition: transform 0.3s ease-in-out;
        margin-bottom: 20px;
    }
    
    .item:hover {
        transform: scale(1.05);
    }
    
    .item img {
        width: 100%;
        height: 200px; /* Tamaño fijo para las imágenes */
        object-fit: cover; /* Asegura que la imagen cubra el espacio sin distorsionarse */
        cursor: pointer; /* Cambia el cursor a pointer para indicar que es clickeable */
    }
    
    .item h3 {
        margin: 0;
        padding: 10px 0 5px;
    }
    
    .item p {
        margin: 0;
        padding-bottom: 10px;
        color: #777;
    }
    
    .centered-item {
        margin: 0 auto;
        float: none;
    }
    
    .centered-row {
        display: flex;
        justify-content: center;
        gap: 20px;
        flex-wrap: wrap;
        margin-bottom: 20px;
    }
    
    .centered-row .item {
        width: 300px;
        flex: 0 0 auto;
    }
    
    /* Estilos para la galería de imágenes */
    .gallery-container {
        display: flex;
        flex-wrap: wrap;
        gap: 15px;
        justify-content: center;
    }
    
    .gallery-container .item {
        width: calc(20% - 15px);
        max-width: 300px;
    }
    
    @media (max-width: 1200px) {
        .gallery-container .item {
            width: calc(25% - 15px);
        }
    }
    
    @media (max-width: 992px) {
        .gallery-container .item {
            width: calc(33.333% - 15px);
        }
    }
    
    @media (max-width: 768px) {
        .gallery-container .item {
            width: calc(50% - 15px);
        }
    }
    
    @media (max-width: 576px) {
        .gallery-container .item {
            width: 100%;
        }
    }
    
    hr {
        margin: 30px 0;
        border-color: #FFD1DC;
    }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg">
        <div class="container">
            <a class="navbar-brand" href="#">Mi Portfolio</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#portfolio">Trabajos</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contacto</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <section class="hero">
        <div class="hero-text">
            <h1>Bienvenido a mi Portafolio</h1>
            <p>Explora mis proyectos y conoce más sobre mi trabajo y las de mis compañeros.</p>
        </div>
    </section>

    <section id="portfolio" class="portfolio">
        <div class="container">
            <h2 class="text-center mb-4">Mis Trabajos</h2>
            <div class="row">
                <!-- Repetición 1 -->
                <div class="col-md-6 mb-4">
                    <div class="item card">
                        <img src="IMG_0604.JPG" alt="Sweet Cherry" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_0604.JPG')">
                    </div>
                </div>
                <div class="col-md-6 mb-4">
                    <div class="item card">
                        <img src="IMG_0633.JPG" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_0633.JPG')">
                    </div>
                </div>

                <hr>

                <!-- Repetición 2 -->
                <div class="col-md-6 mb-4">
                    <div class="item card">
                        <img src="foto 1 del greco.jpg" alt="Sweet Cherry" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('foto 1 del greco.jpg')">
                    </div>
                </div>
                <div class="col-md-6 mb-4">
                    <div class="item card">
                        <img src="FOTO DEL CHAVO COM filtro del greco.jpg" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('FOTO DEL CHAVO COM filtro del greco.jpg')">
                    </div>
                </div>

                <hr>

                <!-- Repetición 3 -->
                <div class="col-md-6 mb-4 mx-auto">
                    <div class="item card">
                        <img src="Imagen de WhatsApp 2025-03-14 a las 11.36.45_09a72a24.jpg" alt="Sweet Cherry" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('Imagen de WhatsApp 2025-03-14 a las 11.36.45_09a72a24.jpg')">
                    </div>
                </div>

                <hr>

                <!-- Repetición 4 -->
                <div class="col-12 mb-4">
                    <div class="centered-row">
                        <div class="item card">
                            <img src="EJE.JPG" alt="Sweet Cherry" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('EJE.JPG')">
                        </div>
                        <div class="item card">
                            <img src="Jerarquia.jpg" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('Jerarquia.jpg')">
                        </div>
                        <div class="item card">
                            <img src="PAUTA.JPG" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('PAUTA.JPG')">
                        </div>
                    </div>
                </div>
                
                <hr>

                 <!-- Repetición 5 -->
                 <div class="col-12 mb-4">
                    <div class="centered-row">
                        <div class="item card">
                            <img src="los peluches 4.jpg" alt="Sweet Cherry" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('los peluches 4.jpg')">
                        </div>
                        <div class="item card">
                            <img src="los peluches 2.jpg" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('los peluches 2.jpg')">
                        </div>
                        <div class="item card">
                            <img src="los peluches 1.jpg" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('los peluches 1.jpg')">
                        </div>
                        <div class="item card">
                            <img src="IMG_4924.JPG" alt="Delicious Fruit" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4924.JPG')">
                        </div>
                    </div>
                </div>

                <hr>

<!-- Repetición 6 (Galería de imágenes) -->
<div class="col-12">
    <h3 class="text-center mb-4">Galería de Proyectos</h3>
    <div class="gallery-container">
        <!-- Imágenes existentes -->
        <div class="item card">
            <img src="IMG-20250318-WA0038.jpg" alt="Imagen 1" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0038.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0037.jpg" alt="Imagen 2" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0037.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0036.jpg" alt="Imagen 3" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0036.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0035.jpg" alt="Imagen 4" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0035.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0034.jpg" alt="Imagen 5" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0034.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0033.jpg" alt="Imagen 6" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0033.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0032.jpg" alt="Imagen 7" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0032.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0031.jpg" alt="Imagen 9" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0031.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0030.jpg" alt="Imagen 11" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0030.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0029.jpg" alt="Imagen 12" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0029.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0028.jpg" alt="Imagen 13" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0028.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0027.jpg" alt="Imagen 14" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0027.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0026.jpg" alt="Imagen 15" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0026.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0025.jpg" alt="Imagen 16" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0025.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0024.jpg" alt="Imagen 17" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0024.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0023.jpg" alt="Imagen 18" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0023.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0022.jpg" alt="Imagen 19" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0022.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0021.jpg" alt="Imagen 20" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0021.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0020.jpg" alt="Imagen 21" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0020.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0019.jpg" alt="Imagen 22" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0019.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0018.jpg" alt="Imagen 23" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0018.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0017.jpg" alt="Imagen 24" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0017.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0016.jpg" alt="Imagen 25" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0016.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0015.jpg" alt="Imagen 26" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0015.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0014.jpg" alt="Imagen 27" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0014.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0013.jpg" alt="Imagen 28" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0013.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0012.jpg" alt="Imagen 29" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0012.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0011.jpg" alt="Imagen 30" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0011.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0010.jpg" alt="Imagen 31" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0010.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0009.jpg" alt="Imagen 32" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0009.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0008.jpg" alt="Imagen 33" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0008.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0007.jpg" alt="Imagen 34" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0007.jpg')">
        </div>
        <div class="item card">
            <img src="IMG-20250318-WA0006.jpg" alt="Imagen 35" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG-20250318-WA0006.jpg')">
        </div>
        <div class="item card">
            <img src="IMG_4924.JPG" alt="Imagen 36" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4924.JPG')">
        </div>
        <div class="item card">
            <img src="IMG_4027.jpeg" alt="Imagen 37" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4027.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4023.jpeg" alt="Imagen 38" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4023.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4022.jpeg" alt="Imagen 39" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4022.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4021.jpeg" alt="Imagen 40" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4021.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4018.jpeg" alt="Imagen 41" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4018.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4015.jpeg" alt="Imagen 42" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4015.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4009.jpeg" alt="Imagen 43" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4009.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4008.jpeg" alt="Imagen 44" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4008.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4006.jpeg" alt="Imagen 45" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4006.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4003.jpeg" alt="Imagen 46" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4003.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3999.jpeg" alt="Imagen 47" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3999.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3996.jpeg" alt="Imagen 48" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3996.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3995.jpeg" alt="Imagen 49" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3995.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3989.jpeg" alt="Imagen 50" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3989.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3987.jpeg" alt="Imagen 51" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3987.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3986.jpeg" alt="Imagen 52" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3986.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3984.jpeg" alt="Imagen 53" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3984.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3981.jpeg" alt="Imagen 54" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3981.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3977.jpeg" alt="Imagen 55" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3977.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3953.jpeg" alt="Imagen 56" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3953.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3943.jpeg" alt="Imagen 57" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3943.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3942.jpeg" alt="Imagen 58" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3942.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3934.jpeg" alt="Imagen 59" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3934.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3928.jpeg" alt="Imagen 60" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3928.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3927.jpeg" alt="Imagen 61" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3927.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3916.jpeg" alt="Imagen 62" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3916.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3912.jpeg" alt="Imagen 63" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3912.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3910.jpeg" alt="Imagen 64" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3910.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3899.jpeg" alt="Imagen 65" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3899.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3897.jpeg" alt="Imagen 66" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3897.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3895.jpeg" alt="Imagen 67" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3895.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_3894.jpeg" alt="Imagen 68" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_3894.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4184.jpeg" alt="Imagen 70" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4184.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4183.jpeg" alt="Imagen 71" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4183.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4181.jpeg" alt="Imagen 72" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4181.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4176.jpeg" alt="Imagen 73" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4176.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4175.jpeg" alt="Imagen 74" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4175.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4174.jpeg" alt="Imagen 75" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4174.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4172.jpeg" alt="Imagen 76" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4172.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4154.jpeg" alt="Imagen 77" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4154.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4153.jpeg" alt="Imagen 78" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4153.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4152.jpeg" alt="Imagen 79" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4152.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4151.jpeg" alt="Imagen 80" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4151.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4147.jpeg" alt="Imagen 81" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4147.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4146.jpeg" alt="Imagen 82" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4146.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4142.jpeg" alt="Imagen 83" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4142.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4144.jpeg" alt="Imagen 84" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4144.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4141.jpeg" alt="Imagen 85" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4141.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4140.jpeg" alt="Imagen 86" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4140.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4139.jpeg" alt="Imagen 87" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4139.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4138.jpeg" alt="Imagen 88" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4138.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4137.jpeg" alt="Imagen 89" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4137.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4136.jpeg" alt="Imagen 90" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4136.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4135.jpeg" alt="Imagen 91" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4135.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4134.jpeg" alt="Imagen 92" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4134.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4130.jpeg" alt="Imagen 93" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4130.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4125.jpeg" alt="Imagen 94" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4125.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4124.jpeg" alt="Imagen 95" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4124.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4116.jpeg" alt="Imagen 96" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4116.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4107.jpeg" alt="Imagen 97" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4107.jpeg')">
        </div>
        <!-- Nuevas imágenes -->
        <div class="item card">
            <img src="IMG_4317.jpeg" alt="Imagen 98" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4317.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4318.jpeg" alt="Imagen 99" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4318.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4319.jpeg" alt="Imagen 100" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4319.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4320.jpeg" alt="Imagen 101" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4320.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4321.jpeg" alt="Imagen 102" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4321.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4322.jpeg" alt="Imagen 103" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4322.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4323.jpeg" alt="Imagen 104" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4323.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4324.jpeg" alt="Imagen 105" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4324.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4325.jpeg" alt="Imagen 106" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4325.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4326.jpeg" alt="Imagen 107" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4326.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4327.jpeg" alt="Imagen 108" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4327.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4328.jpeg" alt="Imagen 109" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4328.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4329.jpeg" alt="Imagen 110" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4329.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4330.jpeg" alt="Imagen 111" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4330.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4331.jpeg" alt="Imagen 112" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4331.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4332.jpeg" alt="Imagen 113" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4332.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4333.jpeg" alt="Imagen 114" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4333.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4334.jpeg" alt="Imagen 115" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4334.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4335.jpeg" alt="Imagen 116" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4335.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4336.jpeg" alt="Imagen 117" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4336.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4338.jpeg" alt="Imagen 118" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4338.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4339.jpeg" alt="Imagen 119" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4339.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4340.jpeg" alt="Imagen 120" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4340.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4341.jpeg" alt="Imagen 121" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4341.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4342.jpeg" alt="Imagen 122" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4342.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4343.jpeg" alt="Imagen 123" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4343.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4344.jpeg" alt="Imagen 124" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4344.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4345.jpeg" alt="Imagen 125" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4345.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4346.jpeg" alt="Imagen 126" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4346.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4347.jpeg" alt="Imagen 127" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4347.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4348.jpeg" alt="Imagen 128" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4348.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4349.jpeg" alt="Imagen 129" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4349.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4350.jpeg" alt="Imagen 130" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4350.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4351.jpeg" alt="Imagen 131" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4351.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4352.jpeg" alt="Imagen 132" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4352.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4353.jpeg" alt="Imagen 133" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4353.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4354.jpeg" alt="Imagen 134" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4354.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4355.jpeg" alt="Imagen 135" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4355.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4356.jpeg" alt="Imagen 136" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4356.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4357.jpeg" alt="Imagen 137" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4357.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4358.jpeg" alt="Imagen 138" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4358.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4359.jpeg" alt="Imagen 139" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4359.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4360.jpeg" alt="Imagen 140" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4360.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4361.jpeg" alt="Imagen 141" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4361.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4362.jpeg" alt="Imagen 142" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4362.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4363.jpeg" alt="Imagen 143" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4363.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4364.jpeg" alt="Imagen 144" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4364.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4365.jpeg" alt="Imagen 145" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4365.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4366.jpeg" alt="Imagen 146" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4366.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4367.jpeg" alt="Imagen 147" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4367.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4368.jpeg" alt="Imagen 148" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4368.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4369.jpeg" alt="Imagen 149" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4369.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4370.jpeg" alt="Imagen 150" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4370.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4371.jpeg" alt="Imagen 151" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4371.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4372.jpeg" alt="Imagen 152" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4372.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4373.jpeg" alt="Imagen 153" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4373.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4374.jpeg" alt="Imagen 154" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4374.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4375.jpeg" alt="Imagen 155" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4375.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4376.jpeg" alt="Imagen 156" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4376.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4377.jpeg" alt="Imagen 157" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4377.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4378.jpeg" alt="Imagen 158" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4378.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4379.jpeg" alt="Imagen 159" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4379.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4381.jpeg" alt="Imagen 160" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4381.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4382.jpeg" alt="Imagen 161" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4382.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4383.jpeg" alt="Imagen 162" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4383.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4384.jpeg" alt="Imagen 163" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4384.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4385.jpeg" alt="Imagen 164" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4385.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4386.jpeg" alt="Imagen 165" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4386.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4387.jpeg" alt="Imagen 166" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4387.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4388.jpeg" alt="Imagen 167" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4388.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4389.jpeg" alt="Imagen 168" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4389.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4390.jpeg" alt="Imagen 169" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4390.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4391.jpeg" alt="Imagen 170" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4391.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4392.jpeg" alt="Imagen 171" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4392.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4393.jpeg" alt="Imagen 172" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4393.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4394.jpeg" alt="Imagen 173" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4394.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4395.jpeg" alt="Imagen 174" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4395.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4396.jpeg" alt="Imagen 175" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4396.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4398.jpeg" alt="Imagen 176" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4398.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4399.jpeg" alt="Imagen 177" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4399.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4400.jpeg" alt="Imagen 178" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4400.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4401.jpeg" alt="Imagen 179" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4401.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4402.jpeg" alt="Imagen 180" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4402.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4403.jpeg" alt="Imagen 181" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4403.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4404.jpeg" alt="Imagen 182" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4404.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4405.jpeg" alt="Imagen 183" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4405.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4406.jpeg" alt="Imagen 184" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4406.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4407.jpeg" alt="Imagen 185" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4407.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4408.jpeg" alt="Imagen 186" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4408.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4409.jpeg" alt="Imagen 187" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4409.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4410.jpeg" alt="Imagen 188" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4410.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4411.jpeg" alt="Imagen 189" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4411.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4412.jpeg" alt="Imagen 190" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4412.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4422.jpeg" alt="Imagen 191" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4422.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4423.jpeg" alt="Imagen 192" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4423.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4424.jpeg" alt="Imagen 193" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4424.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4425.jpeg" alt="Imagen 194" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4425.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4426.jpeg" alt="Imagen 195" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4426.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4427.jpeg" alt="Imagen 196" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4427.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4428.jpeg" alt="Imagen 197" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4428.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4429.jpeg" alt="Imagen 198" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4429.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4430.jpeg" alt="Imagen 199" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4430.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4431.jpeg" alt="Imagen 200" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4431.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4432.jpeg" alt="Imagen 201" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4432.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4433.jpeg" alt="Imagen 202" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4433.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4434.jpeg" alt="Imagen 203" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4434.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4435.jpeg" alt="Imagen 204" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4435.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4436.jpeg" alt="Imagen 205" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4436.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4437.jpeg" alt="Imagen 206" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4437.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4438.jpeg" alt="Imagen 207" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4438.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4439.jpeg" alt="Imagen 208" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4439.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4440.jpeg" alt="Imagen 209" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4440.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4441.jpeg" alt="Imagen 210" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4441.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4442.jpeg" alt="Imagen 211" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4442.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4443.jpeg" alt="Imagen 212" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4443.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4444.jpeg" alt="Imagen 213" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4444.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4445.jpeg" alt="Imagen 214" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4445.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4446.jpeg" alt="Imagen 215" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4446.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4447.jpeg" alt="Imagen 216" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4447.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4448.jpeg" alt="Imagen 217" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4448.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4449.jpeg" alt="Imagen 218" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4449.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4450.jpeg" alt="Imagen 219" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4450.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4451.jpeg" alt="Imagen 220" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4451.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4452.jpeg" alt="Imagen 221" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4452.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4453.jpeg" alt="Imagen 222" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4453.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4454.jpeg" alt="Imagen 223" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4454.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4455.jpeg" alt="Imagen 224" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4455.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4456.jpeg" alt="Imagen 225" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4456.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4457.jpeg" alt="Imagen 226" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4457.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4458.jpeg" alt="Imagen 227" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4458.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4459.jpeg" alt="Imagen 228" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4459.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4460.jpeg" alt="Imagen 229" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4460.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4461.jpeg" alt="Imagen 230" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4461.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4462.jpeg" alt="Imagen 231" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4462.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4464.jpeg" alt="Imagen 232" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4464.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4465.jpeg" alt="Imagen 233" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4465.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4466.jpeg" alt="Imagen 234" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4466.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4467.jpeg" alt="Imagen 235" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4467.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4468.jpeg" alt="Imagen 236" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4468.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4469.jpeg" alt="Imagen 237" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4469.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4470.jpeg" alt="Imagen 238" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4470.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4471.jpeg" alt="Imagen 239" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4471.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4472.jpeg" alt="Imagen 240" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4472.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4473.jpeg" alt="Imagen 241" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4473.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4474.jpeg" alt="Imagen 242" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4474.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4475.jpeg" alt="Imagen 243" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4475.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4476.jpeg" alt="Imagen 244" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4476.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4477.jpeg" alt="Imagen 245" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4477.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4478.jpeg" alt="Imagen 246" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4478.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4479.jpeg" alt="Imagen 247" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4479.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4481.jpeg" alt="Imagen 248" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4481.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4482.jpeg" alt="Imagen 249" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4482.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4483.jpeg" alt="Imagen 250" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4483.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4484.jpeg" alt="Imagen 251" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4484.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4485.jpeg" alt="Imagen 252" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4485.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4486.jpeg" alt="Imagen 253" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4486.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4487.jpeg" alt="Imagen 254" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4487.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4488.jpeg" alt="Imagen 255" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4488.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4489.jpeg" alt="Imagen 256" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4489.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4490.jpeg" alt="Imagen 257" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4490.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4491.jpeg" alt="Imagen 258" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4491.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4492.jpeg" alt="Imagen 259" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4492.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4493.jpeg" alt="Imagen 260" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4493.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4494.jpeg" alt="Imagen 261" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4494.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4495.jpeg" alt="Imagen 262" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4495.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4496.jpeg" alt="Imagen 263" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4496.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4497.jpeg" alt="Imagen 264" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4497.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4498.jpeg" alt="Imagen 265" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4498.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4499.jpeg" alt="Imagen 266" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4499.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4500.jpeg" alt="Imagen 267" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4500.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4501.jpeg" alt="Imagen 268" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4501.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4502.jpeg" alt="Imagen 269" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4502.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4503.jpeg" alt="Imagen 270" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4503.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4504.jpeg" alt="Imagen 271" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4504.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4505.jpeg" alt="Imagen 272" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4505.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4506.jpeg" alt="Imagen 273" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4506.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4507.jpeg" alt="Imagen 274" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4507.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4508.jpeg" alt="Imagen 275" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4508.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4509.jpeg" alt="Imagen 276" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4509.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4510.jpeg" alt="Imagen 277" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4510.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4511.jpeg" alt="Imagen 278" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4511.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4512.jpeg" alt="Imagen 279" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4512.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4513.jpeg" alt="Imagen 280" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4513.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4514.jpeg" alt="Imagen 281" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4514.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4515.jpeg" alt="Imagen 282" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4515.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4516.jpeg" alt="Imagen 283" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4516.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4517.jpeg" alt="Imagen 284" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4517.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4518.jpeg" alt="Imagen 285" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4518.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4519.jpeg" alt="Imagen 286" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4519.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4520.jpeg" alt="Imagen 287" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4520.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4521.jpeg" alt="Imagen 288" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4521.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4522.jpeg" alt="Imagen 289" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4522.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4523.jpeg" alt="Imagen 290" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4523.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4524.jpeg" alt="Imagen 291" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4524.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4525.jpeg" alt="Imagen 292" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4525.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4527.jpeg" alt="Imagen 293" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4527.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4528.jpeg" alt="Imagen 294" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4528.jpeg')">
        </div>
        <div class="item card">
            <img src="IMG_4529.jpeg" alt="Imagen 295" data-bs-toggle="modal" data-bs-target="#imageModal" onclick="updateModal('IMG_4529.jpeg')">
        </div>
    </div>
</div>

                    </div>
                </div>
            </div>
        </section>
    
    <!-- Modal para mostrar la imagen en tamaño completo -->
    <div class="modal fade" id="imageModal" tabindex="-1" aria-labelledby="imageModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered modal-lg">
            <div class="modal-content">
                <div class="modal-body text-center">
                    <img id="modalImage" src="" alt="Imagen completa" class="img-fluid">
                </div>
            </div>
        </div>
    </div>

    <footer id="contact" class="text-center p-4" style="background-color: #FFD1DC;">
        <p>VANESSA ARYL GONZALEZ MENDEZ</p>
    </footer>

    <script>
        // Función para actualizar la imagen del modal
        function updateModal(imageSrc) {
            document.getElementById('modalImage').src = imageSrc;
        }
    </script>
</body>
</html>
