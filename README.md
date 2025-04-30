# HW
/* Общие стили */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  background-color: #f9f9f9;
  color: #333;
}

header,
footer {
  background-color: #005f73;
  color: #fff;
  text-align: center;
  padding: 1rem 0;
}

.container {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  padding: 1rem;
}

.content-box {
  background: #fff;
  padding: 1rem;
  border-radius: 0.5rem;
  box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
}

.content-box img {
  width: 100%;
  height: auto;
  display: block;
  border-radius: 0.5rem;
}

/* Планшет: ≥ 772px */
@media (min-width: 772px) {
  .container {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
  }

  .content-box {
    width: 45%;
  }

  .content-box img {
    max-height: 30vh;
  }
}

/* Широкоэкранный: ≥ 998px */
@media (min-width: 998px) {
  .content-box {
    width: 30%;
  }
}

