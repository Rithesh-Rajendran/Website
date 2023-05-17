<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="style.css">
   <style>
        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
        }

 .left-column {
    position: relative;
    width: 25%;
    padding: 20px;
    background-image: linear-gradient(to bottom, #31aeff, #f5f5f5, #f5f5f5, #f5f5f5, #f5f5f5);
    border-top-left-radius: 8%;
    border-top-right-radius: 30%;
    border-bottom-left-radius: 0%;
    border-bottom-right-radius: 50%;
    overflow: hidden; /* Clip the curved design shape */
}

.left-column::before {
    content: "";
    position: absolute;
    top: 0;
    left: -50%;
    width: 200%;
    height: 100%;
    background-color: #87ceeb; /* Light blue color */
    border-radius: 0% 0% 50% 0% / 0% 0% 50% 0%; /* Right curve at the top */
    z-index: -1; /* Move the shape behind the text content */
}

.left-column-content {
    position: relative;
    z-index: 2; /* Ensure the text content is on top */
    color: #fff; /* Set the text color to white */
    padding: 20px;
}

.left-column-text {
    position: relative;
}
 right-column {
            width: 75%;
            padding: 20px;
        }
        .section {
            margin-bottom: 20px;
        }

        .section-title {
            font-weight: bold;
            margin-bottom: 10px;
        }

        .section-content {
            margin-left: 20px;
        }

        .strengths,
        .declaration {
            margin-top: 20px;
        }
      .button-bar {
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #ffff;
      }
     
.button-bar button {
  border: none;
  padding: 10px 20px;
  background-color: #f8f8f8;
  color: #333;
  font-size: 16px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.button-bar button.active {
  background-color: #333;
  color: #fff;
}
/* Style for left content */
#left-content {
  display: block;
}

/* Style for skills */
.skill {
  margin: 10px 0;
}
.skill-title {
  font-size: 20px;
  margin-right: 20px;
  background-color: rgba(0, 0, 0, 0);
  color: Black;
  padding: 0px;
  display: inline-block;
  border-radius: 0px;
}
.skill-bar {
  width: 600px;
  height: 17px;
  background-color: #ddd;
  border-radius: 10px;
  position: relative;
  overflow: hidden;
  margin-bottom: 10px;
  
}

.skill-progress {
  height: 100%;
  border-radius: 10px;
  background-image: linear-gradient(to bottom, #04AA6D, #048BA8, #0579C9, #0652DD, #1C1A70);
  background-size: 100% 200%;
  background-position: bottom;
  animation: progress 3s ease-out, glitter 2s ease-out infinite;
  position: absolute;
  top: 0;
  left: 0;
  transition: transform 0.1s ease-in-out;
}
.skill-progress:hover {
  transform: translateX(2px);
}

.skill-progress::before {
  content: "";
  position: absolute;
  top: 0;
  left: -50%;
  width: 200%;
  height: 100%;
  background-color: rgba(0, 206, 255, 0.3);
  animation: glow 5s ease-out infinite alternate;
  filter: blur(10px);
}

@keyframes progress {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}

@keyframes glitter {
  0% {
    background-position: bottom;
  }
  100% {
    background-position: top;
  }
}

@keyframes shake {
  0% {
    transform: translateX(0);
  }
  10% {
    transform: translateX(2px);
  }
  20% {
    transform: translateX(-2px);
  }
  30% {
    transform: translateX(2px);
  }
  40% {
    transform: translateX(-2px);
  }
  50% {
    transform: translateX(2px);
  }
  60% {
    transform: translateX(-2px);
  }
  70% {
    transform: translateX(2px);
  }
  80% {
    transform: translateX(-2px);
  }
  90% {
    transform: translateX(2px);
  }
  100% {
    transform: translateX(0);
  }
}

@keyframes glow {
  from {
    opacity: 0.5;
  }
  to {
    opacity: 1;
  }
}
    </style>
</head>
<body>
    <center>
        <h1 style="text-align: center;">Resume</h1>
    </center>

    <div class="container">
        <div class="left-column">
            <img src="https://raw.githubusercontent.com/Rithesh-Rajendran/Website/main/IMG_20210825_162503%20(1).jpg" alt="Profile Photo" style="max-width: 200px; height:200px;">
            <h2>RITHESH R</h2>
            <h2>Technical Engineer</h2>
            <h2 class="section-title">Contact</h2>
            <p class="section-content">
                <strong>PHONE:</strong> 9940188948<br>
                <strong>EMAIL:</strong> ritheshrao12@gmail.com<br>
                <strong>ADDRESS:</strong> 3116, 3rd main road, mathur, M.M.D.A, Chennai-600068.
            </p>
          
             <div class="section">
                <h2 class="section-title">Education</h2>
                <p class="section-content">
                    Apollo Engineering College, Anna University<br>
                    BE CSE 2017 - 2021<br>
                    71%
                </p>
<p class="section-content">
                    Velammal.mat.hr.sec.school<br>
                    HSC 2017<br>
                    68%
                </p>
<p class="section-content">
                    St.thomas.mat.hr.sec.school<br>
                    SSLC 2015<br>
                    81%
                </p>

            </div>

            <div class="section">
                <h2 class="section-title">Languages</h2>
                <p class="section-content">
                    English<br>
                    Hindi<br>
                    Tamil<br>
                    Marathi
                </p>
            </div>

            <div class="section">
                <h2 class="section-title">Hobbies</h2>
                <p class="section-content">
                    Designing<br>
                    Photography<br>
                    Traveling<br>	
                    Circket<br>
                    
                </p>
            </div>
           <div class="section">
               <h2 class="section-title">Soft Skills</h2>
               <p class="section-content">  
                Android Studio<br>
                MS Excel<br>
                Power Point<br>
                Adobe Illustrator<br>
                Adobe Photoshop
               </p>
               </div>

          
               <!--<div class="section">
               <h2 class="section-title">Soft Skills</h2>
               <p class="section-content">  
                • Outstanding customer service and client interfacing skills.<br>
                • Ability to perform excellently on individual projects and cooperatively on teams.<br>
                • High adaptability and capable of handling high workloads.<br>
                • Primary help desk technical assistance and troubleshooting on IT platform.
               </p>
               </div>-->
               </p>
               </div>

        <div class="right-column">
            <h2 class="section-title">Profile</h2>
            <p class="section-content">
               To work with a company which appreciates innovation so that I can enhance my knowledge and skills to give my best for the growth of the company.
            </p>

            <div class="section">
                <h2 class="section-title">Work Experience</h2>
                <p class="section-content">
                    <strong>Redisolve Software</strong><br>
                    System Admin<br>
                    (September 2021 - February 2022)<br><br>

                    <strong>CDTECH Innovation PVT LTD, INDIA</strong><br>
                    Technical Support Engineer<br>
                    (February 2022 - till date)<br><br>

                    • Managing the entire IT System<br>
                    • Developing website and mobile applications based on clients' requirements<br>
                    • Testing software on cloud-based servers<br>
                    • Interacting with vendor support contacts to resolve technical problems with desktop computing equipment, Router and telephone systems.<br>
                    • Managed the design, installation, and management of organization-wide local area network, wide area network, network segment, and internet system<br>
                    • Maintenance and upgrading of computer systems or offering recommendations on upgrades needed.<br>
                    • Maintaining CCTV operations and backup<br>
                    • Support and troubleshooting cloud server related issues.<br>
                    • Implement effective security measures to protect data, software, and hardware • Deliver Tier 1 network ticketing support to resolve all issues for 500+ users<br>
                    • Handling all support calls and Manage engine ticketing system.<br>
                    • Execute the maintenance window changes for multiple locations, performing troubleshooting of routing and switching issues<br>
                    • Providing first-level support services for software and hardware for the end-users.<br>
                    • Wireless Router, switches and Access point installation and Setup.<br>
                    • Installation of client-based windows OS and configure organizational standard applications.<br>
                    • Testing Hardware devices (Internet aggregator, Bonding device, Encoders, Receivers, Android boxes, Routers, Network booster)<br>
                    • Resolving Server and Network related issues<br>
                    • Designed, configured, and installed all Data Center Network Devices to support 1000+ users<br>
                    • Maintained seamless end-to-end communication by delivering support for Video Conferencing System.
                </p>
            </div>

       <div class="section">
    <div class="button-bar">
        <button id="left-btn" class="full-width active">Programing Skills</button>
        <button id="right-btn" class="full-width">Soft Skills</button>
    </div>
    <center><div class="content-wrapper">
        <div id="left-content" class="content">
            <div class="skill">
                <div class="skill-title">HTML</div>
                <div class="skill-bar">
                    <div class="skill-progress" style="width: 95%;"></div>
                </div>
            </div>

    <div class="skill">
      <div class="skill-title">CSS</div>
      <div class="skill-bar">
        <div class="skill-progress" style="width: 85%;"></div>
      </div>
    </div>
         <div class="skill">
        <div class="skill-title">JavaScript</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 70%;"></div>
        </div>
      </div>
   
      <div class="skill">
        <div class="skill-title">PHP</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 80%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Java</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 50%;"></div>
        </div>
      </div>
   
      <div class="skill">
        <div class="skill-title">Python</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 65%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Wordpress</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 95%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">FTP</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 95%;"></div>
        </div>
      </div>
      <div class="skill">
        <div class="skill-title">Linux</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 95%;"></div>
        </div>
      </div>
  </div>
        </div>
        <div id="right-content" class="content" style="display: none;">
            <div id="right-content" class="content">
    <div class="skill">
      <div class="skill-title">Obident</div>
      <div class="skill-bar">
        <div class="skill-progress" style="width: 75%;"></div>
      </div>
    </div>

    <div class="skill">
      <div class="skill-title">React</div>
      <div class="skill-bar">
        <div class="skill-progress" style="width: 65%;"></div>
      </div>
    </div>
    <div class="skill">
        <div class="skill-title">Communication</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 95%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Teamwork</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 90%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Problem Solving</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 85%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Time Management</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 80%;"></div>
        </div>
      </div>

      <div class="skill">
        <div class="skill-title">Leadership</div>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 70%;"></div>
        </div>
  </div>
        </div>
    </div>
</div></center>
              
            <div class="section"> 
	 <h2 class="section-title">Technical Skills</h2>
 		<p class="section-content">        
                • Creating websites<br>
                • Developing Android applications<br>
                • Maintaining cloud servers (Streaming servers. VPN servers)<br>
                • Streaming cloud servers (RTMP, HLS, DASH, HTTPS, SRT, RTSP)<br>
                • Publishing APK in Google and App Store<br>
                • Testing newly developed software's in server<br>
                • Testing Hardware devices (Internet aggregator, Bonding device, Encoders, Receivers, Android
                boxes, Routers, Network boosters)<br>
                • Good knowledge of cloud-based solutions<br>
                • Strong problem-solving ability<br>
                • Basic knowledge of security best practices Installing OS (Ubuntu, Linux, windows)<br>
                • Resolving Server and Network related issues<br>
                • Presenting software and hardware demo to clients. Setting-up servers and configuring on-site.
          </p>
            </div>
			<div class="section"> 
	 <h2 class="section-title">soft Skills</h2>
 		 <p class="section-content">  
                • Outstanding customer service and client interfacing skills.<br>
                • Ability to perform excellently on individual projects and cooperatively on teams.<br>
                • High adaptability and capable of handling high workloads.<br>
                • Primary help desk technical assistance and troubleshooting on IT platform.
               </p>
            </div>

            <div class="section">
                <h2 class="section-title">Internship & Certification</h2>
                <p class="section-content">
                    • Cisco CCNA Certified<br>
                    • Attended Industrial exposure program at wikitechy
					• Java & Manual testing certified under 
                </p>
            </div>


            <div class="section">
                <h2 class="section-title">Declaration</h2>
                <p class="section-content">
                    Thereby declare that the information furnished above is true and correct to my knowledge and belief.<br> 
					<b>RITHESH R</b>
                </p>
            </div>
        </div>
    </div>
<script src="script.js"></script>
<script>
const leftBtn = document.getElementById("left-btn");
const rightBtn = document.getElementById("right-btn");
const leftContent = document.getElementById("left-content");
const rightContent = document.getElementById("right-content");

let isLeftContentDisplayed = true;

function toggleButton(button) {
  // Remove the 'active' class from all buttons
  var buttons = document.querySelectorAll('.button-bar button');
  for (var i = 0; i < buttons.length; i++) {
    buttons[i].classList.remove('active');
  }
  
  // Add the 'active' class to the clicked button
  button.classList.add('active');
}

leftBtn.addEventListener("click", () => {
  if (!isLeftContentDisplayed) {
    leftContent.style.display = "block";
    rightContent.style.display = "none";
    isLeftContentDisplayed = true;
    toggleButton(leftBtn);
  }
});

rightBtn.addEventListener("click", () => {
  if (isLeftContentDisplayed) {
    rightContent.style.display = "block";
    leftContent.style.display = "none";
    isLeftContentDisplayed = false;
    toggleButton(rightBtn);
  }
});
</script>

</body>
</html>
