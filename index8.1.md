1. HTML file — index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Layout</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="header">
        <h1>My Dashboard</h1>
        <p>Welcome back, Student!</p>
    </header>

    <div class="dashboard">

        <aside class="sidebar">
            <h2>Menu</h2>
            <a href="#">Dashboard</a>
            <a href="#">Students</a>
            <a href="#">Courses</a>
            <a href="#">Reports</a>
            <a href="#">Settings</a>
        </aside>

        <main class="main-content">
            <h2>Dashboard Overview</h2>

            <div class="cards">
                <div class="card">
                    <h3>Total Students</h3>
                    <p>1,250</p>
                </div>

                <div class="card">
                    <h3>Total Courses</h3>
                    <p>24</p>
                </div>

                <div class="card">
                    <h3>Assignments</h3>
                    <p>18</p>
                </div>

                <div class="card">
                    <h3>Completed Tasks</h3>
                    <p>85%</p>
                </div>
            </div>

            <section class="welcome">
                <h2>Welcome to Your Dashboard!</h2>
                <p>
                    This dashboard displays important information
                    using CSS Grid Layout.
                </p>
            </section>
        </main>

    </div>

</body>
</html>



2. CSS file — style.css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f1f5f9;
    color: #1e293b;
}

/* Dashboard Header */
.header {
    background-color: #1d4ed8;
    color: white;
    padding: 20px;
    display: grid;
    grid-template-columns: 1fr auto;
    align-items: center;
    gap: 10px;
}

/* Outer Dashboard Layout */
.dashboard {
    display: grid;
    grid-template-columns: 220px 1fr;
    grid-template-rows: 1fr;
    gap: 20px;
    padding: 20px;
    min-height: calc(100vh - 80px);
}

/* Sidebar */
.sidebar {
    background-color: #1e293b;
    color: white;
    padding: 20px;
    border-radius: 10px;
    display: grid;
    grid-template-rows: auto repeat(5, auto);
    gap: 15px;
    align-content: start;
}

.sidebar a {
    color: white;
    text-decoration: none;
    padding: 10px;
    border-radius: 5px;
}

.sidebar a:hover {
    background-color: #334155;
}

/* Main Content */
.main-content {
    display: grid;
    grid-template-rows: auto auto 1fr;
    gap: 20px;
    align-content: start;
}

/* Statistic Cards */
.cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, auto);
    gap: 20px;
}

.card {
    background-color: white;
    padding: 25px;
    border-radius: 10px;
    border-left: 5px solid #2563eb;
    box-shadow: 0 2px 8px #00000010;
}

.card h3 {
    color: #64748b;
    margin-bottom: 15px;
}

.card p {
    font-size: 28px;
    font-weight: bold;
    color: #2563eb;
}

.welcome {
    background-color: white;
    padding: 25px;
    border-radius: 10px;
    line-height: 1.8;
}

/* Responsive Layout */
@media (max-width: 650px) {
    .header {
        grid-template-columns: 1fr;
    }

    .dashboard {
        grid-template-columns: 1fr;
        grid-template-rows: auto 1fr;
    }

    .sidebar {
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: auto auto auto;
    }

    .sidebar h2 {
        grid-column: 1 / -1;
    }

    .cards {
        grid-template-columns: 1fr;
        grid-template-rows: auto;
    }
}



3. How to run your assignment
1. Create a folder named Assignment-8.1.
2. Create index.html and style.css inside that folder.
3. Copy the HTML code into index.html.
4. Copy the CSS code into style.css.
5. Save both files and open index.html in your browser.







dribbble.com


4. Assignment requirements checklist
- [x] Dashboard header created.
- [x] Sidebar and main content area created.
- [x] Four statistic cards added.
- [x] display: grid used for the layout.
- [x] grid-template-columns and grid-template-rows used.
- [x] Gaps added between cards.
- [x] Responsive design added for mobile screens.
- [ ] Open the webpage in your browser and inspect the layout.