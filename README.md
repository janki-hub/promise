# promise
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>promise</title>
</head>
<body>
    <h1 id="pr"></h1>
    
    <script>
        let myPromise = new Promise(function (myResolve, myReject) {
            setTimeout(function () { myResolve("janki solanki"); }, 3000);
        });

        myPromise.then(function (value) {
            document.getElementById("pr").innerHTML = value;
        });
    </script>
</body>
