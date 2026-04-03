<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Life Care Personal Support Services</title>  
    <style>  
        body { font-family: Arial, sans-serif; margin:0; padding:0; background:#f9f9f9; line-height:1.6; }  
        header { background:#4CAF50; color:white; padding:20px 0; text-align:center; }  
        nav { text-align:center; background:#333; }  
        nav a { color:white; padding:14px 20px; display:inline-block; text-decoration:none; }  
        nav a:hover { background:#575757; }  
        section { padding:20px; max-width:1000px; margin:auto; }  
        h2 { color:#333; }  
        .services { display:flex; flex-wrap:wrap; gap:20px; }  
        .service-box { flex:1 1 45%; background:white; padding:20px; border-radius:5px; box-shadow:0 0 5px rgba(0,0,0,0.1); }  
        footer { background:#333; color:white; text-align:center; padding:10px 0; margin-top:20px; }  
        form input, form textarea { width:100%; padding:10px; margin-bottom:10px; }  
        form button { padding:10px 20px; background-color:#4CAF50; color:white; border:none; cursor:pointer; }  
        form button:hover { background-color:#45a049; }  
        .call-button { display:inline-block; margin-top:10px; padding:12px 25px; background:#ff6600; color:white; text-decoration:none; border-radius:5px; }  
        .call-button:hover { background:#e65c00; }  
        #map { width:100%; height:400px; margin-top:20px; border-radius:5px; }  
    </style>  
</head>  
<body>  
  
<header>  
    <h1>Life Care Personal Support Services</h1>  
    <p>Compassionate Home Care in Lewiston & Auburn, ME</p>  
    <a class="call-button" href="tel:+1207XXXXXXX">Call Now</a>  
</header>  
  
<nav>  
    <a href="#home">Home</a>  
    <a href="#about">About Us</a>  
    <a href="#services">Services</a>  
    <a href="#contact">Contact</a>  
</nav>  
  
<section id="home">  
    <h2>Welcome</h2>  
    <p>Life Care Personal Support Services provides compassionate, reliable home care in Lewiston and Auburn, ME. Our trained caregivers offer personal care, companionship, and flexible support to meet your loved one’s needs.</p>  
    <p><strong>Call us today: (207) XXX-XXXX</strong></p>  
</section>  
  
<section id="about">  
    <h2>About Us</h2>  
    <p>At Life Care Personal Support Services, our mission is to provide personalized, high-quality care that helps our clients live safely and comfortably at home. Our caregivers are trained, dependable, and dedicated to treating every client with respect and compassion.</p>  
</section>  
  
<section id="services">  
    <h2>Our Services</h2>  
    <div class="services">  
        <div class="service-box">  
            <h3>Personal Care</h3>  
            <p>Bathing, dressing, grooming, toileting assistance, and mobility support.</p>  
        </div>  
        <div class="service-box">  
            <h3>Companionship</h3>  
            <p>Friendly interaction, conversation, and emotional support.</p>  
        </div>  
        <div class="service-box">  
            <h3>Meal Preparation & Medication</h3>  
            <p>Preparing meals and reminding clients to take medications on time.</p>  
        </div>  
        <div class="service-box">  
            <h3>Light Housekeeping & Transportation</h3>  
            <p>Cleaning, laundry, errands, and transportation to appointments.</p>  
        </div>  
    </div>  
</section>  
  
<section id="contact">  
    <h2>Contact Us</h2>  
    <p>Email us at <a href="mailto:suglmohamed9@gmail.com">suglmohamed9@gmail.com</a> or <a href="mailto:moulimidriss@gmail.com">moulimidriss@gmail.com</a></p>  
    <form id="contactForm">  
        <input type="text" name="name" placeholder="Your Name" required>  
        <input type="email" name="email" placeholder="Your Email" required>  
        <input type="text" name="phone" placeholder="Phone Number">  
        <textarea name="message" placeholder="How can we help you?" rows="5" required></textarea>  
        <button type="submit">Send Message</button>  
    </form>  
    <p id="formMessage" style="color:green;"></p>  
    <div id="map"></div>  
</section>  
  
<footer>  
    <p>&copy; 2026 Life Care Personal Support Services. All Rights Reserved.</p>  
</footer>  
  
<script>  
    // Contact form functionality using mailto  
    const form = document.getElementById('contactForm');  
    form.addEventListener('submit', function(e) {  
        e.preventDefault();  
        const name = form.name.value;  
        const email = form.email.value;  
        const phone = form.phone.value;  
        const message = form.message.value;  
        const subject = encodeURIComponent("New Client Inquiry from Website");  
        const body = encodeURIComponent(`Name: ${name}\nEmail: ${email}\nPhone: ${phone}\nMessage: ${message}`);  
        window.location.href = `mailto:suglmohamed9@gmail.com?cc=moulimidriss@gmail.com&subject=${subject}&body=${body}`;  
        document.getElementById('formMessage').innerText = "Your message is ready to send! Check your email client.";  
        form.reset();  
    });  
  
    // Google Maps Embed  
    function initMap() {  
        const lewiston = { lat: 44.1004, lng: -70.2148 }; // Lewiston, ME  
        const map = new google.maps.Map(document.getElementById("map"), {  
            zoom: 12,  
            center: lewiston,  
        });  
        const marker = new google.maps.Marker({  
            position: lewiston,  
            map: map,  
            title: "Life Care Personal Support Services",  
        });  
    }  
</script>  
<script async src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY&callback=initMap"></script>  
  
</body>  
</html>  
