<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Code Search</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
            max-width: 1012px;
            margin: 0 auto;
            padding: 20px;
            color: #24292e;
            line-height: 1.5;
        }
        h1 {
            font-size: 24px;
            font-weight: 600;
            margin-bottom: 20px;
        }
        .search-container {
            display: flex;
            margin-bottom: 30px;
        }
        .search-input {
            flex: 1;
            padding: 5px 12px;
            font-size: 14px;
            line-height: 20px;
            border: 1px solid #d1d5da;
            border-radius: 6px;
            box-shadow: inset 0 1px 2px rgba(27,31,35,0.075);
        }
        .search-button {
            margin-left: 10px;
            padding: 5px 16px;
            font-size: 14px;
            font-weight: 500;
            color: white;
            background-color: #2ea44f;
            border: 1px solid rgba(27,31,35,0.15);
            border-radius: 6px;
            cursor: pointer;
        }
        h2 {
            font-size: 20px;
            font-weight: 600;
            margin: 24px 0 16px;
            padding-bottom: 8px;
            border-bottom: 1px solid #eaecef;
        }
        .time-item {
            font-weight: 600;
            margin: 10px 0;
        }
        .code-item {
            margin: 15px 0;
        }
        .code-title {
            font-weight: 600;
            color: #0366d6;
        }
        .code-date {
            font-size: 12px;
            color: #586069;
        }
    </style>
</head>
<body>
    <h1>Code</h1>
    
    <div class="search-container">
        <input type="text" class="search-input" placeholder="Search Code Example SSNI-999">
        <button class="search-button">Search</button>
    </div>
    
    <hr>
    
    <h2>Popular Today</h2>
    
    <div class="time-item">2:20:00</div>
    <div class="time-item">23:15:00</div>
    <div class="time-item">2:10:00</div>
    
    <div class="code-item">
        <div class="code-title">TEK-102 Flo...</div>
        <div class="code-date">03 Jun 2025</div>
    </div>
    
    <div class="code-item">
        <div class="code-title">CRDD-034 Bl...</div>
        <div class="code-date">29 May 2024</div>
    </div>
    
    <div class="code-item">
        <div class="code-title">START-258 A ...</div>
        <div class="code-date">04 Feb 2025</div>
    </div>
    
    <div class="time-item">3:42</div>
    <div class="time-item">2:24:00</div>
    <div class="time-item">2:25:00</div>
    <div class="time-item">4:15:00</div>
    
    <div class="code-item">
        <div class="code-title">START-257 A...</div>
        <div class="code-date">10 Feb 2025</div>
    </div>
    
    <div class="code-item">
        <div class="code-title">FSVSS-015 [V...]</div>
        <div class="code-date">01 Jun 2025</div>
    </div>
    
    <div class="code-item">
        <div class="code-title">SDMM-201 E...</div>
        <div class="code-date">03 Jun 2025</div>
    </div>
</body>
</html>
