<!-- # index.html -->
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web App</title>
    
    <!-- Tailwind CSS -->
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <!-- DaisyUI -->
    <link href="https://cdn.jsdelivr.net/npm/daisyui@2.31.0/dist/full.css" rel="stylesheet">
    <!-- Material Icons -->
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <!-- Vue.js -->
    <script src="https://cdn.jsdelivr.net/npm/vue@2.6.14/dist/vue.js"></script>
    <!-- Firebase -->
    <script src="https://www.gstatic.com/firebasejs/8.6.8/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/8.6.8/firebase-auth.js"></script>
    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Google Maps API -->
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY"></script>

    <style>
        /* Custom Styles */
        #map {
            height: 400px;
            width: 100%;
        }
    </style>
</head>

<body class="bg-gray-100">
    <div id="app" class="container mx-auto p-4">
        <!-- Header -->
        <header class="text-center py-4">
            <h1 class="text-3xl font-bold">Welcome to My Web App</h1>
            <p class="text-gray-700">Built with Vue.js, Firebase, Google Maps, and Chart.js</p>
        </header>

        <!-- Login Section -->
        <div v-show="!loggedIn" class="flex justify-center">
            <button @click="loginGuest" class="btn btn-primary">Login as Guest</button>
        </div>

        <!-- Content Section -->
        <div v-show="loggedIn">
            <!-- Google Maps -->
            <div class="my-4">
                <h2 class="text-xl font-semibold">Google Map</h2>
                <div id="map"></div>
            </div>

            <!-- Chart.js Section -->
            <div class="my-4">
                <h2 class="text-xl font-semibold">Crypto Price Chart</h2>
                <canvas id="cryptoChart"></canvas>
            </div>

            <!-- Interactive Elements -->
            <div class="my-4">
                <h2 class="text-xl font-semibold">Interactive Section</h2>
                <button @click="animateElement" class="btn btn-secondary">Click to Animate</button>
                <div :class="{ 'animate-bounce': animate }" class="w-16 h-16 bg-blue-500 mt-4"></div>
            </div>
        </div>
    </div>

    <script>
        // Firebase Configuration
        var firebaseConfig = {
            apiKey: "YOUR_FIREBASE_API_KEY",
            authDomain: "your-app.firebaseapp.com",
            projectId: "your-app",
            storageBucket: "your-app.appspot.com",
            messagingSenderId: "123456789",
            appId: "1:123456789:web:abcdefgh"
        };
        // Initialize Firebase
        firebase.initializeApp(firebaseConfig);

        var app = new Vue({
            el: '#app',
            data: {
                loggedIn: false,
                animate: false,
            },
            methods: {
                loginGuest: function () {
                    firebase.auth().signInAnonymously().then((user) => {
                        console.log('User logged in as guest:', user);
                        this.loggedIn = true;
                        this.initMap();
                        this.loadCryptoData();
                    }).catch((error) => {
                        console.error('Error logging in:', error);
                    });
                },
                initMap: function () {
                    const map = new google.maps.Map(document.getElementById("map"), {
                        center: { lat: -34.397, lng: 150.644 },
                        zoom: 8,
                    });
                    console.log('Google Map initialized:', map);
                },
                loadCryptoData: function () {
                    fetch('https://min-api.cryptocompare.com/data/price?fsym=BTC&tsyms=USD,EUR')
                        .then(response => response.json())
                        .then(data => {
                            console.log('Crypto data:', data);
                            this.renderChart(data);
                        })
                        .catch(error => console.error('Error fetching crypto data:', error));
                },
                renderChart: function (data) {
                    const ctx = document.getElementById('cryptoChart').getContext('2d');
                    new Chart(ctx, {
                        type: 'bar',
                        data: {
                            labels: ['USD', 'EUR'],
                            datasets: [{
                                label: 'BTC Price',
                                data: [data.USD, data.EUR],
                                backgroundColor: ['rgba(75, 192, 192, 0.2)', 'rgba(153, 102, 255, 0.2)'],
                                borderColor: ['rgba(75, 192, 192, 1)', 'rgba(153, 102, 255, 1)'],
                                borderWidth: 1
                            }]
                        },
                        options: {
                            scales: {
                                y: {
                                    beginAtZero: true
                                }
                            }
                        }
                    });
                    console.log('Chart rendered');
                },
                animateElement: function () {
                    this.animate = !this.animate;
                }
            }
        });
    </script>
</body>

</html>
