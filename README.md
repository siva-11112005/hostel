<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>srikar Lodge</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background: #f4f4f4;
            color: #333;
        }
        header {
            background: #ff6600;
            color: white;
            padding: 20px;
            font-size: 24px;
            font-weight: bold;
        }
        .container {
            padding: 20px;
        }
        .room {
            border-radius: 10px;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
            padding: 20px;
            margin: 20px;
            display: inline-block;
            width: 30%;
            background: white;
            transition: transform 0.3s;
        }
        .room:hover {
            transform: scale(1.05);
        }
        .room img {
            width: 100%;
            border-radius: 10px;
            height: 200px;
            object-fit: cover;
        }
        button {
    background: #ff6600;
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    border-radius: 5px;
    font-size: 16px;
}

button:hover {
    background: #cc5500;
}

button a {
    color: white;
    text-decoration: none;
    display: block;
    width: 100%;
    height: 100%;
}

button a:hover {
    background: none;
}

        footer {
            background: #333;
            color: white;
            padding: 15px;
            margin-top: 20px;
        }
        .booking-form {
            text-align: left;
            margin-top: 20px;
        }
        .booking-form input,
        .booking-form select,
        .booking-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid #ccc;
        }
    </style>
</head>
<body>
    <header>
        <h1>Srikar LODGE</h1>
    </header>
    <div class="container">
        <h2>Our Rooms</h2>
        <div class="room">
            <img src="https://i.pinimg.com/736x/9e/b4/51/9eb451db593c7ed8bcfd03cdf26d6e9c.jpg" alt="Single Room">
            <h3>Single Room</h3>
            <p>Cozy and affordable single room.</p>
            <button><a href="#bookingForm"> Book Now</a></button>
        </div>
        <div class="room">
            <img src="https://www.hospitalitynet.org/picture/xxl_153093123.jpg" alt="Double Room">
            <h3>Double Room</h3>
            <p>Spacious double room with amenities.</p>
            <button ><a href="#bookingForm"> Book Now</a></button>
        </div>
        <div class="room">
            <img src="https://i.pinimg.com/736x/c9/0d/67/c90d6776a0aba2bfa75c3427238f5ba9.jpg" alt="Dormitory">
            <h3>Dormitory</h3>
            <p>Budget-friendly dormitory for travelers.</p>
            <button><a href="#bookingForm"> Book Now</a></button>
        </div>

        <div class="booking-form" id="bookingForm" style="display:flexbox;">
            <h3>Book Your Room</h3>
            <form action="submit-booking.html" method="POST">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <input type="tel" name="phone" placeholder="Your Phone" required>
                <select name="room" required>
                    <option value="" disabled selected>Select Room Type</option>
                    <option value="Single thiRoom">Single Room</option>
                    <option value="Double Room">Double Room</option>
                    <option value="Dormitory">Dormitory</option>
                </select>
                <input type="date" placeholder="select yoor date"><input type="time" placeholder="select your time" required>
                <textarea name="message" placeholder="Any Special Requests?" rows="4"></textarea>
                <button type="submit">Submit Booking</button>
            </form>
        </div>
    </div>

    <footer>
        <p>Contact us at: info@srikarlodge.com | Phone: +91 98765 43210</p>
    </footer>

</body>
</html>
#submit page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Booking Success</title>
    <style>
        body {
            background: linear-gradient(to right, rgb(233, 104, 192), rgb(138, 5, 96));
            font-family: 'Poppins', sans-serif;
            text-align: center;
            color: white;
        }
        .b {
            background-color: rgba(239, 66, 66, 0.9);
            width: 400px;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
            margin: 150px auto;
            text-align: center;
        }
        h1 {
            font-size: 24px;
        }
        button {
            margin-top: 30px;
            border: none;
            border-radius: 8px;
            padding: 12px 20px;
            background-color: rgb(32, 102, 12);
            color: white;
            font-size: 16px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.2s;
        }
        button:hover {
            background-color: rgb(25, 85, 10);
            transform: scale(1.05);
        }
        button a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            display: block;
        }
    </style>
</head>
<body>
    <div class="b">
        <h1>Your Booking is Successful! 🎉</h1>
        <button><a href="srikar.html">Book Another Room</a></button>
    </div>
</body>
</html>

