# Aysha-Beauty-Parlour
<!DOCTYPE html><html lang="bn">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Aysha Beauty Parlor</title>
  <style>
    body { margin:0; font-family: Arial, sans-serif; display:flex; }
    nav { background:#e91e63; width:220px; min-height:100vh; color:white; display:flex; flex-direction:column; padding-top:20px; }
    nav a { color:white; padding:15px 20px; text-decoration:none; font-weight:bold; border-bottom:1px solid #d81b60; cursor:pointer; }
    nav a:hover { background:#d81b60; }
    main { flex:1; padding:20px; }
    section { display:none; }
    section.active { display:block; }
    h2 { color:#e91e63; }
    input, select, textarea { width:100%; padding:10px; margin:5px 0 15px; border-radius:5px; border:1px solid #ccc; }
    button { background:#e91e63; color:white; border:none; padding:10px 20px; border-radius:5px; cursor:pointer; }
    .service-item { margin-bottom:15px; border-bottom:1px dashed #e91e63; padding-bottom:10px; }
  </style>
</head>
<body><nav>
  <a onclick="showSection('home')">Home</a>
  <a onclick="showSection('services')">Services</a>
  <a onclick="showSection('contact')">Contact</a>
  <a onclick="showSection('support')">Support</a>
</nav><main>
  <section id="home" class="active">
    <h2>Aysha Beauty Parlor</h2>
    <p>আপনার সৌন্দর্য, আমাদের পেশাদার যত্নে</p>
    <h3>Advance Booking</h3>
    <form>
      <label>নাম</label>
      <input type="text" name="name" required>
      <label>ঠিকানা</label>
      <input type="text" name="address" required>
      <label>উপজেলা</label>
      <input type="text" name="upazila" required>
      <label>জেলা</label>
      <input type="text" name="district" required>
      <label>মোবাইল নাম্বার</label>
      <input type="text" name="mobile" required>
      <label>সার্ভিস নির্বাচন</label>
      <select name="service">
        <option>Facial & Skin Care</option>
        <option>Bridal Makeover</option>
        <option>Hair Cut & Styling</option>
        <option>Manicure & Pedicure</option>
        <option>Party Makeover</option>
      </select>
      <label>তারিখ</label>
      <input type="date" name="date" required>
      <label>সময়</label>
      <input type="time" name="time" required>
      <button type="submit">বুকিং করুন</button>
    </form>
  </section>  <section id="services">
    <h2>আমাদের সেবাসমূহ</h2>
    <div class="service-item"><strong>Facial & Skin Care</strong><br>শুরু মূল্য: ৮০০ টাকা</div>
    <div class="service-item"><strong>Bridal Makeover</strong><br>শুরু মূল্য: ৫,০০০ টাকা</div>
    <div class="service-item"><strong>Hair Cut & Styling</strong><br>শুরু মূল্য: ৩০০ টাকা</div>
    <div class="service-item"><strong>Manicure & Pedicure</strong><br>শুরু মূল্য: ৬০০ টাকা</div>
    <div class="service-item"><strong>Party Makeover</strong><br>শুরু মূল্য: ৪,০০০ টাকা</div>
  </section>  <section id="contact">
    <h2>যোগাযোগ</h2>
    <p>📍 ঠিকানা: কালুরমোড়, ফকিরপাড়া রোড, সদর, দিনাজপুর</p>
    <p>📞 ফোন: +8801739771064</p>
    <p>💬 <a href="https://wa.me/8801739771064" target="_blank">WhatsApp করুন</a></p>
  </section>  <section id="support">
    <h2>Support Form</h2>
    <form>
      <label>নাম</label>
      <input type="text" name="name" required>
      <label>ইমেইল</label>
      <input type="email" name="email" required>
      <label>বিস্তারিত অভিযোগ</label>
      <textarea name="message" rows="5" required></textarea>
      <button type="submit">পাঠান</button>
    </form>
  </section>
</main><script>
  function showSection(id){
    document.querySelectorAll('main section').forEach(s => s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
  }
</script></body>
</html>
