# landingpage
Maiya Landing page

Create Json Service:
	https://learningactors.com/3-ways-to-create-your-own-api/

	npm install -g json-server
	json-server --watch mtidetails.json --port 8080


	<script type="text/javascript">
        document.addEventListener('DOMContentLoaded', function() {
             userAction();
        }, false);
        const userAction = async () => {
                const response = await fetch('http://localhost:8080/data');
                const myJson = await response.json();
                console.log(myJson);        
                document.getElementById("Maiya_Title").innerHTML = myJson[0]["Title"];
                document.getElementById("Maiya_Title_Description").innerHTML = myJson[0]["Description"];    
        }
    </script>

    <form action="mailto:you@yourdmainhere.com" method="post" enctype="text/plain" >
                    <input type="Submit" name="Request Demo"class="mi-button mi-button--green"/>
                </form>
