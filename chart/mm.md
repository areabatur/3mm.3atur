 
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Document</title>
      <script src="libs/jquery.min.js"></script>
      <script src="libs/marked.min.js"></script>
      <script src="libs/mermaid.full.js"></script>
    </head>
    <body>

    <div id="content"></div>

    <script>

      var renderer = new marked.Renderer();
      renderer.code = function (code, language) {
        if(code.match(/^sequenceDiagram/)||code.match(/^graph/)){
           return '<div class="mermaid">'+code+'</div>';
        }
      };

        $(document).ready(function(){

        $.get( "test.md", function( data ) {
          // console.log(data);
          $('#content').html(marked(data));
        });

      });

    console.log(marked('```graph TD;A-->B;A-->C;B-->D;C-->D;```', { renderer: renderer }));

    </script>
    </body>
    </html>
