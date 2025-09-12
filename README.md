## Hi there 👋


**m4ruf07/m4ruf07** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
- ... Be positive ...
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Line Graph Example</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f0f0f0;
    }
    #myChart {
      max-width: 600px;
      width: 100%;
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 4px 8px rgba(0,0,0,0.1);
    }
  </style>
</head>
<body>

  <canvas id="myChart"></canvas>

  <!-- Chart.js Library -->
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script>
    const ctx = document.getElementById('myChart').getContext('2d');

    const myChart = new Chart(ctx, {
      type: 'line', // Change to 'bar', 'pie', etc.
      data: {
        labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun'],
        datasets: [{
          label: 'Sales (in USD)',
          data: [120, 190, 300, 250, 400, 350],
          backgroundColor: 'rgba(54, 162, 235, 0.2)',
          borderColor: 'rgba(54, 162, 235, 1)',
          borderWidth: 2,
          fill: true,
          tension: 0.3 // Smooth curve
        }]
      },
      options: {
        responsive: true,
        plugins: {
          legend: {
            position: 'top',
          },
          title: {
            display: true,
            text: 'Monthly Sales Data'
          }
        },
        scales: {
          y: {
            beginAtZero: true
          }
        }
      }
    });
  </script>

</body>
</html>
