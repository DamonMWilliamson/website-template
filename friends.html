<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Friends</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        #linkList {
            list-style-type: none;
            padding: 0;
        }
        #linkList li {
            margin-bottom: 10px;
        }
        .error {
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Friends</h1>
    <div id="status"></div>
    <ul id="linkList"></ul>

    <script>
        const csvFilePath = 'friends.csv';

        function loadAndProcessCSV() {
            const status = document.getElementById('status');
            status.textContent = 'Loading CSV file...';

            fetch(csvFilePath)
                .then(response => {
                    if (!response.ok) {
                        throw new Error(`HTTP error! status: ${response.status}`);
                    }
                    return response.text();
                })
                .then(data => {
                    status.textContent = 'Processing CSV data...';
                    processCSV(data);
                    status.textContent = '';
                })
                .catch(error => {
                    console.error('Error:', error);
                    status.innerHTML = `<span class="error">Error: ${error.message}</span>`;
                });
        }

        function processCSV(csv) {
            const rows = csv.split('\n').map(row => row.trim().split(','));
            const header = rows.shift(); // Remove header row

            // Sort rows based on pin (column 3)
            const sortedRows = rows.sort((a, b) => {
                const pinA = parseInt(a[2]) || Infinity;
                const pinB = parseInt(b[2]) || Infinity;
                return pinA - pinB;
            });

            // Separate pinned and unpinned rows
            const pinnedRows = sortedRows.filter(row => row.length > 2 && parseInt(row[2]));
            const unpinnedRows = sortedRows.filter(row => row.length <= 2 || !parseInt(row[2]));

            // Shuffle unpinned rows
            for (let i = unpinnedRows.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [unpinnedRows[i], unpinnedRows[j]] = [unpinnedRows[j], unpinnedRows[i]];
            }

            // Combine pinned and unpinned rows
            const finalRows = [...pinnedRows, ...unpinnedRows];

            // Create and display links
            const linkList = document.getElementById('linkList');
            linkList.innerHTML = '';

            finalRows.forEach(row => {
                if (row.length < 2) return; // Skip incomplete rows
                const [name, url] = row;
                const li = document.createElement('li');
                const a = document.createElement('a');
                a.href = url;
                a.textContent = name;
                a.target = "_blank"; // This makes links open in new tabs
                a.rel = "noopener noreferrer"; // Security best practice for target="_blank"
                li.appendChild(a);
                linkList.appendChild(li);
            });
        }

        // Load and process the CSV when the page loads
        window.addEventListener('load', loadAndProcessCSV);
    </script>
</body>
</html>