# Gaming_protofile
<!-- Header and Navigation -->
<header>
    <h1>Gaming Professional Portfolio</h1>
    <nav>
        <a href="#" onclick="showSection('profile')">Profile</a>
        <a href="#" onclick="showSection('achievements')">Achievements</a>
        <a href="#" onclick="showSection('contact')">Contact</a>
    </nav>
</header>

<!-- Main Content -->
<main id="content">
    <!-- Profile Section -->
    <section id="profile" class="profile-section">
        <h2>About Me</h2>
        <div class="profile-info">
            <img src="https://via.placeholder.com/200" alt="Profile Image">
            <div>
                <p>Hello! I am a professional gamer with over 10 years of experience in competitive gaming. I specialize in first-person shooters and have participated in international tournaments. My journey started with small local competitions, and over the years, I have become a seasoned expert in various gaming genres.</p>
                <p>From strategy games to fast-paced shooters, gaming has been my passion. Here, I showcase my journey, achievements, and how to get in touch with me.</p>
            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" class="achievements-section" style="display:none;">
        <h2>Achievements</h2>
        <div class="achievements-list">
            <div class="achievement-item">
                <h3>1st Place - Global FPS Tournament</h3>
                <p>Won first place in the 2022 Global FPS Tournament with a team of skilled players. Over 100 teams participated in the competition.</p>
            </div>
            <div class="achievement-item">
                <h3>2nd Place - Strategy Masters 2023</h3>
                <p>A runner-up position in the 2023 Strategy Masters Championship, showcasing superior team coordination and critical thinking.</p>
            </div>
            <div class="achievement-item">
                <h3>MVP Award - XYZ Gaming League</h3>
                <p>Awarded Most Valuable Player in the XYZ Gaming League for outstanding performance in 10 consecutive matches.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section" style="display:none;">
        <h2>Contact Me</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="5" required></textarea>

            <button type="submit">Submit</button>
        </form>
    </section>
</main>

<!-- Footer -->
<footer>
    <p>© 2024 Gaming Professional. All Rights Reserved.</p>
</footer>

<script>
    // JavaScript: Section Navigation
    function showSection(sectionId) {
        const sections = document.querySelectorAll('main > section');
        sections.forEach(section => {
            section.style.display = 'none';
        });
        document.getElementById(sectionId).style.display = 'block';
    }

    // Show Profile by default on page load
    document.addEventListener('DOMContentLoaded', function() {
        showSection('profile');
    });

    // Contact Form Submission Handling
    document.getElementById('contact-form').addEventListener('submit', function(event) {
        event.preventDefault();
        alert('Thank you for reaching out! I will get back to you soon.');
        event.target.reset();
    });
</script>
