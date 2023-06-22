# Basic-Geometry
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Geometry </title>
    <style>
        

        input[type="text"],
        input[type="number"] {
            width: 30%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin: 10px;
        }

        button {
            background-color: #4daea1;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
        }

        button:hover {
            background-color: #4caf84;
        }
         
         section {
      width: 65%;
      background-color: #e0e0e0;
      border: 1px solid #ccc;
      margin: 20px auto;
      border-radius: 5px 10px;
    }
    
    .wrapper {
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        width: 70%;
        background-color: #f0f0f0;
        margin: 0 auto;
        padding: 5px;
        text-align: center;
        box-sizing: border-box;
    }

    .wrapper h1 {
        font-size: 24px;
        margin-bottom: 10px;
    }

    .wrapper p {
        margin-bottom: 10px;
    }

    .wrapper ul {
        list-style-type: none;
        padding: 0;
    }

    .wrapper li {
        margin-bottom: 5px;
    }

    .wrapper a {
         
        color: inherit;
    }
</style>

     
    

    <script>
        function AreaOfCircle() {
            // Calculate the area of circle
            var radius = document.getElementById("radius").value;
            var area = Math.PI * radius * radius;
            // Display the result
            alert("The area of the given circle radius is: " + area.toFixed(2));
            document.getElementById("circle-area").value = area.toFixed(2);
        }

        function Triangle() {
            // Calculate the area of the triangle
            var base = parseFloat(document.getElementById('triangle-base').value);
            var height = parseFloat(document.getElementById('triangle-height').value);
            var area = (base * height) / 2;
            // Display the result
            alert("The area of the given triangle is: " + area.toFixed(2));
            document.getElementById("triangle-area").value = area.toFixed(2);
        }
         
        function Square() {
            // Calculate the area of the Square
            var side  = parseFloat(document.getElementById('side').value);
            
            var area = side * side ;
            // Display the result
            alert("The area of the given Square is: " + area.toFixed(2));
            document.getElementById("Square-area").value = area.toFixed(2);
        }

        function Rectangle() {
            // Calculate the area of the Rectangle
            var base = parseFloat(document.getElementById('rectangle-base').value);
            var height = parseFloat(document.getElementById('rectangle-height').value);
            var area = base * height;
            // Display the result
            alert("The area of the given Rectangle is: " + area.toFixed(2));
            document.getElementById("rectangle-area").value = area.toFixed(2);
        }
    </script>
</head>

<body>
    <div class="wrapper">
        <h1 id="top">Basic Geometry</h1>
        <p >In this section, we are going to find the area of some two-dimensional shapes.</p>
        <p >You can click on any shape below:</p>
        <ul style="list-style-type: none;">
            <li><a href="#circle" style="text-decoration: none; color: inherit;">Circle</a></li>
            <li><a href="#triangle" style="text-decoration: none; color: inherit;">Triangle</a></li>
            <li><a href="#square" style="text-decoration: none; color: inherit;">Square</a></li>
            <li><a href="#rectangle" style="text-decoration: none; color: inherit;">Rectangle</a></li>
          </ul>


        <section id="circle">
            <h2>Circle Area Calculator</h2>
            <div>
                <label for="radius">Enter the value of the Circle's Radius:</label>
                <input type="text" id="radius">
            </div>
            <div>
                <label for="circle_area">Result:</label>
                <input type="text" id="circle-area" readonly>
            </div>
            <hr>
            <button onclick="AreaOfCircle()">Calculate</button>
        </section>

         <!-- Go to Top -->
        <div class="go"><a href="#top">Go to top</a>
        </div>

        <section id="triangle">
            <h2>Triangle Area Calculator</h2>
            <div>
                <label for="triangle-base">Enter Base Value:</label>
                <input type="number" name="triangle-base" id="triangle-base">
                <br>
                <label for="triangle-height">Enter Height:</label>
                <input type="number" name="triangle-height" id="triangle-height">
            </div>
            <div>
                <label for="triangle-area">Result:</label>
                <input type="text" id="triangle-area" readonly>
            </div>
            <hr>
            <button onclick="Triangle()">Calculate</button>
        </section>
         
        <!-- Go to Top -->
        <div class="go"><a href="#top">Go to top</a>
        </div>

        <section id="Square">
            <h3>Square Area Calculator</h2>
            <div>
                <label for="side ">Enter side Value:</label>
                <input type="number" name="side" id="side">
                
            </div>
            <div>
                <label for="Square_area">Result:</label>
                <input type="text" id="Square-area" readonly>
            </div>
            <hr>
            <button onclick="Square()">Calculate</button>
        </section>


        <!-- Go to Top -->
        <div class="go"><a href="#top">Go to top</a>
        </div>

        <section id="rectangle">
            <h2>Rectangle Area Calculator</h2>
            <div>
                <label for="rectangle-base">Enter Base Value:</label>
                <input type="number" name="rectangle-base" id="rectangle-base">
                <br>
                <label for="rectangle-height">Enter Height:</label>
                <input type="number" name="rectangle-height" id="rectangle-height">
            </div>
            <div>
                <label for="rectangle-area">Result:</label>
                <input type="text" id="rectangle-area" readonly>
            </div>
            <hr>
            <button onclick="Rectangle()">Calculate</button>
        </section>

        <!-- Go to Top -->
        <div class="go"><a href="#top">Go to top</a>
        </div>
        <footer style="background-color: #f8f8f8; padding: 10px;">
            <p style="text-align: center; margin-bottom: 0;">&copy; 2023 Your Website. All rights reserved.</p>
        </footer>
    </div>
</body>

</html>
