  <!DOCTYPE html>
  <html lang="zh">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>量化交易网站</title>
      <style>
          body {
              font-family: Arial, sans-serif;
              background-color: #f4f4f4;
              margin: 0;
              padding: 20px;
          }
          header {
              background: #35424a;
              color: #ffffff;
              padding: 10px 0;
              text-align: center;
          }
          .container {
              max-width: 800px;
              margin: auto;
              background: #ffffff;
              padding: 20px;
              border-radius: 5px;
              box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
          }
          h1 {
              margin: 0;
          }
          .form-group {
              margin: 15px 0;
          }
          label {
              display: block;
              margin-bottom: 5px;
          }
          input[type="text"], input[type="number"] {
              width: 100%;
              padding: 10px;
              border: 1px solid #ccc;
              border-radius: 4px;
          }
          button {
              background: #35424a;
              color: #ffffff;
              border: none;
              padding: 10px 15px;
              cursor: pointer;
              border-radius: 4px;
          }
          button:hover {
              background: #45a049;
          }
      </style>
  </head>
  <body>
      <header>
          <h1>量化交易平台</h1>
      </header>
      <div class="container">
          <h2>策略输入</h2>
          <div class="form-group">
              <label for="strategyName">策略名称:</label>
              <input type="text" id="strategyName" placeholder="输入策略名称">
          </div>
          <div class="form-group">
              <label for="investmentAmount">投资金额:</label>
              <input type="number" id="investmentAmount" placeholder="输入投资金额">
          </div>
          <button onclick="submitStrategy()">提交策略</button>
          <div id="output" style="margin-top: 20px;"></div>
      </div>
      <script>
          function submitStrategy() {
              const name = document.getElementById('strategyName').value;
              const amount = document.getElementById('investmentAmount').value;
              document.getElementById('output').innerHTML = 
                  `<h3>策略已提交:</h3><p>策略名称: ${name}</p><p>投资金额: ${amount}</p>`;
          }
      </script>
  </body>
  </html>
