# bernabasmatric<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bernabas Bmatric - Real Estate Agent</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .business-card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
            max-width: 420px;
            width: 100%;
            overflow: hidden;
            transition: transform 0.3s ease;
        }
        
        .business-card:hover {
            transform: translateY(-5px);
        }
        
        .card-header {
            background: linear-gradient(135deg, #c1440e, #e55d17);
            color: white;
            padding: 30px 20px;
            text-align: center;
            position: relative;
        }
        
        .card-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #ffd700, #ffed4e);
        }
        
        .profile-img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid white;
            margin: 0 auto 15px;
            background: #f8f9fa;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 40px;
            color: #c1440e;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .name {
            font-size: 26px;
            font-weight: bold;
            margin-bottom: 5px;
        }
        
        .title {
            font-size: 18px;
            opacity: 0.95;
            margin-bottom: 5px;
            font-weight: 600;
        }
        
        .company {
            font-size: 16px;
            opacity: 0.9;
            font-weight: 500;
        }
        
        .card-body {
            padding: 30px;
        }
        
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-bottom: 25px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px;
            border-radius: 12px;
            transition: all 0.3s ease;
            cursor: pointer;
            border: 1px solid #f1f3f4;
        }
        
        .contact-item:hover {
            background-color: #f8f9fa;
            transform: translateX(5px);
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
        
        .icon {
            width: 44px;
            height: 44px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 18px;
            flex-shrink: 0;
        }
        
        .email .icon { background: #d44638; }
        .phone .icon { background: #34a853; }
        .whatsapp .icon { background: #25d366; }
        .linkedin .icon { background: #0077b5; }
        .location .icon { background: #9b59b6; }
        
        .contact-text {
            flex: 1;
        }
        
        .label {
            font-size: 12px;
            color: #7f8c8d;
            margin-bottom: 4px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .value {
            font-size: 15px;
            color: #2c3e50;
            font-weight: 500;
        }
        
        .action-buttons {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
        }
        
        .btn {
            flex: 1;
            min-width: 140px;
            padding: 14px 20px;
            border: none;
            border-radius: 12px;
            font-size: 15px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            text-decoration: none;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #c1440e, #e55d17);
            color: white;
        }
        
        .btn-primary:hover {
            background: linear-gradient(135deg, #a8380c, #c44f13);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(193,68,14,0.3);
        }
        
        .btn-secondary {
            background: #ecf0f1;
            color: #2c3e50;
            border: 2px solid #bdc3c7;
        }
        
        .btn-secondary:hover {
            background: #bdc3c7;
            transform: translateY(-2px);
        }
        
        .company-badge {
            background: linear-gradient(135deg, #ffd700, #ffed4e);
            color: #2c3e50;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-top: 10px;
            box-shadow: 0 2px 8px rgba(255,215,0,0.3);
        }
        
        @media (max-width: 480px) {
            .business-card { margin: 10px; }
            .card-body { padding: 25px 20px; }
            .btn { min-width: 100%; }
            .name { font-size: 22px; }
            .title { font-size: 16px; }
        }
    </style>
</head>
<body>
    <div class="business-card">
        <div class="card-header">
            <div class="profile-img">
                <i class="fas fa-home"></i>
            </div>
            <div class="name">Bernabas Bmatric</div>
            <div class="title">Real Estate Agent</div>
            <div class="company">Apollo Properties</div>
            <div class="company-badge">Your Trusted Real Estate Partner</div>
        </div>
        
        <div class="card-body">
            <div class="contact-info">
                <div class="contact-item email">
                    <div class="icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <div class="contact-text">
                        <div class="label">EMAIL</div>
                        <div class="value">barnymatric92@gmail.com</div>
                    </div>
                </div>
                
                <div class="contact-item phone">
                    <div class="icon">
                        <i class="fas fa-phone"></i>
                    </div>
                    <div class="contact-text">
                        <div class="label">PHONE</div>
                        <div class="value">+1 (571) 702-4087</div>
                    </div>
                </div>
                
                <div class="contact-item whatsapp">
                    <div class="icon">
                        <i class="fab fa-whatsapp"></i>
                    </div>
                    <div class="contact-text">
                        <div class="label">WHATSAPP</div>
                        <div class="value">+1 (571) 702-4087</div>
                    </div>
                </div>
                
                <div class="contact-item linkedin">
                    <div class="icon">
                        <i class="fab fa-linkedin-in"></i>
                    </div>
                    <div class="contact-text">
                        <div class="label">LINKEDIN</div>
                        <div class="value">Bernabas Andualem</div>
                    </div>
                </div>
                
                <div class="contact-item location">
                    <div class="icon">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <div class="contact-text">
                        <div class="label">LOCATION</div>
                        <div class="value">United States</div>
                    </div>
                </div>
            </div>
            
            <div class="action-buttons">
                <a href="#" class="btn btn-primary" id="saveContact">
                    <i class="fas fa-save"></i> Save Contact
                </a>
                <a href="#" class="btn btn-secondary" id="shareCard">
                    <i class="fas fa-share-alt"></i> Share Card
                </a>
            </div>
        </div>
    </div>

    <script>
        // Contact item click handlers
        document.querySelector('.email').addEventListener('click', function() {
            window.location.href = 'mailto:barnymatric92@gmail.com';
        });

        document.querySelector('.phone').addEventListener('click', function() {
            window.location.href = 'tel:+15717024087';
        });

        document.querySelector('.whatsapp').addEventListener('click', function() {
            window.open('https://wa.me/15717024087', '_blank');
        });

        document.querySelector('.linkedin').addEventListener('click', function() {
            window.open('https://www.linkedin.com/in/bernabs-andualem-34aa57367', '_blank');
        });

        // Save Contact as vCard
        document.getElementById('saveContact').addEventListener('click', function(e) {
            e.preventDefault();
            
            const vCardData = `BEGIN:VCARD
VERSION:3.0
FN:Bernabas Bmatric
ORG:Apollo Properties
TITLE:Real Estate Agent
TEL:+15717024087
EMAIL:barnymatric92@gmail.com
URL:https://www.linkedin.com/in/bernabs-andualem-34aa57367
NOTE:Your Trusted Real Estate Partner
ADR:;;;United States;;;
END:VCARD`;

            const blob = new Blob([vCardData], { type: 'text/vcard' });
            const url = window.URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.style.display = 'none';
            a.href = url;
            a.download = 'bernabas-bmatric.vcf';
            document.body.appendChild(a);
            a.click();
            window.URL.revokeObjectURL(url);
            document.body.removeChild(a);
        });

        // Share functionality
        document.getElementById('shareCard').addEventListener('click', function(e) {
            e.preventDefault();
            
            if (navigator.share) {
                navigator.share({
                    title: 'Bernabas Bmatric - Real Estate Agent',
                    text: 'Real Estate Agent at Apollo Properties - Your Trusted Real Estate Partner',
                    url: window.location.href
                });
            } else if (navigator.clipboard) {
                navigator.clipboard.writeText(window.location.href).then(function() {
                    alert('Card link copied to clipboard! Share it with your contacts.');
                });
            } else {
                prompt('Copy this link to share:', window.location.href);
            }
        });

        // Animation on load
        document.addEventListener('DOMContentLoaded', function() {
            const card = document.querySelector('.business-card');
            card.style.opacity = '0';
            card.style.transform = 'translateY(20px)';
            
            setTimeout(() => {
                card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                card.style.opacity = '1';
                card.style.transform = 'translateY(0)';
            }, 100);
        });
    </script>
</body>
</html>
