
‏<!DOCTYPE html>
‏<html lang="he">
‏<head>
‏    <meta charset="UTF-8">
‏    <meta name="viewport" content="width=device-width, initial-scale=1.0">
‏    <title>טופס לשליחת קובץ ושדות נוספים</title>
‏</head>
‏<body>
‏    <h2>שלח נתונים להדפסה</h2>

‏    <form id="myForm" action="http://nz.or-efraim.co.il:4321/print" method="POST" enctype="multipart/form-data">
‏        <label for="fileInput">בחר קובץ:</label>
‏        <input type="file" name="file" id="fileInput" required><br><br>

‏        <label for="printerName">שם המדפסת:</label>
‏        <select name="printerName" id="printerName" required>
‏            <option value="1">חכמי ירושלים</option>
‏            <option value="22">אור אפרים</option>
‏        </select><br><br>

‏        <label for="duplex">האם הדפסה דו-צדדית?</label>
‏        <select name="duplex" id="duplex" required>
‏            <option value="true">כן</option>
‏            <option value="false">לא</option>
‏        </select><br><br>

‏        <label for="copies">מספר העותקים:</label>
‏        <input type="number" name="copies" id="copies" min="1" required><br><br>

‏        <input type="hidden" name="color" value="false"><br><br>

‏        <button type="button" onclick="submitForm()">שלח</button>
‏    </form>

‏    <script>
‏        function submitForm() {

‏const form = document.getElementById('myForm');
‏            form.submit(); // שליחת הטופס
        }
‏    </script>
‏</body>
‏</html>
