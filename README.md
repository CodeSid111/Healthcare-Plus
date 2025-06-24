# Healthcare-Plus
A blend of Economy &amp; Quality Healthcare Solutions 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HealthCare Plus - Your Complete Health Solution</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        .header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            box-shadow: 0 2px 20px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 2rem;
            font-weight: bold;
            color: #667eea;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        
        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: #667eea;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.9), rgba(118, 75, 162, 0.9));
            color: white;
            padding: 4rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            animation: fadeInUp 1s ease;
        }
        
        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            animation: fadeInUp 1s ease 0.3s both;
        }
        
        .cta-button {
            display: inline-block;
            background: #fff;
            color: #667eea;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
            animation: fadeInUp 1s ease 0.6s both;
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        
        /* Main Content */
        .main-content {
            background: white;
            padding: 3rem 0;
        }
        
        .section {
            margin-bottom: 4rem;
        }
        
        .section h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #667eea;
            position: relative;
        }
        
        .section h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 2px;
        }
        
        /* Age-wise Packages */
        .packages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        .package-card {
            background: white;
            border-radius: 15px;
            padding: 2rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            border: 2px solid transparent;
        }
        
        .package-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 50px rgba(0,0,0,0.15);
            border-color: #667eea;
        }
        
        .package-header {
            text-align: center;
            margin-bottom: 1.5rem;
        }
        
        .age-badge {
            background: linear-gradient(90deg, #667eea, #764ba2);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            font-weight: bold;
            margin-bottom: 1rem;
        }
        
        .package-title {
            font-size: 1.5rem;
            color: #333;
            margin-bottom: 0.5rem;
        }
        
        .pricing {
            text-align: center;
            margin-bottom: 1.5rem;
        }
        
        .original-price {
            font-size: 1.1rem;
            color: #999;
            text-decoration: line-through;
        }
        
        .discounted-price {
            font-size: 2rem;
            color: #667eea;
            font-weight: bold;
            margin: 0.5rem 0;
        }
        
        .discount-badge {
            background: #ff6b6b;
            color: white;
            padding: 0.25rem 0.5rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .package-features {
            list-style: none;
            margin-bottom: 1.5rem;
        }
        
        .package-features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #eee;
            display: flex;
            align-items: center;
        }
        
        .package-features li::before {
            content: '✓';
            color: #28a745;
            font-weight: bold;
            margin-right: 0.5rem;
        }
        
        .package-button {
            width: 100%;
            background: linear-gradient(90deg, #667eea, #764ba2);
            color: white;
            padding: 1rem;
            border: none;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s;
        }
        
        .package-button:hover {
            transform: scale(1.05);
        }
        
        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background: white;
            border-radius: 15px;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
        }
        
        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .service-title {
            font-size: 1.3rem;
            color: #333;
            margin-bottom: 1rem;
        }
        
        .service-description {
            color: #666;
            margin-bottom: 1.5rem;
        }
        
        .service-button {
            background: #667eea;
            color: white;
            padding: 0.75rem 1.5rem;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .service-button:hover {
            background: #5a6fd8;
        }
        
        /* Partners Section */
        .partners-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .partner-card {
            background: white;
            border-radius: 15px;
            padding: 2rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .partner-name {
            font-size: 1.5rem;
            color: #667eea;
            margin-bottom: 1rem;
        }
        
        .partner-offers {
            background: #f8f9fa;
            padding: 1rem;
            border-radius: 10px;
            margin-bottom: 1rem;
        }
        
        /* Subscription Section */
        .subscription-card {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            border-radius: 20px;
            padding: 3rem;
            text-align: center;
            margin: 2rem 0;
        }
        
        .subscription-title {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .subscription-benefits {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            margin: 2rem 0;
        }
        
        .benefit-item {
            background: rgba(255,255,255,0.1);
            padding: 1rem;
            border-radius: 10px;
        }
        
        /* Footer */
        .footer {
            background: #333;
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .packages-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <nav class="nav">
                <div class="logo">HealthCare Plus</div>
                <ul class="nav-links">
                    <li><a href="#packages">Packages</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#partners">Partners</a></li>
                    <li><a href="#subscription">Subscription</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Your Complete Health Solution</h1>
            <p>Discounted health services, diagnostic tests, pharmacy, and emergency care - all in one place</p>
            <a href="#packages" class="cta-button">Explore Packages</a>
        </div>
    </section>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            
            <!-- Age-wise Center Visit Packages -->
            <section id="packages" class="section">
                <h2>Age-Specific Health Packages - Center Visit</h2>
                <div class="packages-grid">
                    
                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">18-34 Years</div>
                            <h3 class="package-title">Young Adult Essential</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹2,999</div>
                            <div class="discounted-price">₹1,499</div>
                            <span class="discount-badge">50% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>Complete Blood Count (CBC)</li>
                            <li>Lipid Profile</li>
                            <li>Liver Function Test</li>
                            <li>Kidney Function Test</li>
                            <li>Thyroid Profile</li>
                            <li>Vitamin D & B12</li>
                            <li>Free Doctor Consultation</li>
                        </ul>
                        <button class="package-button">Book Now</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">35-40 Years</div>
                            <h3 class="package-title">Career Prime Health</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹4,999</div>
                            <div class="discounted-price">₹2,499</div>
                            <span class="discount-badge">50% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>All Young Adult tests</li>
                            <li>Diabetes Screening (HbA1c)</li>
                            <li>Cardiac Risk Assessment</li>
                            <li>Stress Test (Cortisol)</li>
                            <li>Eye & Vision Test</li>
                            <li>Blood Pressure Monitoring</li>
                            <li>Nutritionist Consultation</li>
                        </ul>
                        <button class="package-button">Book Now</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">41-54 Years</div>
                            <h3 class="package-title">Mid-Life Comprehensive</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹7,999</div>
                            <div class="discounted-price">₹3,999</div>
                            <span class="discount-badge">50% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>All Career Prime tests</li>
                            <li>Cancer Markers Screening</li>
                            <li>Bone Density Test</li>
                            <li>Hormonal Assessment</li>
                            <li>ECG & ECHO</li>
                            <li>Mammography/Prostate Check</li>
                            <li>Specialist Consultation</li>
                        </ul>
                        <button class="package-button">Book Now</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">55+ Years</div>
                            <h3 class="package-title">Senior Wellness Plus</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹12,999</div>
                            <div class="discounted-price">₹6,499</div>
                            <span class="discount-badge">50% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>All Mid-Life tests</li>
                            <li>Comprehensive Cancer Screening</li>
                            <li>Cognitive Assessment</li>
                            <li>Advanced Cardiac Tests</li>
                            <li>Arthritis Panel</li>
                            <li>Geriatric Consultation</li>
                            <li>Annual Health Monitoring</li>
                        </ul>
                        <button class="package-button">Book Now</button>
                    </div>
                </div>
            </section>

            <!-- Home Visit Packages -->
            <section class="section">
                <h2>Home Visit Health Packages</h2>
                <div class="packages-grid">
                    
                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">18-34 Male</div>
                            <h3 class="package-title">Young Male Home Care</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹3,499</div>
                            <div class="discounted-price">₹1,999</div>
                            <span class="discount-badge">43% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>Home Sample Collection</li>
                            <li>Testosterone Levels</li>
                            <li>Fitness Assessment</li>
                            <li>Basic Health Panel</li>
                            <li>Free Home Consultation</li>
                        </ul>
                        <button class="package-button">Book Home Visit</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">18-34 Female</div>
                            <h3 class="package-title">Young Female Home Care</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹3,499</div>
                            <div class="discounted-price">₹1,999</div>
                            <span class="discount-badge">43% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>Home Sample Collection</li>
                            <li>Hormonal Profile</li>
                            <li>Iron & Hemoglobin</li>
                            <li>Reproductive Health Panel</li>
                            <li>Free Home Consultation</li>
                        </ul>
                        <button class="package-button">Book Home Visit</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">35-40 Male</div>
                            <h3 class="package-title">Prime Male Home Care</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹5,499</div>
                            <div class="discounted-price">₹2,999</div>
                            <span class="discount-badge">45% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>Comprehensive Male Panel</li>
                            <li>Prostate Health Check</li>
                            <li>Cardiac Risk Assessment</li>
                            <li>Home BP Monitoring</li>
                            <li>Lifestyle Consultation</li>
                        </ul>
                        <button class="package-button">Book Home Visit</button>
                    </div>

                    <div class="package-card">
                        <div class="package-header">
                            <div class="age-badge">35-40 Female</div>
                            <h3 class="package-title">Prime Female Home Care</h3>
                        </div>
                        <div class="pricing">
                            <div class="original-price">₹5,499</div>
                            <div class="discounted-price">₹2,999</div>
                            <span class="discount-badge">45% OFF</span>
                        </div>
                        <ul class="package-features">
                            <li>Women's Wellness Panel</li>
                            <li>Breast Health Assessment</li>
                            <li>Hormonal Balance Check</li>
                            <li>Fertility Panel</li>
                            <li>Gynecologist Consultation</li>
                        </ul>
                        <button class="package-button">Book Home Visit</button>
                    </div>
                </div>
            </section>

            <!-- Services Section -->
            <section id="services" class="section">
                <h2>Our Complete Health Services</h2>
                <div class="services-grid">
                    
                    <div class="service-card">
                        <div class="service-icon">🏥</div>
                        <h3 class="service-title">Diagnostic Centers</h3>
                        <p class="service-description">State-of-the-art diagnostic facilities with advanced equipment and certified technicians</p>
                        <button class="service-button">Find Centers</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">💊</div>
                        <h3 class="service-title">Online Pharmacy</h3>
                        <p class="service-description">Genuine medicines delivered to your doorstep with up to 25% discount</p>
                        <button class="service-button">Order Medicines</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">🏪</div>
                        <h3 class="service-title">Offline Pharmacies</h3>
                        <p class="service-description">Partner pharmacies in your neighborhood with exclusive member discounts</p>
                        <button class="service-button">Locate Pharmacy</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">💪</div>
                        <h3 class="service-title">Health Clubs</h3>
                        <p class="service-description">Premium fitness centers and wellness clubs with special membership rates</p>
                        <button class="service-button">Join Club</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">🏋️</div>
                        <h3 class="service-title">Gymnasiums</h3>
                        <p class="service-description">Professional gyms with modern equipment and certified trainers</p>
                        <button class="service-button">Find Gyms</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">🚨</div>
                        <h3 class="service-title">Emergency Services</h3>
                        <p class="service-description">24/7 emergency medical services with ambulance and rapid response</p>
                        <button class="service-button">Emergency Call</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">👨⚕️</div>
                        <h3 class="service-title">Doctors on Call</h3>
                        <p class="service-description">Qualified doctors available for home visits and teleconsultations</p>
                        <button class="service-button">Call Doctor</button>
                    </div>

                    <div class="service-card">
                        <div class="service-icon">🏥</div>
                        <h3 class="service-title">OPD Services</h3>
                        <p class="service-description">Outpatient department services with specialist consultations</p>
                        <button class="service-button">Book OPD</button>
                    </div>
                </div>
            </section>

            <!-- Partners Section -->
            <section id="partners" class="section">
                <h2>Our Trusted Partners</h2>
                <div class="partners-grid">
                    
                    <div class="partner-card">
                        <h3 class="partner-name">MediLab Diagnostics</h3>
                        <div class="partner-offers">
                            <p><strong>Rack Rate:</strong> ₹2,500</p>
                            <p><strong>Our Rate:</strong> ₹1,250 (50% Off)</p>
                            <p><strong>Special Offers:</strong> Free home collection, Same day reports</p>
                        </div>
                        <button class="service-button">View Details</button>
                    </div>

                    <div class="partner-card">
                        <h3 class="partner-name">HealthFirst Pharmacy</h3>
                        <div class="partner-offers">
                            <p><strong>Rack Rate:</strong> MRP</p>
                            <p><strong>Our Rate:</strong> MRP - 25%</p>
                            <p><strong>Special Offers:</strong> Free delivery above ₹500, Generic alternatives</p>
                        </div>
                        <button class="service-button">View Details</button>
                    </div>

                    <div class="partner-card">
                        <h3 class="partner-name">FitZone Gymnasium</h3>
                        <div class="partner-offers">
                            <p><strong>Rack Rate:</strong> ₹3,000/month</p>
                            <p><strong>Our Rate:</strong> ₹2,000/month (33% Off)</p>
                            <p><strong>Special Offers:</strong> Free trainer sessions, Nutrition counseling</p>
                        </div>
                        <button class="service-button">View Details</button>
                    </div>

                    <div class="partner-card">
                        <h3 class="partner-name">CityLife Emergency</h3>
                        <div class="partner-offers">
                            <p><strong>Rack Rate:</strong> ₹2,000</p>
                            <p><strong>Our Rate:</strong> ₹1,500 (25% Off)</p>
                            <p><strong>Special Offers:</strong> 24/7 availability, ICU ambulance</p>
                        </div>
                        <button class="service-button">View Details</button>
                    </div>
                </div>
            </section>

            <!-- Subscription Section -->
            <section id="subscription" class="section">
                <div class="subscription-card">
                    <h2 class="subscription-title">HealthCare Plus Premium</h2>
                    <p>Unlock unlimited access to all our services with deeper discounts and exclusive benefits</p>
                    
                    <div class="subscription-benefits">
                        <div class="benefit-item">
                            <h4>Unlimited Consultations</h4>
                            <p>Free doctor consultations via call/video</p>
                        </div>
                        <div class="benefit-item">
                            <h4>Priority Booking</h4>
                            <p>Skip the queue with priority appointments</p>
                        </div>
                        <div class="benefit-item">
                            <h4>Extra 20% Off</h4>
                            <p>Additional discounts on all services</p>
                        </div>
                        <div class="benefit-item">
                            <h4>Free Home Visits</h4>
                            <p>Unlimited free sample collection</p>
                        </div>
                    </div>
                    
                    <div class="pricing">
                        <div class="original-price">₹12,000/year</div>
                        <div class="discounted-price">₹6,999/year</div>
                        <span class="discount-badge">42% OFF</span>
                    </div>
                    
                    <button class="cta-button">Subscribe Now</button>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2025 HealthCare Plus. All rights reserved. | Contact: +91-9876543210 | Email: info@healthcareplus.com</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Add click handlers for buttons
        document.querySelectorAll('.package-button, .service-button').forEach(button => {
            button.addEventListener('click', function() {
                alert('Feature coming soon! Thank you for your interest.');
            });
        });
    </script>
</body>
</html>
