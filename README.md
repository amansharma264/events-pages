footer {
    text-align: center;
    padding: 30px;
    background: rgba(255, 0, 0, 0.1);
    margin-top: 50px;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-bottom: 20px;
}

.social-links a {
    color: white;
    font-size: 1.5rem;
    transition: all 0.3s ease;
}

.social-links a:hover {
    color: #ff0000;
}

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

// Mobile Menu Toggle
const menuToggle = document.querySelector('.menu-toggle');
const navLinks = document.querySelector('.nav-links');

menuToggle.addEventListener('click', () => {
    navLinks.classList.toggle('active');
});

// Close mobile menu when clicking a link
document.querySelectorAll('.nav-links a').forEach(link => {
    link.addEventListener('click', () => {
        navLinks.classList.remove('active');
    });
});
