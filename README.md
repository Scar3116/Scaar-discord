
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1">
    <title>Scaar'bot 2.0 - Bot Discord Futuriste</title>
    <meta name="description" content="Découvrez Scaar'bot 2.0, le bot Discord futuriste ultime avec des fonctionnalités avancées pour votre serveur. Invitez-le maintenant !">
    <meta property="og:title" content="Scaar'bot 2.0 - Bot Discord Futuriste">
    <meta property="og:description" content="Le bot Discord le plus avancé avec des fonctionnalités futuristes pour améliorer votre serveur Discord.">
    <meta property="og:type" content="website">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'orbitron': ['Orbitron', 'monospace'],
                        'inter': ['Inter', 'sans-serif']
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'glow': 'glow 2s ease-in-out infinite alternate',
                        'slide-up': 'slideUp 0.8s ease-out',
                        'fade-in': 'fadeIn 0.6s ease-out'
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-10px)' }
                        },
                        glow: {
                            'from': { textShadow: '0 0 20px #06b6d4, 0 0 30px #06b6d4, 0 0 40px #06b6d4' },
                            'to': { textShadow: '0 0 10px #06b6d4, 0 0 20px #06b6d4, 0 0 30px #06b6d4' }
                        },
                        slideUp: {
                            'from': { opacity: '0', transform: 'translateY(30px)' },
                            'to': { opacity: '1', transform: 'translateY(0)' }
                        },
                        fadeIn: {
                            'from': { opacity: '0' },
                            'to': { opacity: '1' }
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .glass-effect {
            background: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(6, 182, 212, 0.2);
        }
        .cyber-gradient {
            background: linear-gradient(45deg, #06b6d4, #8b5cf6, #ec4899);
        }
        .text-glow {
            text-shadow: 0 0 20px #06b6d4;
        }
        .hover-glow:hover {
            box-shadow: 0 0 30px rgba(6, 182, 212, 0.3);
            transform: translateY(-2px);
            transition: all 0.3s ease;
        }
        body {
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            color: #e2e8f0;
            font-family: 'Inter', sans-serif;
        }
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
        .animate-glow {
            animation: glow 2s ease-in-out infinite alternate;
        }
        .btn-primary {
            background: linear-gradient(45deg, #06b6d4, #8b5cf6);
            padding: 12px 32px;
            border-radius: 8px;
            color: white;
            font-weight: 600;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(6, 182, 212, 0.4);
        }
        .card {
            background: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(6, 182, 212, 0.2);
            border-radius: 12px;
            padding: 24px;
            margin-bottom: 24px;
        }
        .badge-premium {
            background: linear-gradient(45deg, #f59e0b, #ea580c);
            color: white;
            padding: 4px 8px;
            border-radius: 4px;
            font-size: 12px;
            font-weight: 600;
        }
        .nav-link {
            color: #94a3b8;
            text-decoration: none;
            padding: 8px 16px;
            border-radius: 6px;
            transition: all 0.3s ease;
        }
        .nav-link:hover {
            color: #06b6d4;
            background: rgba(6, 182, 212, 0.1);
        }
    </style>
</head>
<body>
    <div id="app">
        <!-- Navigation -->
        <nav class="fixed top-0 w-full z-50 glass-effect">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex justify-between h-16">
                    <div class="flex items-center">
                        <div class="flex-shrink-0 flex items-center">
                            <div class="w-8 h-8 cyber-gradient rounded-lg flex items-center justify-center mr-3">
                                <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
                                    <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3z"/>
                                </svg>
                            </div>
                            <span class="font-orbitron font-bold text-xl text-glow">Scaar'bot 2.0</span>
                        </div>
                    </div>
                    <div class="flex items-center space-x-4">
                        <a href="#home" class="nav-link">Accueil</a>
                        <a href="#commands" class="nav-link">Commandes</a>
                        <a href="#team" class="nav-link">Équipe</a>
                        <a href="#privacy" class="nav-link">Confidentialité</a>
                        <a href="https://discord.com/oauth2/authorize?client_id=YOUR_BOT_ID&permissions=8&scope=bot%20applications.commands" class="btn-primary">Inviter le Bot</a>
                    </div>
                </div>
            </div>
        </nav>

        <!-- Home Section -->
        <section id="home" class="min-h-screen pt-20 px-4 sm:px-6 lg:px-8">
            <div class="max-w-7xl mx-auto">
                <!-- Hero Section -->
                <div class="text-center py-20">
                    <div class="inline-flex items-center justify-center w-20 h-20 cyber-gradient rounded-full mb-8 animate-float">
                        <svg class="w-10 h-10 text-white" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3z"/>
                        </svg>
                    </div>
                    
                    <h1 class="font-orbitron text-5xl md:text-7xl font-bold text-glow mb-6 animate-glow">
                        Scaar'bot 2.0
                    </h1>
                    
                    <p class="text-xl md:text-2xl text-slate-300 mb-8 max-w-4xl mx-auto">
                        Le bot Discord du futur. Intelligence artificielle avancée, modération automatique, 
                        et plus de 100 commandes pour transformer votre serveur en expérience immersive.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row gap-4 justify-center mb-16">
                        <a href="https://discord.com/oauth2/authorize?client_id=YOUR_BOT_ID&permissions=8&scope=bot%20applications.commands" class="btn-primary">
                            Inviter Maintenant
                        </a>
                        <a href="#commands" class="nav-link border border-cyan-500/50 px-8 py-3 rounded-lg">
                            Voir les Commandes
                        </a>
                    </div>
                </div>

                <!-- Stats -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-6 mb-20">
                    <div class="card text-center">
                        <div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mx-auto mb-4">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M3 4a1 1 0 011-1h12a1 1 0 011 1v2a1 1 0 01-1 1H4a1 1 0 01-1-1V4zM3 10a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H4a1 1 0 01-1-1v-6zM14 9a1 1 0 00-1 1v6a1 1 0 001 1h2a1 1 0 001-1v-6a1 1 0 00-1-1h-2z"/>
                            </svg>
                        </div>
                        <div class="text-2xl font-bold text-cyan-400 mb-1">2,847</div>
                        <div class="text-sm text-slate-400">Serveurs Actifs</div>
                        <div class="text-xs text-emerald-400 mt-1">+12.5%</div>
                    </div>
                    
                    <div class="card text-center">
                        <div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-lg flex items-center justify-center mx-auto mb-4">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M9 6a3 3 0 11-6 0 3 3 0 016 0zM17 6a3 3 0 11-6 0 3 3 0 016 0zM12.93 17c.046-.327.07-.66.07-1a6.97 6.97 0 00-1.5-4.33A5 5 0 0119 16v1h-6.07zM6 11a5 5 0 015 5v1H1v-1a5 5 0 015-5z"/>
                            </svg>
                        </div>
                        <div class="text-2xl font-bold text-cyan-400 mb-1">156K</div>
                        <div class="text-sm text-slate-400">Utilisateurs</div>
                        <div class="text-xs text-emerald-400 mt-1">+8.2%</div>
                    </div>
                    
                    <div class="card text-center">
                        <div class="w-12 h-12 bg-gradient-to-r from-emerald-500 to-teal-500 rounded-lg flex items-center justify-center mx-auto mb-4">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M18 10c0 3.866-3.582 7-8 7a8.841 8.841 0 01-4.083-.98L2 17l1.338-3.123C2.493 12.767 2 11.434 2 10c0-3.866 3.582-7 8-7s8 3.134 8 7zM7 9H5v2h2V9zm8 0h-2v2h2V9zM9 9h2v2H9V9z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <div class="text-2xl font-bold text-cyan-400 mb-1">89K</div>
                        <div class="text-sm text-slate-400">Commandes/jour</div>
                        <div class="text-xs text-emerald-400 mt-1">+15.3%</div>
                    </div>
                    
                    <div class="card text-center">
                        <div class="w-12 h-12 bg-gradient-to-r from-orange-500 to-red-500 rounded-lg flex items-center justify-center mx-auto mb-4">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M12 7a1 1 0 110-2h5a1 1 0 011 1v5a1 1 0 11-2 0V8.414l-4.293 4.293a1 1 0 01-1.414 0L8 10.414l-4.293 4.293a1 1 0 01-1.414-1.414l5-5a1 1 0 011.414 0L11 10.586 14.586 7H12z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <div class="text-2xl font-bold text-cyan-400 mb-1">99.9%</div>
                        <div class="text-sm text-slate-400">Uptime</div>
                        <div class="text-xs text-emerald-400 mt-1">+0.1%</div>
                    </div>
                </div>

                <!-- Features -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-20">
                    <div class="card hover-glow">
                        <div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-lg flex items-center justify-center mb-4 animate-float">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M9.383 3.076A1 1 0 0110 4v12a1 1 0 01-1.617.76l-4-3.333H3a1 1 0 01-1-1V7.667a1 1 0 011-1h1.383l4-3.334zm7.133-.36c.11-.026.224-.026.334 0A8.968 8.968 0 0120 9c0 2.59-1.098 4.923-2.85 6.574-.135.135-.31.206-.49.206a.697.697 0 01-.49-.206c-.135-.135-.206-.31-.206-.49 0-.18.071-.355.206-.49A6.975 6.975 0 0018 9c0-2.019-.854-3.84-2.224-5.13-.135-.135-.206-.31-.206-.49s.071-.355.206-.49z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <h3 class="font-orbitron text-xl font-bold text-glow mb-3">Musique Avancée</h3>
                        <p class="text-slate-300">Lecture haute qualité avec playlists personnalisées et contrôles vocaux</p>
                    </div>
                    
                    <div class="card hover-glow">
                        <div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center mb-4 animate-float" style="animation-delay: 0.1s">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M2.166 4.999A11.954 11.954 0 0010 1.944 11.954 11.954 0 0017.834 5c.11.65.166 1.32.166 2.001 0 5.225-3.34 9.67-8 11.317C5.34 16.67 2 12.225 2 7c0-.682.057-1.35.166-2.001zm11.541 3.708a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <h3 class="font-orbitron text-xl font-bold text-glow mb-3">Modération IA</h3>
                        <p class="text-slate-300">Protection automatique contre le spam et contenu inapproprié</p>
                    </div>
                    
                    <div class="card hover-glow">
                        <div class="w-12 h-12 bg-gradient-to-r from-emerald-500 to-teal-500 rounded-lg flex items-center justify-center mb-4 animate-float" style="animation-delay: 0.2s">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M11 17a1 1 0 001.447.894l4-2A1 1 0 0017 15V9.236a1 1 0 00-1.447-.894l-4 2a1 1 0 00-.553.894V17zM15.211 6.276a1 1 0 000-1.788l-4.764-2.382a1 1 0 00-.894 0L4.789 4.488a1 1 0 000 1.788l4.764 2.382a1 1 0 00.894 0l4.764-2.382zM4.447 8.342A1 1 0 003 9.236V15a1 1 0 00.553.894l4 2A1 1 0 009 17v-5.764a1 1 0 00-.553-.894l-4-2z"/>
                            </svg>
                        </div>
                        <h3 class="font-orbitron text-xl font-bold text-glow mb-3">Jeux Interactifs</h3>
                        <p class="text-slate-300">Mini-jeux multijoueurs et système de classement</p>
                    </div>
                    
                    <div class="card hover-glow">
                        <div class="w-12 h-12 bg-gradient-to-r from-orange-500 to-red-500 rounded-lg flex items-center justify-center mb-4 animate-float" style="animation-delay: 0.3s">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M5 2a1 1 0 011 1v1h1a1 1 0 010 2H6v1a1 1 0 01-2 0V6H3a1 1 0 010-2h1V3a1 1 0 011-1zm0 10a1 1 0 011 1v1h1a1 1 0 110 2H6v1a1 1 0 11-2 0v-1H3a1 1 0 110-2h1v-1a1 1 0 011-1zM12 2a1 1 0 01.967.744L14.146 7.2 17.5 9.134a1 1 0 010 1.732L14.146 12.8l-1.179 4.456a1 1 0 01-1.934 0L9.854 12.8 6.5 10.866a1 1 0 010-1.732L9.854 7.2l1.179-4.456A1 1 0 0112 2z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <h3 class="font-orbitron text-xl font-bold text-glow mb-3">Système de Niveaux</h3>
                        <p class="text-slate-300">XP, récompenses et rôles automatiques pour l'engagement</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Commands Section -->
        <section id="commands" class="min-h-screen py-20 px-4 sm:px-6 lg:px-8">
            <div class="max-w-7xl mx-auto">
                <div class="text-center mb-16">
                    <div class="inline-flex items-center justify-center w-16 h-16 cyber-gradient rounded-full mb-6 animate-float">
                        <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3z"/>
                        </svg>
                    </div>
                    
                    <h1 class="font-orbitron text-4xl md:text-5xl font-bold text-glow mb-4">
                        Commandes du Bot
                    </h1>
                    
                    <p class="text-lg text-slate-400 max-w-3xl mx-auto mb-8">
                        Découvrez toutes les commandes disponibles de Scaar'bot 2.0. 
                        Plus de 100 commandes pour personnaliser votre expérience Discord.
                    </p>
                    
                    <div class="flex items-center justify-center gap-2 text-sm text-slate-400">
                        <svg class="w-4 h-4 text-yellow-400" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M11.3 1.046A1 1 0 0112 2v5h4a1 1 0 01.82 1.573l-7 10A1 1 0 018 18v-5H4a1 1 0 01-.82-1.573l7-10a1 1 0 011.12-.38z" clip-rule="evenodd"/>
                        </svg>
                        <span>Les commandes premium sont marquées avec un badge spécial</span>
                    </div>
                </div>

                <!-- Music Commands -->
                <div class="mb-12">
                    <div class="flex items-center space-x-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-lg flex items-center justify-center animate-float">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M9.383 3.076A1 1 0 0110 4v12a1 1 0 01-1.617.76l-4-3.333H3a1 1 0 01-1-1V7.667a1 1 0 011-1h1.383l4-3.334z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <h2 class="font-orbitron text-2xl font-bold text-glow">Musique</h2>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        <div class="card hover-glow">
                            <div class="flex items-center justify-between mb-3">
                                <h3 class="font-orbitron text-lg text-cyan-400">/play</h3>
                            </div>
                            <p class="text-slate-300 mb-3">Jouer une musique depuis YouTube, Spotify ou SoundCloud</p>
                            <p class="text-sm text-slate-400">Usage: /play [titre/url]</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <div class="flex items-center justify-between mb-3">
                                <h3 class="font-orbitron text-lg text-cyan-400">/queue</h3>
                            </div>
                            <p class="text-slate-300 mb-3">Afficher la file d'attente actuelle</p>
                            <p class="text-sm text-slate-400">Usage: /queue</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <div class="flex items-center justify-between mb-3">
                                <h3 class="font-orbitron text-lg text-cyan-400">/lyrics</h3>
                                <span class="badge-premium">PREMIUM</span>
                            </div>
                            <p class="text-slate-300 mb-3">Afficher les paroles de la musique actuelle</p>
                            <p class="text-sm text-slate-400">Usage: /lyrics</p>
                        </div>
                    </div>
                </div>

                <!-- Moderation Commands -->
                <div class="mb-12">
                    <div class="flex items-center space-x-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-lg flex items-center justify-center animate-float">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M2.166 4.999A11.954 11.954 0 0010 1.944 11.954 11.954 0 0017.834 5c.11.65.166 1.32.166 2.001 0 5.225-3.34 9.67-8 11.317C5.34 16.67 2 12.225 2 7c0-.682.057-1.35.166-2.001z" clip-rule="evenodd"/>
                            </svg>
                        </div>
                        <h2 class="font-orbitron text-2xl font-bold text-glow">Modération</h2>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        <div class="card hover-glow">
                            <h3 class="font-orbitron text-lg text-cyan-400 mb-3">/ban</h3>
                            <p class="text-slate-300 mb-3">Bannir un membre du serveur</p>
                            <p class="text-sm text-slate-400">Usage: /ban [@membre] [raison]</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <h3 class="font-orbitron text-lg text-cyan-400 mb-3">/kick</h3>
                            <p class="text-slate-300 mb-3">Expulser un membre du serveur</p>
                            <p class="text-sm text-slate-400">Usage: /kick [@membre] [raison]</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <div class="flex items-center justify-between mb-3">
                                <h3 class="font-orbitron text-lg text-cyan-400">/automod</h3>
                                <span class="badge-premium">PREMIUM</span>
                            </div>
                            <p class="text-slate-300 mb-3">Configurer la modération automatique</p>
                            <p class="text-sm text-slate-400">Usage: /automod [enable/disable]</p>
                        </div>
                    </div>
                </div>

                <!-- Games Commands -->
                <div class="mb-12">
                    <div class="flex items-center space-x-4 mb-8">
                        <div class="w-12 h-12 bg-gradient-to-r from-emerald-500 to-teal-500 rounded-lg flex items-center justify-center animate-float">
                            <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M11 17a1 1 0 001.447.894l4-2A1 1 0 0017 15V9.236a1 1 0 00-1.447-.894l-4 2a1 1 0 00-.553.894V17z"/>
                            </svg>
                        </div>
                        <h2 class="font-orbitron text-2xl font-bold text-glow">Jeux</h2>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        <div class="card hover-glow">
                            <h3 class="font-orbitron text-lg text-cyan-400 mb-3">/rps</h3>
                            <p class="text-slate-300 mb-3">Jouer à Pierre-Papier-Ciseaux</p>
                            <p class="text-sm text-slate-400">Usage: /rps [pierre/papier/ciseaux]</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <h3 class="font-orbitron text-lg text-cyan-400 mb-3">/trivia</h3>
                            <p class="text-slate-300 mb-3">Questions-réponses multijoueurs</p>
                            <p class="text-sm text-slate-400">Usage: /trivia [difficulté]</p>
                        </div>
                        
                        <div class="card hover-glow">
                            <div class="flex items-center justify-between mb-3">
                                <h3 class="font-orbitron text-lg text-cyan-400">/casino</h3>
                                <span class="badge-premium">PREMIUM</span>
                            </div>
                            <p class="text-slate-300 mb-3">Jeux de casino avec économie virtuelle</p>
                            <p class="text-sm text-slate-400">Usage: /casino [jeu]</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Team Section -->
        <section id="team" class="min-h-screen py-20 px-4 sm:px-6 lg:px-8">
            <div class="max-w-7xl mx-auto">
                <div class="text-center mb-16">
                    <div class="inline-flex items-center justify-center w-16 h-16 cyber-gradient rounded-full mb-6 animate-float">
                        <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M9 6a3 3 0 11-6 0 3 3 0 016 0zM17 6a3 3 0 11-6 0 3 3 0 016 0zM12.93 17c.046-.327.07-.66.07-1a6.97 6.97 0 00-1.5-4.33A5 5 0 0119 16v1h-6.07zM6 11a5 5 0 015 5v1H1v-1a5 5 0 015-5z"/>
                        </svg>
                    </div>
                    
                    <h1 class="font-orbitron text-4xl md:text-5xl font-bold text-glow mb-4">
                        Notre Équipe
                    </h1>
                    
                    <p class="text-lg text-slate-400 max-w-3xl mx-auto">
                        Rencontrez les visionnaires derrière Scaar'bot 2.0. Une équipe passionnée 
                        dédiée à révolutionner l'expérience Discord avec des technologies de pointe.
                    </p>
                </div>

                <!-- Team Members -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-16">
                    <div class="card hover-glow">
                        <div class="flex items-start space-x-6">
                            <div class="w-20 h-20 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full flex items-center justify-center flex-shrink-0 animate-float">
                                <span class="text-white font-bold text-xl font-orbitron">AC</span>
                            </div>
                            
                            <div class="flex-1">
                                <h3 class="font-orbitron text-xl font-bold text-glow mb-1">Alex Cyber</h3>
                                <p class="text-cyan-400 font-medium mb-3">Lead Developer</p>
                                <p class="text-slate-300 text-sm mb-4 leading-relaxed">
                                    Architecte principal de Scaar'bot 2.0, spécialisé en intelligence artificielle et systèmes distribués.
                                </p>
                                
                                <div class="flex flex-wrap gap-2 mb-4">
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Python</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Node.js</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Machine Learning</span>
                                </div>
                                
                                <div class="flex space-x-4">
                                    <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors">
                                        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
                                            <path fill-rule="evenodd" d="M10 0C4.477 0 0 4.484 0 10.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0110 4.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.942.359.31.678.921.678 1.856 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0020 10.017C20 4.484 15.522 0 10 0z" clip-rule="evenodd"/>
                                        </svg>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="card hover-glow">
                        <div class="flex items-start space-x-6">
                            <div class="w-20 h-20 bg-gradient-to-r from-purple-500 to-pink-500 rounded-full flex items-center justify-center flex-shrink-0 animate-float">
                                <span class="text-white font-bold text-xl font-orbitron">SN</span>
                            </div>
                            
                            <div class="flex-1">
                                <h3 class="font-orbitron text-xl font-bold text-glow mb-1">Sarah Neural</h3>
                                <p class="text-cyan-400 font-medium mb-3">AI Specialist</p>
                                <p class="text-slate-300 text-sm mb-4 leading-relaxed">
                                    Experte en IA conversationnelle et traitement du langage naturel pour les interactions avancées.
                                </p>
                                
                                <div class="flex flex-wrap gap-2 mb-4">
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">TensorFlow</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">NLP</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Deep Learning</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="card hover-glow">
                        <div class="flex items-start space-x-6">
                            <div class="w-20 h-20 bg-gradient-to-r from-emerald-500 to-teal-500 rounded-full flex items-center justify-center flex-shrink-0 animate-float">
                                <span class="text-white font-bold text-xl font-orbitron">MS</span>
                            </div>
                            
                            <div class="flex-1">
                                <h3 class="font-orbitron text-xl font-bold text-glow mb-1">Max Security</h3>
                                <p class="text-cyan-400 font-medium mb-3">Security Engineer</p>
                                <p class="text-slate-300 text-sm mb-4 leading-relaxed">
                                    Responsable de la sécurité et de la protection des données utilisateurs et serveurs.
                                </p>
                                
                                <div class="flex flex-wrap gap-2 mb-4">
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Cybersecurity</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Encryption</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="card hover-glow">
                        <div class="flex items-start space-x-6">
                            <div class="w-20 h-20 bg-gradient-to-r from-orange-500 to-red-500 rounded-full flex items-center justify-center flex-shrink-0 animate-float">
                                <span class="text-white font-bold text-xl font-orbitron">LD</span>
                            </div>
                            
                            <div class="flex-1">
                                <h3 class="font-orbitron text-xl font-bold text-glow mb-1">Luna Design</h3>
                                <p class="text-cyan-400 font-medium mb-3">UX/UI Designer</p>
                                <p class="text-slate-300 text-sm mb-4 leading-relaxed">
                                    Créatrice de l'interface futuriste et de l'expérience utilisateur révolutionnaire.
                                </p>
                                
                                <div class="flex flex-wrap gap-2 mb-4">
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">Figma</span>
                                    <span class="px-2 py-1 bg-slate-800/50 border border-slate-700 rounded text-xs text-slate-300">UI/UX</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Stats -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                    <div class="card text-center">
                        <div class="text-3xl font-bold text-cyan-400 mb-2">25+</div>
                        <div class="text-slate-400">Années d'Expérience</div>
                    </div>
                    <div class="card text-center">
                        <div class="text-3xl font-bold text-cyan-400 mb-2">100+</div>
                        <div class="text-slate-400">Projets Réalisés</div>
                    </div>
                    <div class="card text-center">
                        <div class="text-3xl font-bold text-cyan-400 mb-2">1M+</div>
                        <div class="text-slate-400">Utilisateurs Servis</div>
                    </div>
                    <div class="card text-center">
                        <div class="text-3xl font-bold text-cyan-400 mb-2">99.9%</div>
                        <div class="text-slate-400">Uptime Garanti</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Privacy Section -->
        <section id="privacy" class="min-h-screen py-20 px-4 sm:px-6 lg:px-8">
            <div class="max-w-4xl mx-auto">
                <div class="text-center mb-16">
                    <div class="inline-flex items-center justify-center w-16 h-16 cyber-gradient rounded-full mb-6 animate-float">
                        <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M2.166 4.999A11.954 11.954 0 0010 1.944 11.954 11.954 0 0017.834 5c.11.65.166 1.32.166 2.001 0 5.225-3.34 9.67-8 11.317C5.34 16.67 2 12.225 2 7c0-.682.057-1.35.166-2.001z" clip-rule="evenodd"/>
                        </svg>
                    </div>
                    
                    <h1 class="font-orbitron text-4xl md:text-5xl font-bold text-glow mb-4">
                        Politique de Confidentialité
                    </h1>
                    
                    <div class="text-sm text-slate-400 mb-8">
                        Dernière mise à jour : 17 juin 2025
                    </div>
                </div>

                <!-- Privacy Content -->
                <div class="card mb-12">
                    <h2 class="font-orbitron text-2xl font-bold text-glow mb-4">Notre Engagement</h2>
                    <p class="text-slate-300 leading-relaxed mb-6">
                        Chez Scaar'bot 2.0, nous nous engageons à protéger votre vie privée et vos données personnelles. 
                        Cette politique de confidentialité explique comment nous collectons, utilisons, stockons et 
                        protégeons vos informations lorsque vous utilisez notre bot Discord.
                    </p>
                    
                    <h3 class="font-orbitron text-xl font-bold text-cyan-400 mb-3">Données Collectées</h3>
                    <ul class="text-slate-300 space-y-2 mb-6">
                        <li>• Identifiants Discord (ID utilisateur, serveur)</li>
                        <li>• Messages et commandes utilisées</li>
                        <li>• Statistiques d'utilisation anonymisées</li>
                        <li>• Préférences et configurations personnalisées</li>
                    </ul>
                    
                    <h3 class="font-orbitron text-xl font-bold text-cyan-400 mb-3">Utilisation des Données</h3>
                    <p class="text-slate-300 leading-relaxed mb-6">
                        Nous utilisons vos données uniquement pour améliorer les fonctionnalités du bot, 
                        personnaliser votre expérience et assurer la sécurité de nos services.
                    </p>
                    
                    <h3 class="font-orbitron text-xl font-bold text-cyan-400 mb-3">Protection et Sécurité</h3>
                    <p class="text-slate-300 leading-relaxed">
                        Toutes les données sont chiffrées et stockées de manière sécurisée. Nous ne partageons 
                        jamais vos informations personnelles avec des tiers sans votre consentement explicite.
                    </p>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="border-t border-slate-800 py-12 px-4 sm:px-6 lg:px-8">
            <div class="max-w-7xl mx-auto">
                <div class="text-center">
                    <div class="flex items-center justify-center mb-4">
                        <div class="w-8 h-8 cyber-gradient rounded-lg flex items-center justify-center mr-3">
                            <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
                                <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3z"/>
                            </svg>
                        </div>
                        <span class="font-orbitron font-bold text-xl text-glow">Scaar'bot 2.0</span>
                    </div>
                    
                    <p class="text-slate-400 mb-6">
                        Le bot Discord du futur, développé avec passion pour votre communauté.
                    </p>
                    
                    <div class="flex justify-center space-x-6 mb-8">
                        <a href="#home" class="nav-link">Accueil</a>
                        <a href="#commands" class="nav-link">Commandes</a>
                        <a href="#team" class="nav-link">Équipe</a>
                        <a href="#privacy" class="nav-link">Confidentialité</a>
                    </div>
                    
                    <div class="border-t border-slate-800 pt-8">
                        <p class="text-slate-500 text-sm">
                            © 2025 Scaar'bot 2.0. Tous droits réservés.
                        </p>
                    </div>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add active state to navigation
        const sections = document.querySelectorAll('section[id]');
        const navLinks = document.querySelectorAll('a[href^="#"]');

        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if (scrollY >= sectionTop - 200) {
                    current = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.classList.remove('text-cyan-400');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('text-cyan-400');
                }
            });
        });

        // Add intersection observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Observe all cards for animation
        document.querySelectorAll('.card').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(30px)';
            card.style.transition = 'all 0.6s ease-out';
            observer.observe(card);
        });
    </script>
</body>
</html>
