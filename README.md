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
    <script>
        function calculateColumnSum(columnIndex) {
            var table = document.getElementById("myTable");
            var rows = table.getElementsByTagName("tr");
            var sum = 0;

            for (var i = 1; i < rows.length; i++) {
                var row = rows[i];
                var cell = row.getElementsByTagName("td")[columnIndex];
                var value = parseFloat(cell.firstChild.value);

                if (!isNaN(value)) {
                    sum += value;
                }
            }

            return sum;
        }

        function updateSum() {
            var sumElement = document.getElementById("sum");
            var columnIndex = parseInt(sumElement.getAttribute("data-column"));

            var columnSum = calculateColumnSum(columnIndex);
            sumElement.textContent = "Sum: " + columnSum;
        }
    </script>
</head>
<body>
    <table id="myTable">
        <thead>
            <tr>
                <th></th> <!-- Empty cell in row 1 column 1 -->
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
                <td></td> <!-- Empty cell in row 1 column 1 -->
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <!-- Repeat the above <tr> element for the remaining 19 rows -->
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <tr>
                <td></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
                <td><input type="text" oninput="updateSum()"></td>
            </tr>
            <!-- Repeat this row for the remaining 18 rows -->
            <!-- Total 20 rows -->
        </tbody>
    </table>

    <p id="sum" data-column="1">Sum: 0</p>
</body>
</html>
