<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MeetMe - Profile Page</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #6a11cb, #2575fc);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }
        .container {
            background: white;
            border-radius: 10px;
            display: flex;
            max-width: 800px;
            overflow: hidden;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.2);
            flex-direction: column;
            text-align: center;
            position: relative;
        }
        .sky {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 120px;
            background: linear-gradient(to bottom, #87CEEB, transparent);
            overflow: hidden;
        }
        .cloud {
            position: absolute;
            background: white;
            width: 80px;
            height: 50px;
            border-radius: 50%;
            opacity: 0.8;
            box-shadow: 10px 10px 30px rgba(0, 0, 0, 0.1);
            animation: moveClouds 15s linear infinite;
        }
        .cloud:nth-child(1) { top: 20px; left: 10%; animation-duration: 20s; }
        .cloud:nth-child(2) { top: 40px; left: 50%; animation-duration: 18s; }
        .cloud:nth-child(3) { top: 10px; left: 80%; animation-duration: 25s; }

        .bird {
            position: absolute;
            top: 50px;
            left: -100px;
            width: 40px;
            height: 40px;
            background: url('https://upload.wikimedia.org/wikipedia/commons/4/41/Bird_icon.svg') no-repeat center;
            background-size: contain;
            animation: flyBirds 10s linear infinite;
        }

        @keyframes moveClouds {
            from { transform: translateX(-100px); }
            to { transform: translateX(100vw); }
        }

        @keyframes flyBirds {
            from { transform: translateX(-100px) translateY(-10px); }
            to { transform: translateX(100vw) translateY(10px); }
        }

        .profile-images {
            display: flex;
            gap: 20px;
            padding: 20px;
            justify-content: center;
        }
        .profile-images img {
            width: 100px;
            height: 100px;
            object-fit: cover;
            border-radius: 10px;
            border: 2px solid #2575fc;
        }
        .profile-info {
            padding: 30px;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }
        .title {
            color: gray;
            font-size: 14px;
        }
        .details {
            margin-top: 15px;
        }
        .details p {
            margin: 10px 0;
            font-size: 14px;
        }
        .details i {
            margin-right: 10px;
            color: #2575fc;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="sky">
            <div class="cloud"></div>
            <div class="cloud"></div>
            <div class="cloud"></div>
            <div class="bird"></div>
        </div>
        <div class="profile-images">
            <img src="public/0.jpg" alt="Profile Image 1">
            <img src="public/1.jpg" alt="Profile Image 2">
            <img src="public/5.jpg" alt="Profile Image 3">
            <img src="public/2.jpg"Profile Image 4">
            <img src="public/3.jpg" alt="Profile Image 5">
        </div>
        <div class="profile-info">
            <p>Hello Everyone, I am</p>
           <h1>John Kim Taborete</h1>
                <p><i class="fas"></i> SANTO TOMAS NATIONAL HIGH SCHOOL </p>
            <p>Make the Most of the Day with Friends</p>
            <p>Life moves fast, and sometimes we forget to enjoy the present moment. But true happiness comes from embracing today, especially when we share it with others.</p>
            <p>Our group is more than just friends—we support and care for each other. We study together, help each other grow, and share fun moments along the way. Whether it’s working on school tasks, setting small goals, or simply laughing together, every day is a chance to learn and bond.</p>
            <div class="details">

                <p><i class="fas fa-calendar-alt"></i> 28th December, 2006</p>
                <p><i class="fas fa-phone"></i> 09756074379</p>
                <p><i class="fas fa-envelope"></i> johnkimtaborete@example.com</p>
                <p><i class="fas fa-map-marker-alt"></i> Amakan 20-D, Barangay Tibal-og, Sto. Tomas, Davao del Norte</p>
            </div>
        </div>
    </div>
</body>
</html>
