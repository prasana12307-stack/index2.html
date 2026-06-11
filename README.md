# index2.html
movie ticket generator
<!DOCTYPE html>
<html>
<head>
    <title>Movie Ticket Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 30px;
        }

        .container {
            width: 400px;
            margin: auto;
        }

        input {
            width: 100%;
            padding: 8px;
            margin: 5px 0;
        }

        button {
            padding: 10px;
            background: #28a745;
            color: white;
            border: none;
            cursor: pointer;
        }

        .ticket {
            margin-top: 20px;
            border: 2px dashed black;
            padding: 15px;
            display: none;
        }

        h2 {
            text-align: center;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Movie Ticket Generator</h2>

    <input type="text" id="customer" placeholder="Customer Name">
    <input type="text" id="movie" placeholder="Movie Name">
    <input type="text" id="theater" placeholder="Theater Name">
    <input type="date" id="date">
    <input type="time" id="time">
    <input type="text" id="seat" placeholder="Seat Number">
    <input type="number" id="price" placeholder="Ticket Price">

    <button onclick="generateTicket()">Generate Ticket</button>

    <div class="ticket" id="ticket">
        <h3>🎬 Movie Ticket</h3>
        <p><b>Customer:</b> <span id="tCustomer"></span></p>
        <p><b>Movie:</b> <span id="tMovie"></span></p>
        <p><b>Theater:</b> <span id="tTheater"></span></p>
        <p><b>Date:</b> <span id="tDate"></span></p>
        <p><b>Time:</b> <span id="tTime"></span></p>
        <p><b>Seat:</b> <span id="tSeat"></span></p>
        <p><b>Price:</b> ₹<span id="tPrice"></span></p>
    </div>
</div>

<script>
function generateTicket() {
    document.getElementById("tCustomer").innerText =
        document.getElementById("customer").value;

    document.getElementById("tMovie").innerText =
        document.getElementById("movie").value;

    document.getElementById("tTheater").innerText =
        document.getElementById("theater").value;

    document.getElementById("tDate").innerText =
        document.getElementById("date").value;

    document.getElementById("tTime").innerText =
        document.getElementById("time").value;

    document.getElementById("tSeat").innerText =
        document.getElementById("seat").value;

    document.getElementById("tPrice").innerText =
        document.getElementById("price").value;

    document.getElementById("ticket").style.display = "block";
}
</script>

</body>
</html>
