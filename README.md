<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Warriors Defence Academy | Best NDA & CDS Coaching</title>
    <style>
        /* Modern CSS Variables */
        :root {
            --primary-blue: #0f172a;
            --secondary-blue: #1d4ed8;
            --accent-orange: #ea580c;
            --light-bg: #f8fafc;
            --white: #ffffff;
            --text-dark: #1e293b;
            --text-gray: #64748b;
        }

        body { 
            font-family: 'Inter', system-ui, -apple-system, sans-serif; 
            margin: 0; 
            padding: 0; 
            background-color: var(--light-bg); 
            color: var(--text-dark);
            overflow-x: hidden;
        }

        /* Navratri & Diwali Offer Bar */
        .offer-bar {
            background: linear-gradient(90deg, #d97706, #ea580c, #dc2626);
            color: white;
            text-align: center;
            padding: 12px;
            font-size: 14px;
            font-weight: 700;
            letter-spacing: 0.5px;
            animation: pulse 2s infinite;
        }
        .offer-bar span { color: #fde047; font-weight: 900; }
        @keyframes pulse { 0% { opacity: 1; } 50% { opacity: 0.85; } 100% { opacity: 1; } }

        /* Top Bar */
        .top-bar { background-color: var(--primary-blue); color: #cbd5e1; padding: 10px 20px; display: flex; justify-content: space-between; font-size: 13px; }
        .top-bar a { color: #fbbf24; text-decoration: none; font-weight: bold; font-size: 15px; }

        /* Header */
        .header { background-color: var(--white); padding: 15px 20px; display: flex; align-items: center; justify-content: center; gap: 20px; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); position: sticky; top: 0; z-index: 100; }
        .header img { width: 80px; height: 80px; border-radius: 50%; border: 3px solid var(--accent-orange); object-fit: cover; }
        .header-text h1 { margin: 0; font-size: 26px; color: var(--primary-blue); text-transform: uppercase; font-weight: 900; }
        .header-text p { margin: 2px 0 0 0; font-size: 14px; color: var(--text-gray); font-weight: 600; }

        /* Hero Section */
        .hero { background: linear-gradient(rgba(15, 23, 42, 0.85), rgba(15, 23, 42, 0.85)), url('main-photo.jpg') center/cover; color: white; text-align: center; padding: 70px 20px; }
        .hero h2 { font-size: 38px; margin-bottom: 15px; font-weight: 900; line-height: 1.2; }
        .hero h2 span { color: #fbbf24; }
        .hero p { font-size: 18px; max-width: 700px; margin: 0 auto 30px auto; color: #e2e8f0; line-height: 1.6; }
        .btn-primary { background: var(--accent-orange); color: white; padding: 15px 35px; font-size: 18px; font-weight: bold; border-radius: 8px; text-decoration: none; display: inline-block; transition: 0.3s; border: none; cursor: pointer; box-shadow: 0 10px 15px -3px rgba(234, 88, 12, 0.4); }
        .btn-primary:hover { background: #c2410c; transform: translateY(-3px); }

        /* 20,000+ Selections Milestone */
        .milestone-section { background: linear-gradient(135deg, #065f46, #047857); color: white; padding: 30px 20px; text-align: center; box-shadow: 0 10px 15px -3px rgba(0,0,0,0.2); }
        .milestone-section h2 { margin: 0; font-size: 48px; font-weight: 900; color: #fef08a; text-shadow: 2px 2px 4px rgba(0,0,0,0.3); }
        .milestone-section p { margin: 10px 0 0 0; font-size: 20px; font-weight: 600; text-transform: uppercase; letter-spacing: 1px; }

        /* Container */
        .container { max-width: 1050px; margin: 0 auto; padding: 0 20px 50px 20px; }
        .section-title { text-align: center; color: var(--primary-blue); margin: 50px 0 35px 0; font-size: 30px; font-weight: 900; text-transform: uppercase; }
        .section-title::after { content: ''; display: block; width: 70px; height: 5px; background: var(--accent-orange); margin: 12px auto 0 auto; border-radius: 3px; }

        /* BATCES SECTION (New Detailed Design) */
        .batch-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 25px; }
        .batch-card { background: white; border-radius: 12px; padding: 25px; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); border-top: 5px solid var(--secondary-blue); transition: 0.3s; position: relative; }
        .batch-card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15); }
        .batch-card h3 { color: var(--primary-blue); font-size: 22px; margin: 0 0 8px 0; font-weight: 800; }
        .batch-card .batch-desc { color: var(--text-gray); margin-bottom: 15px; line-height: 1.5; font-size: 14px; }
        
        /* Faculty Assignment Box inside Batch */
        .batch-faculty { background: #f1f5f9; padding: 15px; border-radius: 8px; margin-bottom: 18px; border-left: 4px solid #fbbf24; font-size: 13.5px; line-height: 1.6; color: #334155; }
        .batch-faculty strong { color: var(--primary-blue); font-size: 14px; }
        .batch-faculty .commander { color: #b91c1c; font-weight: bold; margin-bottom: 5px; display: block; }
        .batch-faculty .teachers { display: block; margin-top: 5px; }

        /* Price Box */
        .price-box { background: #fff7ed; border: 1px dashed #fdba74; padding: 15px; border-radius: 8px; margin-bottom: 20px; text-align: center; }
        .price-box .coupon { display: inline-block; background: #22c55e; color: white; padding: 4px 12px; border-radius: 20px; font-size: 12px; font-weight: bold; margin-bottom: 8px; animation: pulse 2s infinite; }
        .price-box .old-price { text-decoration: line-through; color: #94a3b8; font-size: 15px; display: block; }
        .price-box .new-price { color: #b91c1c; font-size: 28px; font-weight: 900; display: block; margin-top: 5px; }
        
        .btn-secondary { background: var(--secondary-blue); color: white; border: none; padding: 14px; width: 100%; font-size: 16px; font-weight: bold; border-radius: 6px; cursor: pointer; transition: 0.3s; }
        .btn-secondary:hover { background: #1e3a8a; }

        /* Media Section & Footer (Compact for CSS) */
        .media-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; }
        .media-card { background: white; padding: 12px; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
        .media-card img, .media-card video { width: 100%; height: 220px; object-fit: cover; border-radius: 8px; }
        .media-card p { text-align: center; font-weight: 700; color: var(--primary-blue); margin: 12px 0 5px 0; font-size: 16px; }
        
        .whatsapp-float { position: fixed; width: 60px; height: 60px; bottom: 30px; right: 30px; background-color: #25d366; color: #FFF; border-radius: 50px; text-align: center; font-size: 35px; box-shadow: 2px 2px 10px rgba(0,0,0,0.2); z-index: 1000; display: flex; align-items: center; justify-content: center; text-decoration: none; animation: bounce 2s infinite; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }

        .footer { background: #020617; color: #94a3b8; padding: 40px 20px 20px 20px; text-align: center; font-size: 15px; margin-top: 40px; }
        .footer span { color: white; font-weight: bold; }
    </style>
</head>
<body>

    <div class="offer-bar">
        🌸 NAVRATRI MAHA-OFFER: Flat 70% OFF on Live Batches! <span>(🎁 Mega Diwali Surprise Coming Soon...)</span> 🌸
    </div>

    <div class="top-bar">
        <div>📍 Location: Kapoor Thala, Lucknow, UP</div>
        <div>📞 Admission Helpline: <a href="tel:881790961">881790961</a> (Tap to call)</div>
    </div>
    
    <div class="header">
        <img src="1000020835.jpg" alt="Warriors Defence Academy Logo">
        <div class="header-text">
            <h1>Warriors Defence Academy</h1>
            <p>Director: Gulab Singh | India's Premier Defence Institute</p>
        </div>
    </div>
    
    <div class="hero">
        <h2>Achieve Your Defence Dreams With <span>India's Best</span></h2>
        <p>Prepare with top defence experts, ex-SSB panelists, and rigorous physical training.</p>
        <a href="#batches" class="btn-primary">Explore Live Batches</a>
    </div>

    <div class="milestone-section">
        <h2>20,000+</h2>
        <p>Proud Selections in NDA & CDS across India</p>
    </div>
    
    <div class="container">
        
        <h2 class="section-title" id="batches">🔥 Our Live Batches (Navratri Offer)</h2>
        <div class="batch-grid">
            
            <!-- Class 11 Foundation Batch -->
            <div class="batch-card">
                <h3>Foundation Batch (Class 11)</h3>
                <p class="batch-desc">Complete base building and NDA preparation for 11th studying students.</p>
                
                <div class="batch-faculty">
                    <span class="commander">🎖️ Batch Commander: Dr. Natrajan</span>
                    <span class="teachers"><strong>📚 Key Faculty:</strong> Neeraj Bainsla Sir (Maths), Reshma Khan Mam (Science), Anuj Chouhan Sir (English)</span>
                </div>

                <div class="price-box">
                    <span class="coupon">NAVRATRI70 Applied (70% OFF)</span>
                    <span class="old-price">Base Fee: ₹5,000</span>
                    <span class="new-price">₹1,500</span>
                </div>
                <button class="btn-secondary">Enroll Now</button>
            </div>

            <!-- NDA Batch -->
            <div class="batch-card">
                <h3>NDA Target Batch</h3>
                <p class="batch-desc">Strictly focused and comprehensive course for National Defence Academy.</p>
                
                <div class="batch-faculty">
                    <span class="commander">🎖️ Batch Commander: Cdr. Vikram Yadav</span>
                    <span class="teachers"><strong>📚 Key Faculty:</strong> Arpit Choudhary Sir (Maths), Sanjeev Thakur Sir (English), Shyam Sharma Sir (Science)</span>
                </div>

                <div class="price-box">
                    <span class="coupon">NAVRATRI70 Applied (70% OFF)</span>
                    <span class="old-price">Base Fee: ₹9,333</span>
                    <span class="new-price">₹2,800</span>
                </div>
                <button class="btn-secondary">Enroll Now</button>
            </div>

            <!-- CDS Batch -->
            <div class="batch-card">
                <h3>CDS Target Batch</h3>
                <p class="batch-desc">Advanced preparation and tactical syllabus coverage for CDS Examination.</p>
                
                <div class="batch-faculty">
                    <span class="commander">🎖️ Batch Commander: Cdr. Rajveer Ranjan</span>
                    <span class="teachers"><strong>📚 Key Faculty:</strong> Sandeep Sir (CDS Maths), Khan Sir (GS), Anuj Chouhan Sir (English)</span>
                </div>

                <div class="price-box">
                    <span class="coupon">NAVRATRI70 Applied (70% OFF)</span>
                    <span class="old-price">Base Fee: ₹10,666</span>
                    <span class="new-price">₹3,200</span>
                </div>
                <button class="btn-secondary">Enroll Now</button>
            </div>

            <!-- AFCAT Batch -->
            <div class="batch-card">
                <h3>AFCAT Special Batch</h3>
                <p class="batch-desc">Air Force Common Admission Test complete syllabus and mock tests.</p>
                
                <div class="batch-faculty">
                    <span class="commander">🎖️ Batch Commander: K.P. Thakur</span>
                    <span class="teachers"><strong>📚 Key Faculty:</strong> Sumit Kumar Sir (GS), Neha Mam (Science), Sanjeev Thakur Sir (English)</span>
                </div>

                <div class="price-box">
                    <span class="coupon">NAVRATRI70 Applied (70% OFF)</span>
                    <span class="old-price">Base Fee: ₹14,000</span>
                    <span class="new-price">₹4,200</span>
                </div>
                <button class="btn-secondary">Enroll Now</button>
            </div>

        </div>

        <h2 class="section-title">Academy Glimpses & Training</h2>
        <div class="media-grid">
            <div class="media-card">
                <img src="ground.jpg" alt="Ground Training">
                <p>Rigorous Ground Training</p>
            </div>
            <div class="media-card">
                <img src="ssb-panel.jpg" alt="Live SSB Session">
                <p>Live SSB Interview Prep</p>
            </div>
            <div class="media-card">
                <video controls>
                    <source src="training-video.mp4" type="video/mp4">
                </video>
                <p>Watch Our Training Action</p>
            </div>
        </div>

    </div>

    <div class="footer">
        <p>&copy; 2027 <span>Warriors Defence Academy</span>, Lucknow. All Rights Reserved. | Designed for 2027-2028 Sessions.</p>
    </div>

    <a href="https://wa.me/91881790961" class="whatsapp-float" target="_blank" title="Chat with us on WhatsApp">
        💬
    </a>

</body>
</html>
