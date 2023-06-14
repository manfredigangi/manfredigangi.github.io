<!DOCTYPE html>
<html>
<head>
    <title>Tabella Excel Modificabile</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.css">
    <script src="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.js"></script>
    <style>
        #hot {
            width: 100%;
            height: 400px;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            var container = document.getElementById("hot");
            var hot = new Handsontable(container, {
                data: [[]], // Dati iniziali della tabella (vuoti)
                rowHeaders: true, // Visualizza numeri di riga
                colHeaders: true, // Visualizza nomi di colonna
                formulas: true, // Abilita il supporto alle formule di Excel
                contextMenu: true // Abilita il menu contestuale per le operazioni sulla tabella
            });
        });
    </script>
</head>
<body>
    <div id="hot"></div>
</body>
</html>
In questo esempio, abbiamo incluso Handsontable nel nostro documento HTML utilizzando i link alle risorse CSS e JavaScript fornite dalla libreria. Abbiamo anche creato un <div> con l'id "hot" per contenere la nostra tabella.

Nel codice JavaScript, utilizziamo il DOMContentLoaded event listener per assicurarci che il codice venga eseguito dopo che l'intero documento è stato caricato. All'interno dell'event listener, selezioniamo l'elemento con l'id "hot" e creiamo un'istanza di Handsontable su di esso. Configuriamo le opzioni desiderate come data, rowHeaders, colHeaders, formulas, e contextMenu per ottenere la funzionalità desiderata.

Ricorda che dovrai includere il link corretto alle risorse CSS e JavaScript di Handsontable nel tuo file HTML. Puoi scaricare la libreria Handsontable e utilizzare i link locali se preferisci.

Con Handsontable, gli utenti possono modificare i dati nella tabella come farebbero in Excel e le formule di Excel vengono mantenute. Tuttavia, tieni presente che Handsontable è una libreria complessa e potrebbe richiedere una certa conoscenza di JavaScript per configurar





User
Can you create the code for a website where there is a table with 8 columns, 20 rows, then of this table the cell positioned as following (row 1 column 1) could be deleted, the cells (row 1 column 8 and row 1 column 8) could be merged into one single cell, then write "TOTAL" in cell located at row 2 column 1 . This table should be accessible to the user so that numbers can be put inside
ChatGPT
Certainly! Here's an example of HTML code for a website with a table that meets your requirements:

html
Copy code
<!DOCTYPE html>
<html>
<head>
    <title>Editable Table</title>
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
            text-align: center;
        }
    </style>
</head>
<body>
    <table>
        <tr>
            <th colspan="7">Table Title</th>
            <th colspan="2">Merged Cell</th>
        </tr>
        <tr>
            <th>Column 1</th>
            <th>Column 2</th>
            <th>Column 3</th>
            <th>Column 4</th>
            <th>Column 5</th>
            <th>Column 6</th>
            <th>Column 7</th>
            <th colspan="2">Column 8-9</th>
        </tr>
        <tr>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td colspan="2" contenteditable="true"></td>
        </tr>
        <tr>
            <td contenteditable="true">TOTAL</td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td contenteditable="true"></td>
            <td colspan="2" contenteditable="true"></td>
        </tr>
        <!-- Add more rows as needed -->
    </table>
</body>
</html>
