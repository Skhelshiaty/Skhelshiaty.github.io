// Smooth scrolling
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function(e) {
    e.preventDefault();

    const target = document.querySelector(this.getAttribute('href'));

    if (target) {
      target.scrollIntoView({
        behavior: 'smooth'
      });
    }
  });
});

// Navbar effect on scroll
const navbar = document.querySelector('.navbar');

window.addEventListener('scroll', () => {
  if (window.scrollY > 50) {
    navbar.style.background = '#ffffff';
  } else {
    navbar.style.background = '#ffffff';
  }
});

console.log("Portfolio loaded successfully!");