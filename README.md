<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spider-Man Cast Members</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #1a2a6c);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: #fff;
            min-height: 100vh;
            padding: 20px;
            position: relative;
        }
        
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            padding: 30px 0;
            margin-bottom: 30px;
            position: relative;
        }
        
        h1 {
            font-size: 3.5rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.7);
            margin-bottom: 10px;
            position: relative;
            display: inline-block;
        }
        
        h1:after {
            content: "";
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 200px;
            height: 4px;
            background: linear-gradient(90deg, transparent, #ff0000, transparent);
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #ffd700;
            margin-top: 10px;
        }
        
        .cast-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .cast-card {
            background: rgba(0, 0, 0, 0.7);
            border-radius: 15px;
            overflow: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
            position: relative;
        }
        
        .cast-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(255, 0, 0, 0.4);
            background: rgba(0, 0, 0, 0.9);
        }
        
        .card-header {
            padding: 25px 20px 20px;
            position: relative;
            text-align: center;
            border-bottom: 2px solid #ff0000;
        }
        
        .main-cast .card-header {
            background: linear-gradient(to right, #8e0e00, #1a2a6c);
        }
        
        .supporting-cast .card-header {
            background: linear-gradient(to right, #1a2a6c, #000);
        }
        
        .actor-name {
            font-size: 1.8rem;
            margin-bottom: 5px;
            color: #ffd700;
            text-shadow: 0 0 5px rgba(255, 215, 0, 0.5);
        }
        
        .character-name {
            font-size: 1.3rem;
            color: #ff6b6b;
            font-style: italic;
        }
        
        .card-content {
            padding: 20px;
            text-align: center;
        }
        
        .actor-info {
            display: flex;
            justify-content: space-around;
            margin: 15px 0;
        }
        
        .info-item {
            text-align: center;
            padding: 10px;
        }
        
        .info-item i {
            font-size: 1.5rem;
            color: #ff6b6b;
            margin-bottom: 5px;
        }
        
        .info-label {
            font-size: 0.9rem;
            color: #aaa;
        }
        
        .info-value {
            font-size: 1.1rem;
            font-weight: bold;
            color: #fff;
        }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #ff0000, transparent);
            margin: 25px 0;
        }
        
        .show-more {
            text-align: center;
            margin-top: 40px;
        }
        
        .show-more-btn {
            background: linear-gradient(to right, #8e0e00, #1a2a6c);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1.2rem;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .show-more-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(255, 0, 0, 0.5);
        }
        
        .spider-logo {
            position: absolute;
            top: 20px;
            right: 20px;
            width: 80px;
            height: 80px;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><path d="M50 15a35 35 0 1 0 0 70 35 35 0 0 0 0-70zm0 5a30 30 0 1 1 0 60 30 30 0 0 1 0-60z" fill="red"/><path d="M50 30a20 20 0 1 0 0 40 20 20 0 0 0 0-40z" fill="white"/><path d="M50 20l-10 30h20z" fill="red"/></svg>') no-repeat center;
            background-size: contain;
            opacity: 0.3;
        }
        
        .web-effect {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            background: 
                radial-gradient(circle at 20% 30%, rgba(255,255,255,0.05) 0%, transparent 10%),
                radial-gradient(circle at 80% 70%, rgba(255,255,255,0.05) 0%, transparent 10%);
            z-index: -1;
        }
        
        @media (max-width: 768px) {
            .cast-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="web-effect"></div>
    <div class="container">
        <header>
            <div class="spider-logo"></div>
            <h1>Spider-Man Cast</h1>
            <p class="subtitle">Meet the characters from the Spider-Man universe</p>
        </header>
        
        <div class="cast-grid">
            <!-- Main Cast -->
            <div class="cast-card main-cast">
                <div class="card-header">
                    <h2 class="actor-name">Tobey Maguire</h2>
                    <p class="character-name">Spider-Man, Peter Parker</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">12 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card main-cast">
                <div class="card-header">
                    <h2 class="actor-name">Kirsten Dunst</h2>
                    <p class="character-name">Mary Jane Watson</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">8 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card main-cast">
                <div class="card-header">
                    <h2 class="actor-name">Willem Dafoe</h2>
                    <p class="character-name">Norman Osborn</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">2 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">20 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="divider"></div>
            
            <!-- Supporting Cast -->
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">James Franco</h2>
                    <p class="character-name">Harry Osborn</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">5 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Elizabeth Banks</h2>
                    <p class="character-name">Betty Brant</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">2 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">3 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Joe Manganiello</h2>
                    <p class="character-name">Flash Thompson</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">2 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">1 Win</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="divider"></div>
            
            <!-- Additional Cast -->
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">J. K. Simmons</h2>
                    <p class="character-name">J. Jonah Jameson</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">Oscar Winner</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Rosemary Harris</h2>
                    <p class="character-name">Aunt May</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">4 Wins</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Cliff Robertson</h2>
                    <p class="character-name">Ben Parker</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">2 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-award"></i>
                            <div class="info-label">Awards</div>
                            <div class="info-value">Oscar Winner</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="divider"></div>
            
            <!-- More Cast -->
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Randy Savage</h2>
                    <p class="character-name">Bone Saw McGraw</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">1 Film</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-trophy"></i>
                            <div class="info-label">Wrestling</div>
                            <div class="info-value">Champion</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Bill Nunn</h2>
                    <p class="character-name">Robbie Robertson</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">3 Films</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-theater-masks"></i>
                            <div class="info-label">Theater</div>
                            <div class="info-value">Broadway</div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="cast-card supporting-cast">
                <div class="card-header">
                    <h2 class="actor-name">Kristen Marie Holly</h2>
                    <p class="character-name">Young Lady at Fire</p>
                </div>
                <div class="card-content">
                    <div class="actor-info">
                        <div class="info-item">
                            <i class="fas fa-film"></i>
                            <div class="info-label">Appearances</div>
                            <div class="info-value">1 Film</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-graduation-cap"></i>
                            <div class="info-label">Education</div>
                            <div class="info-value">NYU Grad</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="show-more">
            <button class="show-more-btn">
                <i class="fas fa-chevron-down"></i> Show More Cast Members
            </button>
        </div>
    </div>

    <script>
        // Simple animation for the show more button
        document.querySelector('.show-more-btn').addEventListener('click', function() {
            alert('More cast members would load here in a real implementation!');
            this.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Loading...';
            
            setTimeout(() => {
                this.innerHTML = '<i class="fas fa-check"></i> More Cast Loaded!';
                this.style.background = 'linear-gradient(to right, #1a2a6c, #008000)';
            }, 1500);
        });
        
        // Add subtle hover effect to all cast cards
        const cards = document.querySelectorAll('.cast-card');
        cards.forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'translateY(-10px)';
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'translateY(0)';
            });
        });
    </script>
</body>
</html>
