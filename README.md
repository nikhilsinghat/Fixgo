<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>FixGo | Reliable Home Services at Your Doorstep</title>
    <meta name="description" content="FixGo offers trusted home services including electricians, plumbers, cleaners, beauty & wellness, and home repair. Available in Varanasi, Mirzapur, Bhadohi." />
    <meta name="keywords" content="home services, electrician, plumber, cleaning, beauty wellness, home repair, Varanasi, Mirzapur, Bhadohi" />
    <style>
      /* Reset and base styles */
      *, *::before, *::after {
        box-sizing: border-box;
      }
      body {
        margin: 0;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background-color: #f9fafb;
        color: #222;
        line-height: 1.5;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
      }
      a {
        color: inherit;
        text-decoration: none;
      }
      a:focus-visible,
      button:focus-visible,
      input:focus-visible,
      textarea:focus-visible {
        outline: 3px solid #ffdd57;
        outline-offset: 2px;
      }
      /* Header */
      header {
        background: linear-gradient(45deg, #2a6ebb, #0066cc);
        color: white;
        padding: 2rem 1rem;
        text-align: center;
        box-shadow: 0 4px 12px rgb(0 0 0 / 0.1);
      }
      header h1 {
        font-size: 3rem;
        margin-bottom: 0.25rem;
        font-weight: 900;
        letter-spacing: 3px;
      }
      header p {
        font-size: 1.3rem;
        font-weight: 600;
        opacity: 0.9;
      }
      /* Navigation */
      nav {
        background: #005bb5;
        display: flex;
        justify-content: center;
        gap: 2rem;
        padding: 1rem 0;
        box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      }
      nav a {
        color: white;
        font-weight: 600;
        font-size: 1.15rem;
        padding: 0.3rem 0.5rem;
        border-radius: 6px;
        transition: background-color 0.3s ease;
      }
      nav a:hover,
      nav a:focus {
        background-color: #ffdd57;
        color: #003f7f;
        outline-offset: 2px;
      }
      nav a[aria-current="page"] {
        background-color: #ffdd57;
        color: #003f7f;
      }
      /* Main Hero Section */
      main {
        flex-grow: 1;
      }
      .hero {
        background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1350&q=80') center/cover no-repeat;
        color: white;
        text-align: center;
        padding: 6rem 1rem 4rem;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
      }
      .hero::before {
        content: "";
        position: absolute;
        inset: 0;
        background-color: rgba(0, 0, 0, 0.37);
        z-index: 0;
      }
      .hero > * {
        position: relative;
        z-index: 1;
      }
      .hero h2 {
        font-size: 3.6rem;
        font-weight: 900;
        margin-bottom: 1rem;
        max-width: 800px;
        margin-left: auto;
        margin-right: auto;
        text-shadow: 0 3px 8px rgba(0,0,0,0.6);
      }
      .hero p {
        font-weight: 600;
        font-size: 1.6rem;
        max-width: 650px;
        margin: 0 auto 2.5rem;
        text-shadow: 0 2px 7px rgba(0,0,0,0.45);
      }
      .hero button {
        background-color: #ffdd57;
        color: #005bb5;
        font-weight: 700;
        font-size: 1.3rem;
        border: none;
        border-radius: 9999px;
        padding: 0.8rem 3.6rem;
        cursor: pointer;
        box-shadow: 0 7px 14px rgba(255,221,87,0.5);
        transition: background-color 0.3s ease, color 0.3s ease;
        user-select: none;
      }
      .hero button:hover,
      .hero button:focus {
        background-color: #f7c200;
        outline-offset: 3px;
      }

      /* Sections */
      .section {
        max-width: 1100px;
        margin: 2rem auto 4rem;
        padding: 0 1rem;
      }
      .section h2 {
        text-align: center;
        font-size: 2.7rem;
        font-weight: 900;
        color: #005bb5;
        margin-bottom: 2rem;
        letter-spacing: 1.4px;
      }
      .cards-grid {
        display: grid;
        gap: 1.9rem;
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      }
      .card {
        background-color: white;
        border-radius: 14px;
        box-shadow: 0 8px 21px rgba(0,0,0,0.07);
        padding: 1.8rem 1.6rem;
        transition: box-shadow 0.3s ease, transform 0.35s ease;
        cursor: default;
      }
      .card:hover,
      .card:focus-within {
        outline: none;
        box-shadow: 0 14px 30px rgba(0,0,0,0.15);
        transform: translateY(-10px);
      }
      .card h3 {
        color: #0077ff;
        font-weight: 700;
        margin-bottom: 10px;
        font-size: 1.4rem;
      }
      .card p {
        font-weight: 500;
        font-size: 1rem;
        color: #555;
      }

      /* Footer */
      footer {
        text-align: center;
        padding: 2rem 1rem;
        background-color: #005bb5;
        color: white;
        font-weight: 500;
        font-size: 0.95rem;
        box-shadow: 0 -6px 10px rgba(0,0,0,0.12);
      }
      footer p + p {
        margin-top: 0.4rem;
        font-style: italic;
        font-size: 0.9rem;
      }
      footer a {
        color: #ffdd57;
        text-decoration: none;
        font-weight: 600;
      }
      footer a:hover,
      footer a:focus {
        text-decoration: underline;
      }

      /* Modal styles */
      .modal-overlay {
        position: fixed;
        inset: 0;
        background-color: rgba(0,0,0,0.6);
        display: none;
        justify-content: center;
        align-items: center;
        z-index: 10000;
      }
      .modal-overlay.active {
        display: flex;
      }
      .modal {
        background-color: white;
        border-radius: 12px;
        max-width: 400px;
        width: 90%;
        padding: 2rem;
        box-shadow: 0 12px 28px rgb(0 0 0 / 0.2);
        position: relative;
        outline: none;
      }
      .modal h3 {
        margin-top: 0;
        margin-bottom: 1rem;
        font-size: 1.8rem;
        color: #005bb5;
      }
      .modal label {
        display: block;
        margin: 0.7rem 0 0.3rem;
        font-weight: 600;
        font-size: 1rem;
      }
      .modal input[type="text"],
      .modal input[type="email"],
      .modal input[type="tel"],
      .modal select,
      .modal textarea {
        width: 100%;
        padding: 0.4rem 0.6rem;
        font-size: 1rem;
        border: 1.8px solid #ccc;
        border-radius: 8px;
        font-family: inherit;
      }
      .modal textarea {
        resize: vertical;
        min-height: 80px;
      }
      .modal button {
        margin-top: 1.5rem;
        background-color: #005bb5;
        color: white;
        border: none;
        padding: 0.7rem 2.5rem;
        font-size: 1.1rem;
        border-radius: 9999px;
        cursor: pointer;
        font-weight: 700;
        transition: background-color 0.3s ease;
      }
      .modal button:hover,
      .modal button:focus {
        background-color: #003f7f;
        outline-offset: 2px;
      }
      .modal .close-btn {
        position: absolute;
        top: 15px;
        right: 20px;
        background: none;
        border: none;
        font-size: 1.6rem;
        cursor: pointer;
        color: #333;
      }
      .modal .close-btn:hover,
      .modal .close-btn:focus {
        color: #005bb5;
        outline-offset: 2px;
      }

      /* Responsive */
      @media (max-width: 768px) {
        header h1 {
          font-size: 2.4rem;
        }
        nav {
          gap: 1rem;
        }
        .hero h2 {
          font-size: 2.6rem;
        }
        .hero p {
          font-size: 1.3rem;
          max-width: 90%;
        }
        .section h2 {
          font-size: 2rem;
        }
        .cards-grid {
          grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        }
      }
      @media (max-width: 400px) {
        .hero h2 {
          font-size: 1.8rem;
        }
        .hero p {
          font-size: 1rem;
        }
        .hero button {
          width: 100%;
          max-width: 280px;
        }
      }
    </style>
  </head>
  <body>
    <header>
      <h1>FixGo</h1>
      <p>Your Trusted Partner for Reliable Home Services</p>
    </header>

    <nav aria-label="Primary navigation">
      <a href="#" aria-current="page">Home</a>
      <a href="#services-section">Services</a>
      <a href="#cities-section">Cities</a>
      <a href="#contact-section">Contact</a>
    </nav>

    <main>
      <section class="hero" role="banner" aria-label="Promotional introduction">
        <h2>Your Trusted Partner for Home Services</h2>
        <p>Electricians, Plumbers, Cleaners, and More – Just a Click Away</p>
        <button id="bookNowBtn" type="button" aria-haspopup="dialog" aria-controls="bookingModal" aria-expanded="false">Book Now</button>
      </section>

      <section id="services-section" class="section" aria-labelledby="servicesHeading">
        <h2 id="servicesHeading">Our Services</h2>
        <div class="cards-grid">
          <article class="card" tabindex="0" aria-labelledby="serviceElectrician">
            <h3 id="serviceElectrician">Electrician</h3>
            <p>Quick and reliable electrical solutions to keep your home powered safely.</p>
          </article>
          <article class="card" tabindex="0" aria-labelledby="servicePlumber">
            <h3 id="servicePlumber">Plumber</h3>
            <p>Expert plumbing services for installations, repairs, and maintenance.</p>
          </article>
          <article class="card" tabindex="0" aria-labelledby="serviceBeauty">
            <h3 id="serviceBeauty">Beauty &amp; Wellness</h3>
            <p>Convenient salon and wellness treatments in the comfort of your home.</p>
          </article>
          <article class="card" tabindex="0" aria-labelledby="serviceRepair">
            <h3 id="serviceRepair">Home Repair</h3>
            <p>From small fixes to major repairs, we help you maintain your home.</p>
          </article>
          <article class="card" tabindex="0" aria-labelledby="serviceCleaning">
            <h3 id="serviceCleaning">Cleaning</h3>
            <p>Comprehensive cleaning and disinfection to keep your home fresh and safe.</p>
          </article>
        </div>
      </section>

      <section id="cities-section" class="section" aria-labelledby="citiesHeading">
        <h2 id="citiesHeading">Currently Available In</h2>
        <div class="cards-grid">
          <article class="card" tabindex="0" aria-labelledby="cityVaranasi">
            <h3 id="cityVaranasi">Varanasi</h3>
          </article>
          <article class="card" tabindex="0" aria-labelledby="cityMirzapur">
            <h3 id="cityMirzapur">Mirzapur</h3>
          </article>
          <article class="card" tabindex="0" aria-labelledby="cityBhadohi">
            <h3 id="cityBhadohi">Bhadohi</h3>
          </article>
        </div>
      </section>

      <section id="contact-section" class="section" aria-labelledby="contactHeading">
        <h2 id="contactHeading">Contact Us</h2>
        <p style="text-align:center; max-width:600px; margin: 0 auto 1rem;">
          Need assistance? Reach out to our support team for queries or booking help.
        </p>
        <p style="text-align:center; margin-bottom: 3rem;">
          Email: <a href="mailto:support itsashish0001@gmail.com.in" style="color:#005bb5; font-weight:600;">support@fixgo.in</a> | Phone: <a href="tel:+918303948098" style="color:#005bb5; font-weight:600;">+91 12345 67890</a>
        </p>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 FixGo. All rights reserved.</p>
      <p>Contact us anytime at <a href="mailto:support itsashish0001@gmail.com">support@fixgo.in</a></p>
    </footer>

    <!-- Booking Modal -->
    <div class="modal-overlay" id="bookingModal" role="dialog" aria-modal="true" aria-labelledby="bookingModalTitle" aria-describedby="bookingModalDesc" tabindex="-1">
      <div class="modal" role="document">
        <button class="close-btn" aria-label="Close booking form" id="closeModalBtn">&times;</button>
        <h3 id="bookingModalTitle">Book a Service</h3>
        <p id="bookingModalDesc">Please fill in your details below to request a service. We will get back to you shortly.</p>
        <form id="bookingForm">
          <label for="fullName">Full Name</label>
          <input type="text" id="fullName" name="fullName" required autocomplete="name" placeholder="Your full name" />

          <label for="email">Email Address</label>
          <input type="email" id="email" name="email" required autocomplete="email" placeholder="you@example.com" />

          <label for="phone">Phone Number</label>
          <input type="tel" id="phone" name="phone" required autocomplete="tel" placeholder="+91 12345 67890" pattern="^\+?\d{7,15}$" />

          <label for="serviceSelect">Service Needed</label>
          <select id="serviceSelect" name="serviceSelect" required>
            <option value="" disabled selected>Select a service</option>
            <option value="Electrician">Electrician</option>
            <option value="Plumber">Plumber</option>
            <option value="Beauty & Wellness">Beauty &amp; Wellness</option>
            <option value="Home Repair">Home Repair</option>
            <option value="Cleaning">Cleaning</option>
          </select>

          <label for="address">Service Address</label>
          <textarea id="address" name="address" required placeholder="Enter your address"></textarea>

          <button type="submit">Submit Booking</button>
        </form>
      </div>
    </div>

    <script>
      // Modal elements
      const bookNowBtn = document.getElementById('bookNowBtn');
      const bookingModal = document.getElementById('bookingModal');
      const closeModalBtn = document.getElementById('closeModalBtn');
      const bookingForm = document.getElementById('bookingForm');

      // Trap focus in modal for accessibility
      let focusableElementsString = 'a[href], area[href], input:not([disabled]), select:not([disabled]), textarea:not([disabled]), button:not([disabled]), [tabindex="0"]';
      let firstFocusableElement = null;
      let lastFocusableElement = null;

      function trapFocus(element) {
        const focusableElements = element.querySelectorAll(focusableElementsString);
        if (focusableElements.length > 0) {
          firstFocusableElement = focusableElements[0];
          lastFocusableElement = focusableElements[focusableElements.length -1];
          firstFocusableElement.focus();

          function handleTrap(e) {
            if (e.key === 'Tab' || e.keyCode === 9) {
              if ( e.shiftKey ) /* shift + tab */ {
                if (document.activeElement === firstFocusableElement) {
                  e.preventDefault();
                  lastFocusableElement.focus();
                }
              } else /* tab */ {
                if (document.activeElement === lastFocusableElement) {
                  e.preventDefault();
                  firstFocusableElement.focus();
                }
              }
            }
            if (e.key === 'Escape' || e.key === 'Esc') {
              closeModal();
            }
          }
          element.addEventListener('keydown', handleTrap);
          // Remove listener on modal close to avoiding duplicate binds
          element.dataset.trapListener = true;
        }
      }

      function openModal() {
        bookingModal.classList.add('active');
        bookNowBtn.setAttribute('aria-expanded', 'true');
        trapFocus(bookingModal);
      }

      function closeModal() {
        bookingModal.classList.remove('active');
        bookNowBtn.setAttribute('aria-expanded', 'false');
        bookNowBtn.focus();
      }

      bookNowBtn.addEventListener('click', () => {
        openModal();
      });

      closeModalBtn.addEventListener('click', () => {
        closeModal();
      });

      // Close modal on overlay click but not when clicking inside modal content
      bookingModal.addEventListener('click', e => {
        if (e.target === bookingModal) {
          closeModal();
        }
      });

      // Handle form submission
      bookingForm.addEventListener('submit', (event) => {
        event.preventDefault();

        // Validate form manually (some browsers might not validate pattern)
        const phone = bookingForm.phone.value.trim();
        const phonePattern = /^\+?\d{7,15}$/;
        if (!phonePattern.test(phone)) {
          alert('Please enter a valid phone number including country code, digits only.');
          bookingForm.phone.focus();
          return;
        }

        // Simulate form submission success
        alert('Thank you for booking with FixGo! We will contact you soon.');

        bookingForm.reset();
        closeModal();
      });

      // Close modal on Escape key globally
      document.addEventListener('keydown', (e) => {
        if ((e.key === 'Escape' || e.key === 'Esc') && bookingModal.classList.contains('active')) {
          closeModal();
        }
      });
    </script>
  </body>
</html>
