<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./styles.css">
        
    </head> 
    <body>
        <div class="container">
            <div >
                <h1 class = "header_text">Do you wanna go out with me?</h1>
            </div>
            <div class="gif_container">
                <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExd2F6dGp4ODNlc2loN2kxeWhmc2N1bTI5NWp2Ym54OXgwY2hvbDgyMSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/LTNTIw21Qy0ko8SS4Y/giphy.gif">
            </div>
            <div class = "buttons">
                <button class="btn" id = "yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 85;
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 48;
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                    }
                </script> 
            </div>
        </div>
       
    </body> 
</html>
