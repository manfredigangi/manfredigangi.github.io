<!DOCTYPE html>
<html>
<head>
    <title>User-Fillable Table</title>
    <style>
        table {
            border-collapse: collapse;
            width: 100%;
        }

        th, td {
            border: 1px solid black;
            padding: 8px;
        }

        th {
            background-color: #f2f2f2;
        }

        td input {
            width: 100%;
        }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>Column 1</th>
                <th>Column 2</th>
                <th>Column 3</th>
                <th>Column 4</th>
                <th>Column 5</th>
                <th>Column 6</th>
                <th>Column 7</th>
                <th>Column 8</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
                <td><input type="text"></td>
            </tr>
            <!-- Repeat the above <tr> element for the remaining rows -->
            <!-- Total 20 rows -->
        </tbody>
    </table>
</body>
</html>
