# liberty-casino-demo
<!-- The full code from the previous slot demo I gave you -->  
<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8" />  
  <meta name="viewport" content="width=device-width, initial-scale=1" />  
  <title>Liberty Casino - USDT Slot Machine Demo</title>  
  <style>  
    body {  
      font-family: 'Arial', sans-serif;  
      background-color: #0d0d2b;  
      color: #fff;  
      margin: 0;  
      padding: 0;  
      display: flex;  
      flex-direction: column;  
      align-items: center;  
      min-height: 100vh;  
    }  
    header {  
      background: #1a1a4d;  
      width: 100%;  
      padding: 20px 0;  
      text-align: center;  
      box-shadow: 0 0 10px #333;  
      margin-bottom: 30px;  
    }  
    header h1 {  
      margin: 0;  
      font-size: 2.5rem;  
      color: #ffd700;  
      text-shadow: 1px 1px 3px #c18d00;  
    }  
    #balance-container {  
      margin-bottom: 20px;  
      font-size: 1.4rem;  
      font-weight: bold;  
    }  
    #deposit-withdraw {  
      margin-bottom: 30px;  
      display: flex;  
      gap: 20px;  
      flex-wrap: wrap;  
      justify-content: center;  
    }  
    input[type=number] {  
      padding: 10px;  
      font-size: 1rem;  
      border-radius: 5px;  
      border: none;  
      width: 150px;  
      text-align: center;  
    }  
    button {  
      background: #ffd700;  
      color: #1a1a4d;  
      border: none;  
      padding: 12px 25px;  
      font-size: 1.1rem;  
      font-weight: bold;  
      border-radius: 30px;  
      cursor: pointer;  
      box-shadow: 0 0 15px #ffd700;  
      transition: background 0.3s ease;  
      min-width: 120px;  
    }  
    button:hover:not(:disabled) {  
      background: #e6c200;  
    }  
    button:disabled {  
      background: #666;  
      cursor: not-allowed;  
      box-shadow: none;  
    }  
    #slot-machine {  
      background: #1a1a4d;  
      padding: 30px 40px;  
      border-radius: 15px;  
      box-shadow: 0 0 20px rgba(255, 215, 0, 0.5);  
      text-align: center;  
      max-width: 400px;  
      user-select: none;  
    }  
    #slots {  
      display: flex;  
      justify-content: center;  
      margin: 30px 0;  
      gap: 15px;  
    }  
    .slot {  
      background: #0d0d2b;  
      width: 80px;  
      height: 80px;  
      border-radius: 15px;  
      font-size: 3rem;  
      line-height: 80px;  
      color: #ffd700;  
      box-shadow: inset 0 0 10px #c18d00;  
    }  
    #message {  
      min-height: 40px;  
      font-size: 1.2rem;  
      font-weight: bold;  
      color: #fff;  
      margin-bottom: 20px;  
      min-width: 100%;  
    }  
    #bet-section {  
      margin-top: 20px;  
      display: flex;  
      justify-content: center;  
      gap: 10px;  
      flex-wrap: wrap;  
    }  
    #bet-input {  
      padding: 10px;  
      font-size: 1.1rem;  
      width: 120px;  
      text-align: center;  
      border-radius: 5px;  
      border: none;  
    }  
    footer {  
      margin-top: auto;  
      background: #1a1a4d;  
      color: #bbb;  
      width: 100%;  
      padding: 15px 0;  
      text-align: center;  
      font-size: 0.9rem;  
      border-top: 1px solid #333;  
      user-select: none;  
    }  
    @media (max-width: 480px) {  
      #slots {  
        gap: 10px;  
      }  
      .slot {  
        width: 60px;  
        height: 60px;  
        font-size: 2.4rem;  
        line-height: 60px;  
      }  
      #deposit-withdraw {  
        gap: 10px;  
      }  
      #bet-input {  
        width: 100px;  
      }  
    }  
  </style>  
</head>  
<body>  
  <header>  
    <h1>Liberty Casino - USDT Slots Demo</h1>  
  </header>  

  <
