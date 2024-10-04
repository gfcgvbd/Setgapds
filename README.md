<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App de Salud Infantil</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #a8e0ff, #ff9bff);
            color: #333;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }

        h1, h2 {
            text-align: center;
            color: #1a237e;
        }

        .card {
            margin: 20px 0;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.2s;
        }

        .card:hover {
            transform: scale(1.02);
        }

        .icons {
            color: #1a237e;
        }

        .tips, .recipes {
            margin: 10px 0;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            margin-top: 20px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        input, textarea, button {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            background: #1a237e;
            color: white;
            border: none;
            cursor: pointer;
            transition: background 0.3s;
        }

        button:hover {
            background: #0d47a1;
        }

        .login-register {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
        }

        .login-register div {
            width: 48%;
        }
        @media (max-width: 600px) {
    .container {
        width: 95%;
        padding: 15px;
    }

    h1, h2 {
        font-size: 1.5rem;
    }

    button {
        padding: 15px;
        font-size: 1.2rem;
    }

    input, textarea {
        padding: 12px;
        font-size: 1.1rem;
    }

    .card {
        margin: 10px 0;
        padding: 15px;
    }
}

    </style>
</head>
<body>
    <div class="container">
        <h1>App de Salud Infantil</h1>

        <!-- Sección de Registro e Inicio de Sesión -->
        <div class="card login-register">
            <!-- Registro -->
            <div>
                <h2>Regístrate</h2>
                <input type="text" placeholder="Correo electrónico" required>
                <input type="password" placeholder="Contraseña" required>
                <select required>
                    <option value="">¿Es tu primera vez usando una aplicación similar?</option>
                    <option value="si">Sí</option>
                    <option value="no">No</option>
                </select>
                <button>Registrarse</button>
            </div>

            <!-- Inicio de Sesión -->
            <div>
                <h2>Iniciar Sesión</h2>
                <input type="text" placeholder="Correo electrónico" required>
                <input type="password" placeholder="Contraseña" required>
                <button>Entrar</button>
            </div>
        </div>

        <!-- Bienvenida -->
        <div class="card">
            <h2>Bienvenido</h2>
            <p>La salud de su niño está en nuestras manos. Gracias por usar nuestra app para monitorear su bienestar.</p>
        </div>

        <!-- Datos del Niño -->
        <div class="card">
            <h2>Datos del Niño</h2>
            <input type="text" placeholder="Nombre del niño" required>
            <input type="number" placeholder="Edad" required>
            <input type="number" placeholder="Estatura (cm)" required>
            <input type="number" placeholder="Peso (kg)" required>
            <textarea rows="4" placeholder="¿Qué más debemos saber del niño?" required></textarea>
            <button>Guardar Datos</button>
        </div>

        <!-- Información sobre alimentación -->
        <div class="card">
            <h2>Información de Alimentación</h2>
            <p>Alimentos recomendados para el niño según su perfil:</p>
            <ul>
                <li>Desayunos recomendados: Avena, Frutas, Yogurt</li>
                <li>Almuerzos recomendados: Pollo, Verduras, Arroz integral</li>
                <li>Cenas recomendadas: Sopa ligera, Ensaladas</li>
            </ul>
        </div>

        <!-- Consejos para padres -->
        <div class="card">
            <h2>Consejos para Padres</h2>
            <div class="tips">
                <h3><i class="fas fa-lightbulb icons"></i> Consejos Prácticos:</h3>
                <ul>
                    <li><strong>Fomentar Hábitos Saludables:</strong> Involucra a tu hijo en la preparación de comidas saludables.</li>
                    <li><strong>Consultas Médicas Regulares:</strong> Visita a médicos regulares para asegurar que su crecimiento y desarrollo estén en buen camino.</li>
                    <li><strong>Ser un Modelo a Seguir:</strong> Los niños aprenden observando. Muestra hábitos saludables en tu propia alimentación y estilo de vida.</li>
                    <li><strong>Limitar el Azúcar:</strong> Trata de reducir el consumo de azúcares añadidos y alimentos altamente procesados en la dieta de tu hijo.</li>
                </ul>
            </div>
        </div>

        <!-- Recetas -->
        <div class="card">
            <h2>Recetas Saludables</h2>
            <p>Aquí encontrarás muchas recetas saludables adaptadas a las necesidades de tu hijo.</p>
            <button>Ver Recetas</button>
        </div>

        <!-- Contacto -->
        <div class="card contact" id="contacto">
            <h2>Contacto</h2>
            <p>Si tienes preguntas, sugerencias o comentarios, no dudes en contactarnos:</p>
            <p><strong>Email:</strong> <a href="mailto:appdesaludinfantil@gmail.com">appdesaludinfantil@gmail.com</a></p>
            <p><strong>Teléfono:</strong> +51 980 823 626</p>
            <form>
                <input type="text" placeholder="Nombre" required>
                <input type="email" placeholder="Correo Electrónico" required>
                <textarea rows="4" placeholder="Tu Mensaje" required></textarea>
                <button>Enviar Mensaje</button>
            </form>
        </div>

        <footer>
            <p>© 2024 App de Salud Infantil. Todos los derechos reservados.</p>
        </footer>
    </div>
</body>
</html>
