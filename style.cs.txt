* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body, html {
  width: 100%;
  height: 100%;
  overflow: hidden;
  font-family: 'Segoe UI', sans-serif;
  background: #0a0a0a;
  color: white;
}

canvas#particles {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
}

.content {
  position: relative;
  z-index: 2;
  text-align: center;
  top: 40%;
  transform: translateY(-50%);
  animation: fadeIn 2s ease-in-out;
}

h1.glow {
  font-size: 4rem;
  color: #00ffe0;
  text-shadow: 0 0 20px #00ffe0, 0 0 40px #00ffe0;
  animation: pulse 2s infinite alternate;
}

p.tagline {
  margin-top: 10px;
  color: #aaa;
  font-size: 1.2rem;
  animation: fadeIn 3s ease-in-out;
}

footer {
  margin-top: 20px;
  font-size: 0.9rem;
  color: #555;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes pulse {
  from { text-shadow: 0 0 10px #00ffe0; }
  to { text-shadow: 0 0 40px #00ffe0; }
}
