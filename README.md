# kaushal-tours-and-travels
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Book Hyundai Aura and Maruti Suzuki Dzire taxis with Kaushal Tours and Travels. AC and Non-AC options available.">
<title>Kaushal Tours and Travels | Taxi Booking</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#f4f7fb;color:#182238}
header{background:#102448;color:white;text-align:center;padding:30px 15px}
header h1{margin:0;font-size:29px}
header p{margin-bottom:0}
nav{background:#193967;text-align:center;padding:14px}
nav a{color:white;text-decoration:none;margin:0 10px;font-weight:bold}
main{max-width:900px;margin:auto;padding:18px}
.hero,.card{background:white;border-radius:15px;padding:24px;margin:18px 0;box-shadow:0 4px 18px #0000000d}
.hero{text-align:center;padding:40px 20px}
h2{color:#193967}
.cars,.rates{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px}
.item{background:#edf4ff;padding:18px;border-radius:12px}
.item h3{margin-top:0}
.price{font-size:23px;font-weight:bold;color:#16834a}
label{display:block;margin-top:12px;font-weight:bold}
input,select{width:100%;padding:12px;margin-top:6px;border:1px solid #ccd3df;border-radius:8px;font-size:16px;background:white}
button,.btn{display:inline-block;border:0;background:#16834a;color:white;padding:14px 18px;border-radius:9px;text-decoration:none;font-size:16px;cursor:pointer}
button{width:100%;margin-top:18px}
.btn{margin-top:10px}
.note{font-size:14px;color:#596579;line-height:1.6}
footer{background:#102448;color:white;text-align:center;padding:24px}
@media(max-width:520px){.cars,.rates{grid-template-columns:1fr}header h1{font-size:24px}nav a{display:inline-block;margin:5px}}
</style>
</head>
<body>
<header>
<h1>Kaushal Tours and Travels</h1>
<p>Your Journey, Our Responsibility 🚗</p>
</header>

<nav>
<a href="#cars">Our Cars</a>
<a href="#rates">Rates</a>
<a href="#booking">Book Taxi</a>
</nav>

<main>
<section class="hero">
<h2>Travel Comfortably, Travel Safely</h2>
<p>Book your taxi for local travel, outstation trips and round journeys.</p>
<a class="btn" href="#booking">Book Your Taxi</a>
</section>

<section class="card" id="cars">
<h2>Our Available Cars</h2>
<div class="cars">
<div class="item">
<h3>Hyundai Aura</h3>
<p>Comfortable sedan</p>
<p>AC and Non-AC available</p>
</div>
<div class="item">
<h3>Maruti Suzuki Dzire</h3>
<p>Comfortable sedan</p>
<p>AC and Non-AC available</p>
</div>
</div>
</section>

<section class="card" id="rates">
<h2>Our Taxi Rates</h2>
<div class="rates">
<div class="item">
<h3>❄️ AC Taxi</h3>
<p class="price">₹28/km</p>
</div>
<div class="item">
<h3>🌬️ Non-AC Taxi</h3>
<p class="price">₹25/km</p>
</div>
</div>
<p class="note">Important: Toll tax is extra. Minimum kilometre charges, driver allowance, parking and other applicable charges (if any) will be confirmed before the trip. Final fare depends on your route and trip details.</p>
</section>

<section class="card" id="booking">
<h2>Book Your Taxi on WhatsApp</h2>
<form id="bookingForm">
<label for="customer">Your Name</label>
<input id="customer" required placeholder="Enter your name">

<label for="phone">Your Contact Number</label>
<input id="phone" type="tel" required placeholder="Enter your mobile number">

<label for="pickup">Pickup Location</label>
<input id="pickup" required placeholder="Enter pickup location">

<label for="destination">Drop Location</label>
<input id="destination" required placeholder="Enter destination">

<label for="traveldate">Travel Date</label>
<input id="traveldate" type="date" required>

<label for="cartype">Select Car</label>
<select id="cartype">
<option>Hyundai Aura</option>
<option>Maruti Suzuki Dzire</option>
</select>

<label for="ac">AC Type</label>
<select id="ac">
<option>AC - ₹28/km</option>
<option>Non-AC - ₹25/km</option>
</select>

<label for="trip">Trip Type</label>
<select id="trip">
<option>One Way</option>
<option>Round Trip</option>
</select>

<label for="extra">Additional Details (Optional)</label>
<input id="extra" placeholder="Passengers or other requirements">

<button type="submit">Send Booking on WhatsApp</button>
</form>
<p class="note">Your request will open in WhatsApp. Your booking is not confirmed until the fare and trip details are agreed with us.</p>
</section>

<section class="card">
<h2>Contact Us</h2>
<p>Kaushal Tours and Travels</p>
<p>WhatsApp / Phone: +91 8976643386</p>
<a class="btn" href="https://wa.me/918976643386">Chat with Us on WhatsApp</a>
</section>
</main>

<footer>
<p>© Kaushal Tours and Travels</p>
<p>Thank you for choosing us!</p>
</footer>

<script>
document.getElementById("bookingForm").addEventListener("submit",function(event){
event.preventDefault();
const get=id=>document.getElementById(id).value.trim();
const message=
"NEW TAXI BOOKING REQUEST\n"+
"Business: Kaushal Tours and Travels\n"+
"Customer: "+get("customer")+"\n"+
"Customer Contact: "+get("phone")+"\n"+
"Pickup: "+get("pickup")+"\n"+
"Drop: "+get("destination")+"\n"+
"Travel Date: "+get("traveldate")+"\n"+
"Car: "+get("cartype")+"\n"+
"AC Type: "+get("ac")+"\n"+
"Trip Type: "+get("trip")+"\n"+
"Additional Details: "+(get("extra")||"None")+"\n"+
"Toll tax extra. Please confirm final fare.";
window.open("https://wa.me/918976643386?text="+encodeURIComponent(message),"_blank");
});
</script>
</body>
</html>
