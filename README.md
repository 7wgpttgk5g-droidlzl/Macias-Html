<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luis Macías - Entrenador Personal</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8f9fa;
        }
        .gradient-header {
            background: linear-gradient(180deg, #374151 0%, #111827 100%);
        }
        .yellow-bg {
            background-color: #facc15;
        }
        .btn-yellow {
            background-color: #facc15;
            transition: all 0.2s ease;
        }
        .btn-yellow:hover {
            background-color: #eab308;
            transform: translateY(-2px);
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
        }
        .card-shadow {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        /* Sticky Chat Button */
        .chat-btn {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 60px;
            height: 60px;
            background-color: #facc15;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 4px 15px rgba(250, 204, 21, 0.4);
            cursor: pointer;
            z-index: 50;
            transition: transform 0.2s ease;
        }
        .chat-btn:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body class="text-gray-800 antialiased">

    <header class="gradient-header text-white pt-12 pb-8 px-4 text-center relative overflow-hidden">
        <div class="max-w-md mx-auto relative z-10">
            <div class="w-24 h-24 bg-white rounded-xl mx-auto flex items-center justify-center text-4xl mb-4 shadow-lg">
                💪
            </div>
            <h1 class="text-3xl font-bold mb-2">LUIS MACÍAS</h1>
            <p class="text-gray-300 mb-6">Instructor Especializado en Fitness Integral</p>
            
            <div class="inline-flex items-center bg-yellow-400 text-gray-900 px-6 py-2 rounded-full font-bold shadow-md">
                <i class="fas fa-dumbbell mr-2"></i> SMART FIT
            </div>
        </div>
        <!-- Decorative circles -->
        <div class="absolute top-4 left-4 w-16 h-16 bg-white opacity-5 rounded-full"></div>
        <div class="absolute bottom-4 right-4 w-24 h-24 bg-white opacity-5 rounded-full"></div>
    </header>

    <section class="yellow-bg py-10 px-4">
        <div class="max-w-md mx-auto">
            <div class="text-center mb-8">
                <span class="bg-red-600 text-white text-xs font-bold px-3 py-1 rounded-full uppercase tracking-wide inline-block mb-4 shadow-sm">
                    🔥 Oferta por tiempo limitado
                </span>
                <h2 class="text-3xl font-extrabold text-gray-900 mb-2">¡PROMOCIONES ESPECIALES!</h2>
                <p class="text-gray-800 font-medium">Aprovecha estos precios únicos - Solo hasta fin de mes</p>
                <div class="w-12 h-1 bg-white mx-auto mt-4 rounded-full"></div>
            </div>

            <!-- Promocion 1: Prueba Semanal -->
            <div class="bg-white rounded-3xl p-6 mb-6 card-shadow relative">
                <div class="absolute -top-3 left-1/2 transform -translate-x-1/2">
                    <span class="bg-red-600 text-white text-xs font-bold px-4 py-1 rounded-full uppercase">Popular</span>
                </div>
                <div class="text-center mb-6 pt-2">
                    <h3 class="text-xl font-bold mb-1">PRUEBA SEMANAL</h3>
                    <p class="text-blue-600 font-medium text-sm">1 Persona • 1 Semana</p>
                </div>
                <div class="text-center mb-2">
                    <span class="text-gray-400 line-through text-lg mr-2">$800</span>
                    <span class="text-blue-600 text-4xl font-extrabold">$600</span>
                </div>
                <div class="text-center mb-6">
                    <span class="text-green-500 font-bold text-sm">¡AHORRA $200!</span>
                </div>
                <ul class="space-y-3 mb-8">
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">5 sesiones de 1 hora</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Evaluación física gratuita</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Plan de ejercicios personalizado</span>
                    </li>
                </ul>
                <button class="w-full btn-yellow text-gray-900 font-bold py-4 rounded-2xl text-lg" onclick="sendMessage('¡Hola! Me interesa la promoción PRUEBA SEMANAL de $600.')">
                    ¡QUIERO ESTA OFERTA!
                </button>
            </div>

            <!-- Promocion 2: Transformacion Total -->
            <div class="bg-white rounded-3xl p-6 mb-6 card-shadow relative">
                <div class="absolute -top-3 left-1/2 transform -translate-x-1/2">
                    <span class="bg-yellow-400 text-gray-900 text-xs font-bold px-4 py-1 rounded-full uppercase shadow-sm">Mejor Valor</span>
                </div>
                <div class="text-center mb-6 pt-2">
                    <h3 class="text-xl font-bold mb-1">TRANSFORMACIÓN TOTAL</h3>
                    <p class="text-blue-600 font-medium text-sm">1 Persona • 4 Semanas</p>
                </div>
                <div class="text-center mb-2">
                    <span class="text-gray-400 line-through text-lg mr-2">$3,000</span>
                    <span class="text-blue-600 text-4xl font-extrabold">$2,400</span>
                </div>
                <div class="text-center mb-6">
                    <span class="text-green-500 font-bold text-sm">¡AHORRA $600!</span>
                </div>
                <ul class="space-y-3 mb-8">
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">20 sesiones de entrenamiento</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Evaluación de progreso continuo</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Seguimiento semanal</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Asesoría WhatsApp incluida</span>
                    </li>
                </ul>
                <button class="w-full btn-yellow text-gray-900 font-bold py-4 rounded-2xl text-lg" onclick="sendMessage('¡Hola! Me interesa la promoción TRANSFORMACIÓN TOTAL de $2,400.')">
                    ¡APROVECHA AHORA!
                </button>
            </div>

            <!-- Promocion 3: Entrena en Pareja -->
            <div class="bg-white rounded-3xl p-6 mb-6 card-shadow relative">
                <div class="absolute -top-3 left-1/2 transform -translate-x-1/2">
                    <span class="bg-pink-500 text-white text-xs font-bold px-4 py-1 rounded-full uppercase">Parejas</span>
                </div>
                <div class="text-center mb-6 pt-2">
                    <h3 class="text-xl font-bold mb-1">ENTRENA EN PAREJA</h3>
                    <p class="text-blue-600 font-medium text-sm">2 Personas • 4 Semanas</p>
                </div>
                <div class="text-center mb-2">
                    <span class="text-gray-400 line-through text-lg mr-2">$4,400</span>
                    <span class="text-blue-600 text-4xl font-extrabold">$3,600</span>
                </div>
                <div class="text-center mb-6">
                    <span class="text-green-500 font-bold text-sm">¡AHORRA $800!</span>
                </div>
                <ul class="space-y-3 mb-8">
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">20 sesiones para ambos</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Motivación mutua</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Rutinas complementarias</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Precio por persona: $1,800</span>
                    </li>
                </ul>
                <button class="w-full btn-yellow text-gray-900 font-bold py-4 rounded-2xl text-lg" onclick="sendMessage('¡Hola! Me interesa la promoción ENTRENA EN PAREJA de $3,600.')">
                    ¡ENTRENA JUNTOS!
                </button>
            </div>

            <!-- Countdown Banner -->
            <div class="bg-red-600 rounded-3xl p-6 text-center text-white card-shadow">
                <div class="flex items-center justify-center mb-4">
                    <i class="far fa-clock text-2xl mr-2"></i>
                    <h3 class="text-xl font-bold">OFERTA TERMINA EN:</h3>
                </div>
                <div class="flex justify-center space-x-6 mb-4 font-bold">
                    <div>
                        <div class="text-4xl" id="days">24</div>
                        <div class="text-xs tracking-wider uppercase opacity-90">Días</div>
                    </div>
                    <div>
                        <div class="text-4xl" id="hours">7</div>
                        <div class="text-xs tracking-wider uppercase opacity-90">Horas</div>
                    </div>
                    <div>
                        <div class="text-4xl" id="mins">49</div>
                        <div class="text-xs tracking-wider uppercase opacity-90">Min</div>
                    </div>
                </div>
                <p class="text-sm opacity-90">*Solo quedan 8 cupos disponibles este mes</p>
            </div>
        </div>
    </section>

    <section class="py-12 px-4 bg-gray-50">
        <div class="max-w-md mx-auto">
            <div class="text-center mb-10">
                <h2 class="text-3xl font-bold text-gray-900 mb-2">Precios Regulares</h2>
                <p class="text-gray-500">Después de las promociones, estos son nuestros precios estándar</p>
                <div class="w-12 h-1 bg-yellow-400 mx-auto mt-4 rounded-full"></div>
            </div>

            <!-- 1 Persona Reg -->
            <div class="bg-white rounded-3xl p-6 mb-6 card-shadow text-center">
                <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4 text-blue-500 text-2xl">
                    <i class="fas fa-user"></i>
                </div>
                <h3 class="text-2xl font-bold mb-1">1 PERSONA</h3>
                <p class="text-blue-600 text-sm font-semibold mb-6 uppercase">Entrenamiento Personalizado</p>
                
                <div class="bg-gray-50 rounded-2xl p-4 flex justify-between items-center mb-4 border border-gray-100">
                    <span class="text-gray-600 font-medium">1 SEMANA</span>
                    <span class="text-blue-600 font-bold text-xl">$600</span>
                </div>
                <div class="bg-gray-50 rounded-2xl p-4 flex justify-between items-center border border-gray-100">
                    <span class="text-gray-600 font-medium">4 SEMANAS</span>
                    <span class="text-blue-600 font-bold text-xl">$3,000</span>
                </div>
            </div>

            <!-- 2 Personas Reg -->
            <div class="bg-white rounded-3xl p-6 card-shadow text-center mb-12">
                <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4 text-blue-500 text-2xl">
                    <i class="fas fa-user-friends"></i>
                </div>
                <h3 class="text-2xl font-bold mb-1">2 PERSONAS</h3>
                <p class="text-blue-600 text-sm font-semibold mb-6 uppercase">Entrenamiento en Pareja</p>
                
                <div class="bg-gray-50 rounded-2xl p-4 flex justify-between items-center mb-4 border border-gray-100">
                    <span class="text-gray-600 font-medium">1 SEMANA</span>
                    <span class="text-blue-600 font-bold text-xl">$900</span>
                </div>
                <div class="bg-gray-50 rounded-2xl p-4 flex justify-between items-center border border-gray-100">
                    <span class="text-gray-600 font-medium">4 SEMANAS</span>
                    <span class="text-blue-600 font-bold text-xl">$4,400</span>
                </div>
            </div>
            
            <div class="text-center mb-8 pt-8 border-t border-gray-200">
                <h2 class="text-3xl font-bold text-gray-900 mb-2">¿Qué Incluye?</h2>
                <div class="w-12 h-1 bg-yellow-400 mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="space-y-4">
                <!-- Include 1 -->
                <div class="bg-white rounded-3xl p-6 card-shadow text-center">
                    <div class="w-12 h-12 bg-yellow-100 rounded-full flex items-center justify-center mx-auto mb-3 text-red-500 text-xl">
                        <i class="far fa-clock"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-2">Horario Flexible</h4>
                    <p class="text-gray-500 text-sm">1 hora diaria, 5 días por semana (Lunes a Viernes)</p>
                </div>
                <!-- Include 2 -->
                <div class="bg-white rounded-3xl p-6 card-shadow text-center">
                    <div class="w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center mx-auto mb-3 text-xl">
                        <i class="fas fa-check"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-2">Corrección de Técnica</h4>
                    <p class="text-gray-500 text-sm">Supervisión constante para mejores resultados</p>
                </div>
            </div>

            <div class="text-center mb-8 mt-12">
                <h2 class="text-2xl font-bold text-gray-900 mb-2">Servicios Adicionales</h2>
                <div class="w-10 h-1 bg-red-600 mx-auto mt-4 rounded-full"></div>
                <p class="text-gray-500 mt-3 text-sm">La nutrición se maneja de forma independiente para ofrecerte una atención 100% especializada.</p>
            </div>

            <!-- Tarjeta de Nutrición Aparte -->
            <div class="bg-white rounded-3xl p-6 card-shadow border-2 border-green-500 relative mb-6">
                <div class="absolute -top-3 left-1/2 transform -translate-x-1/2 w-full text-center">
                    <span class="bg-green-500 text-white text-xs font-bold px-4 py-1.5 rounded-full uppercase shadow-sm">
                        Nutrición y Suplementación
                    </span>
                </div>
                <div class="text-center mb-4 pt-5">
                    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-3 text-green-600 text-3xl">
                        🥗
                    </div>
                    <h3 class="text-2xl font-bold mb-1">Consulta Nutricional</h3>
                    <p class="text-green-600 font-extrabold text-4xl my-3">$400</p>
                </div>
                <ul class="space-y-3 mb-6">
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700"><strong>2 menús</strong> personalizados</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Asesoría en <strong>suplementación</strong></span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-check text-green-500 mt-1 mr-3"></i>
                        <span class="text-gray-700">Modificaciones y ajustes incluidos</span>
                    </li>
                </ul>
                <button class="w-full bg-green-500 hover:bg-green-600 text-white font-bold py-4 rounded-2xl text-lg transition shadow-md flex items-center justify-center" onclick="sendMessage('¡Hola Luis! Me interesa agendar una cita para la Consulta Nutricional de $400.')">
                    <i class="fab fa-whatsapp text-2xl mr-2"></i> Agendar Cita
                </button>
            </div>
        </div>
    </section>

    <section class="gradient-header py-12 px-4 text-white">
        <div class="max-w-md mx-auto">
            <div class="text-center mb-10">
                <h2 class="text-2xl font-bold mb-2">Certificaciones y Especialidades</h2>
                <div class="w-12 h-1 bg-red-600 mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="space-y-4">
                <div class="bg-gray-800/50 backdrop-blur-sm border border-gray-700 rounded-2xl p-5 flex items-center">
                    <span class="text-2xl mr-4">🏆</span>
                    <span class="font-medium">Entrenamiento Especializado para Mujeres</span>
                </div>
                <div class="bg-gray-800/50 backdrop-blur-sm border border-gray-700 rounded-2xl p-5 flex items-center">
                    <span class="text-2xl mr-4">🥗</span>
                    <span class="font-medium">Asesor en Nutrición Deportiva</span>
                </div>
                <div class="bg-gray-800/50 backdrop-blur-sm border border-gray-700 rounded-2xl p-5 flex items-center">
                    <span class="text-2xl mr-4">💪</span>
                    <span class="font-medium">Diploma de Fisicoconstructivismo</span>
                </div>
                <div class="bg-gray-800/50 backdrop-blur-sm border border-gray-700 rounded-2xl p-5 flex items-center">
                    <span class="text-2xl mr-4">🎯</span>
                    <span class="font-medium">Instructor en Fitness Integral</span>
                </div>
                <div class="bg-gray-800/50 backdrop-blur-sm border border-gray-700 rounded-2xl p-5 flex items-center">
                    <span class="text-2xl mr-4">💊</span>
                    <span class="font-medium">Certificación en Asesor en Suplementación</span>
                </div>
            </div>
        </div>
    </section>

    <section class="yellow-bg py-12 px-4">
        <div class="max-w-md mx-auto">
            <h2 class="text-2xl font-bold text-center text-gray-900 mb-8 px-4">
                ¡Contáctame para Más Información!
            </h2>

            <div class="space-y-4 mb-8">
                <!-- Phone -->
                <a href="tel:3329512916" class="block bg-white rounded-2xl p-6 text-center card-shadow transition hover:scale-105">
                    <i class="fas fa-mobile-alt text-2xl text-gray-600 mb-2"></i>
                    <h4 class="font-bold text-gray-900 mb-1">Teléfono</h4>
                    <p class="text-gray-600">332 951 2916</p>
                </a>
                
                <!-- Email -->
                <a href="mailto:ja6774356@gmail.com" class="block bg-white rounded-2xl p-6 text-center card-shadow transition hover:scale-105">
                    <i class="far fa-envelope text-2xl text-blue-400 mb-2"></i>
                    <h4 class="font-bold text-gray-900 mb-1">Email</h4>
                    <p class="text-gray-600">ja6774356@gmail.com</p>
                </a>

                <!-- Location -->
                <div class="bg-white rounded-2xl p-6 text-center card-shadow">
                    <i class="fas fa-map-pin text-2xl text-red-500 mb-2"></i>
                    <h4 class="font-bold text-gray-900 mb-1">Ubicación</h4>
                    <p class="text-gray-600">León Campestre</p>
                </div>
            </div>

            <!-- Action Buttons -->
            <div class="space-y-4">
                <a href="tel:3329512916" class="flex items-center justify-center w-full bg-orange-500 hover:bg-orange-600 text-white font-bold py-4 rounded-full text-lg transition shadow-md">
                    <i class="fas fa-phone-alt mr-2"></i> Llamar Ahora
                </a>
                <a href="mailto:ja6774356@gmail.com" class="flex items-center justify-center w-full bg-transparent border-2 border-white hover:bg-white/20 text-white font-bold py-4 rounded-full text-lg transition">
                    <i class="far fa-envelope mr-2"></i> Enviar Email
                </a>
            </div>
        </div>
    </section>

    <footer class="gradient-header py-8 px-4 text-center">
        <div class="max-w-md mx-auto text-gray-400">
            <p class="font-bold text-white text-lg mb-1">LUIS MACÍAS - Entrenador Personal</p>
            <p class="text-sm mb-4">Smart Fit • León Campestre</p>
            <div class="w-16 h-1 bg-red-600 mx-auto mb-4 rounded-full"></div>
            <p class="text-sm italic">Transforma tu cuerpo, transforma tu vida</p>
        </div>
    </footer>

    <!-- WhatsApp Floating Button -->
    <div class="chat-btn" onclick="sendMessage('¡Hola Luis! Vengo de tu página web y quiero más información sobre tus entrenamientos.')">
        <i class="fab fa-whatsapp text-white text-3xl"></i>
    </div>

    <script>
        // Número de WhatsApp configurado
        const WHATSAPP_NUMBER = "523329512916"; 

        function sendMessage(customMessage) {
            const url = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(customMessage)}`;
            window.open(url, '_blank');
        }

        // Script del temporizador (Visual)
        function updateCountdown() {
            let hours = document.getElementById('hours').innerText;
            let mins = document.getElementById('mins').innerText;

            let h = parseInt(hours);
            let m = parseInt(mins);

            if (m > 0) {
                m--;
            } else {
                if (h > 0) {
                    h--;
                    m = 59;
                }
            }

            document.getElementById('hours').innerText = h.toString().padStart(2, '0');
            document.getElementById('mins').innerText = m.toString().padStart(2, '0');
        }

        // Actualizar cada minuto
        setInterval(updateCountdown, 60000);
    </script>
</body>
</html>