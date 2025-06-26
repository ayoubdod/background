const colors = ['#8a2be2', '#9370db', '#6a5acd', '#7b68ee', '#4169e1', '#00bfff'];
const balloonCount = 25;

for (let i = 0; i < balloonCount; i++) {
  const balloon = document.createElement('div');
  balloon.classList.add('balloon');
  balloon.style.left = `${Math.random() * 100}%`;
  balloon.style.animationDuration = `${5 + Math.random() * 10}s`;
  balloon.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
  balloon.style.opacity = Math.random().toFixed(2);
  document.querySelector('.background').appendChild(balloon);
}
