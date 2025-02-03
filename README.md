<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Стили</title>
    <style>
        body{font-family: 'Arial', sans-serif;
            margin: 35px;
                background-color:#f9f9f9;
           color:#444;}

       h2  {border:3px dashed #ef9a9a;
           border-radius:12px;padding: 17px;text-align:center;
                background-color: #fff;  box-shadow: 0 3px 7px rgba(0,0,0,.1);
              margin-bottom: 23px;}
        ul{padding-left: 32px;list-style-type:circle;}
        li {border: 1px solid #ffccbc;padding: 13px;
               margin-bottom: 7px;background-color:#fff;
            border-radius:6px;
        box-shadow: 0 2px 3px rgba(0,0,0,.1);}

        form  {margin-top:31px;padding: 19px;display: inline-block;
               border:2px solid #a1887f;
            border-radius: 11px;background-color: #f0ede8;}

         button:hover
         {
            background-color:#4caf50;color: white;
           transform:scale(1.03);transition: transform .2s ease;
           }

        li:nth-child(odd) {background-color: #f1f1f1;    }

        li:nth-child(even){background-color: #fafafa;}


       input:focus {outline: none; border: 2px solid #52b8d2;box-shadow: 0 0 6px rgba(52,152,219,.6);
        }


        h2::first-line {font-weight: bold;  text-transform:uppercase; letter-spacing:1.4px;color:#ff7043;}

        li::first-letter{font-size:1.7em; color:#f44336;font-weight:bold;}
         input::placeholder{color: #9e9e9e;font-style: italic; font-weight: 300;}


          .advanced-block {border: 3px solid #9c27b0;
            border-radius: 20px;box-shadow: 6px 6px 14px rgba(0,0,0,.2);
            padding:24px;margin: 32px 0;
           background-color:#fff;text-align:center; position:relative;
              transition: transform .2s ease;       }

          .advanced-block:hover{
            transform:translateY(-4px) ;}


        .advanced-block:not(.no-style)
          {color: #333; }

         .advanced-block::before {
           content:"✨";
            font-size:2em;margin-right:9px;
               color: #ab47bc;  position: absolute;top: 4px;left: 4px;    }
        .advanced-block::after {
              content: "✨";
              font-size: 2em;
                margin-left:10px;
            color:#ab47bc;position:absolute;
            bottom:3px;right:4px;}
    </style>
</head>
<body>
  <h2>Стилизация границ и отступов</h2>
    <ul>
        <li>Список 1</li>
        <li>Список 2</li>
        <li>Список 3</li>
        <li>Список 4</li>
    </ul>
  <form>
       <input type="text" placeholder="Текст">
       <button>Отправить</button>
    </form>

  <div class="advanced-block">
     Продвинутая стилизация
    </div>
    <div class="advanced-block no-style"> Продвинутая стилизация с no-style</div>
</body>
</html>
