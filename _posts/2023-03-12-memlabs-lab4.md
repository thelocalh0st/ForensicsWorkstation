---
layout: post
author: sujay adkesar
tags: [memoryforensics, lab4, Obsession]
---


<br>
<div class="eleven">
  <h1 style="color:cyan;">Lab 4 - Obsession</h1>
</div>
<br>
## Challenge Description

My system was recently compromised. The Hacker stole a lot of information but he also deleted a very important file of mine. I have no idea on how to recover it. The only evidence we have, at this point of time is this memory dump. Please help me.

Note: This challenge is composed of only 1 flag.

The flag format for this lab is: inctf{s0me_l33t_Str1ng}

Challenge file: <a href="https://mega.nz/#!Tx41jC5K!ifdu9DUair0sHncj5QWImJovfxixcAY-gt72mCXmYrE">Google drive</a>

<br>
<iframe style="display: block; margin: auto;"width="560" height="315" src="https://www.youtube.com/embed/MqN2yxsSn9U?si=zBkMfzn4jtqumDUc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<br>

## Tasks

<!-- Question 1 -->

<form onsubmit="verifyAnswer(); return false;">
  <label for="answer">1] Enter the OS of the system by analyzing the profile using volatility </label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <g>
        <path d="M55.146 51.887 41.588 37.786A22.926 22.926 0 0 0 46.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 0 0 .083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z" fill="currentColor" data-original="#000000" class=""></path>
      </g>
    </svg>
  </label>
  <button type="submit">
  <div class="svg-wrapper-1">
    <div class="svg-wrapper">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path fill="none" d="M0 0h24v24H0z"></path>
        <path fill="currentColor" d="M1.946 9.315c-.522-.174-.527-.455.01-.634l19.087-6.362c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8-8 6-8.054-2.685z"></path>
      </svg>
    </div>
  </div>
  <span>Submit</span>
</button>
</form>

<div id="verificationResult"></div>

<script>
  function verifyAnswer() {
    var userAnswer = document.getElementById("answer").value;
    var correctAnswer = "Win7SP1x86_23418";
    var resultDisplay = document.getElementById("verificationResult");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 2 -->

<form onsubmit="verifyAnswer2(); return false;">
  <label for="answer2">2] Which file was deleted by the hackers ?  </label>
<label class="search-label">
    <input type="text" name="text" class="input" id="answer2" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <g>
        <path d="M55.146 51.887 41.588 37.786A22.926 22.926 0 0 0 46.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 0 0 .083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z" fill="currentColor" data-original="#000000" class=""></path>
      </g>
    </svg>
  </label>
 <button type="submit">
  <div class="svg-wrapper-1">
    <div class="svg-wrapper">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path fill="none" d="M0 0h24v24H0z"></path>
        <path fill="currentColor" d="M1.946 9.315c-.522-.174-.527-.455.01-.634l19.087-6.362c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8-8 6-8.054-2.685z"></path>
      </svg>
    </div>
  </div>
  <span>Submit</span>
</button>
</form>

<div id="verificationResult2"></div>

<script>
  function verifyAnswer2() {
    var userAnswer = document.getElementById("answer2").value;
    var correctAnswer = "Important.txt";
    var resultDisplay = document.getElementById("verificationResult2");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 3 -->

<form onsubmit="verifyAnswer3(); return false;">
  <label for="answer3">3] What does MFT Stands for ?  (Use Lowercase Letters)</label>
<label class="search-label">
    <input type="text" name="text" class="input" id="answer3" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <g>
        <path d="M55.146 51.887 41.588 37.786A22.926 22.926 0 0 0 46.984 23c0-12.682-10.318-23-23-23s-23 10.318-23 23 10.318 23 23 23c4.761 0 9.298-1.436 13.177-4.162l13.661 14.208c.571.593 1.339.92 2.162.92.779 0 1.518-.297 2.079-.837a3.004 3.004 0 0 0 .083-4.242zM23.984 6c9.374 0 17 7.626 17 17s-7.626 17-17 17-17-7.626-17-17 7.626-17 17-17z" fill="currentColor" data-original="#000000" class=""></path>
      </g>
    </svg>
  </label>
<button type="submit">
  <div class="svg-wrapper-1">
    <div class="svg-wrapper">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path fill="none" d="M0 0h24v24H0z"></path>
        <path fill="currentColor" d="M1.946 9.315c-.522-.174-.527-.455.01-.634l19.087-6.362c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8-8 6-8.054-2.685z"></path>
      </svg>
    </div>
  </div>
  <span>Submit</span>
</button>
</form>

<div id="verificationResult3"></div>

<script>
  function verifyAnswer3() {
    var userAnswer = document.getElementById("answer3").value;
    var correctAnswer = "master file table";
    var resultDisplay = document.getElementById("verificationResult3");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<style>


    /* success */
    .wrapper-success {
      margin: 120px;
    }

    .wrapper-success .card {
      width: 720px;
      height: 120px;
      background-color: #fff;
      padding: 10px 20px;
      display: flex;
      justify-content: space-around;
      align-items: center;
      border-left: 5px solid #49d761;
      border-radius: 3px;
      box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    }

    .wrapper-success .card .subject {
      margin-right: 180px;
    }

    .wrapper-success .card .subject p {
      color: #909092;
    }

    .wrapper-success .card .icon {
      font-size: 28px;
      color: #49d761;
    }

    .wrapper-success .card .icon-times {
      font-size: 28px;
      color: #c3c2c7;
      cursor: pointer;
    }
    /* success */





  
  form {
    margin-bottom: 20px;
  }

  label {
    display: block;
    margin-bottom: 5px;
    color: #FFFFFF; /* White color for text */
  }

  .dark-input {
    padding: 8px;
    font-size: 14px;
    width: 200px;
    background-color: #333; /* Dark gray background */
    color: #FFFFFF; /* White text color */
    border: 1px solid #555; /* Slightly lighter gray border */
    border-radius: 5px;
  }

button {
  font-family: inherit;
  font-size: 14px; /* Adjusted font size */
  background: linear-gradient(to bottom, #4dc7d9 0%, #66a6ff 100%);
  color: white;
  padding: 0.6em 1em; /* Adjusted padding */
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
  border-radius: 20px; /* Adjusted border radius */
  box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.2); /* Adjusted box shadow */
  transition: all 0.3s;
}

button:hover {
  transform: translateY(-2px); /* Adjusted translateY */
  box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.3); /* Adjusted box shadow */
}

button:active {
  transform: scale(0.95);
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.2); /* Adjusted box shadow */
}

button span {
  display: block;
  margin-left: 0.2em; /* Adjusted margin */
  transition: all 0.3s;
}

button svg {
  width: 14px; /* Adjusted SVG width */
  height: 14px; /* Adjusted SVG height */
  fill: white;
  transition: all 0.3s;
}

button .svg-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 24px; /* Adjusted wrapper width */
  height: 24px; /* Adjusted wrapper height */
  border-radius: 50%;
  background-color: rgba(255, 255, 255, 0.2);
  margin-right: 0.3em; /* Adjusted margin */
  transition: all 0.3s;
}

button:hover .svg-wrapper {
  background-color: rgba(255, 255, 255, 0.5);
}

button:hover svg {
  transform: rotate(45deg);
}


  .verification-result {
    margin-top: 10px;
    font-weight: bold;
  }


  .search-label {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  position: relative;
  border: 1px solid transparent;
  border-radius: 12px;
  overflow: hidden;
  background: #3D3D3D;
  padding: 9px;
  cursor: text;
}

.search-label:hover {
  border-color: gray;
}

.search-label:focus-within {
  background: #464646;
  border-color: gray;
}

.search-label input {
  outline: none;
  width: 100%;
  border: none;
  background: none;
  color: rgb(162, 162, 162);
}

.search-label input:focus+.slash-icon,
.search-label input:valid+.slash-icon {
  display: none;
}

.search-label input:valid~.search-icon {
  display: block;
}

.search-label input:valid {
  width: calc(100% - 22px);
  transform: translateX(20px);
}

.search-label svg,
.slash-icon {
  position: absolute;
  color: #7e7e7e;
}

.search-icon {
  display: none;
  width: 12px;
  height: auto;
}

.slash-icon {
  right: 7px;
  border: 1px solid #393838;
  background: linear-gradient(-225deg, #343434, #6d6d6d);
  border-radius: 3px;
  text-align: center;
  box-shadow: inset 0 -2px 0 0 #3f3f3f, inset 0 0 1px 1px rgb(94, 93, 93), 0 1px 2px 1px rgba(28, 28, 29, 0.4);
  cursor: pointer;
  font-size: 12px;
  width: 15px;
}

.slash-icon:active {
  box-shadow: inset 0 1px 0 0 #3f3f3f, inset 0 0 1px 1px rgb(94, 93, 93), 0 1px 2px 0 rgba(28, 28, 29, 0.4);
  text-shadow: 0 1px 0 #7e7e7e;
  color: transparent;
}
</style>
