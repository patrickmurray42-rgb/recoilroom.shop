// Smooth scrolling for nav links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
anchor.addEventListener('click', function (e) {
e.preventDefault();
document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
});
});

// Placeholder for "Add to Cart" – expand with localStorage or integrate Snipcart for real e-comm
document.querySelectorAll('button').forEach(btn => {
if (btn.textContent === 'Add to Cart') {
btn.addEventListener('click', () => alert('Added to cart! (Demo – integrate real cart next)'));
}
});