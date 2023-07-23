# Data-visualization-javascript-code
document.addEventListener("DOMContentLoaded", function () {
    const barChartCanvas = document.getElementById("barChart");
    
    const data = {
        labels: ['Data 1', 'Data 2', 'Data 3', 'Data 4', 'Data 5'],
        datasets: [{
            label: 'Sample Data',
            data: [23,18,19,45,68,89,45],
            backgroundColor: 'rgba(54, 162, 235, 0.6)',
            borderColor: 'rgba(54, 162, 235, 1)',
            borderWidth: 1
        }]
    };

    const options = {
        responsive: true,
        maintainAspectRatio: false,
        scales: {
            y: {
                beginAtZero: true
            }
        }
    };

    new Chart(barChartCanvas, {
        type: 'bar',
        data: data,
        options: options
    });
});
