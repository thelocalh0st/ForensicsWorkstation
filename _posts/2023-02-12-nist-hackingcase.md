---
layout: post
author: sujay adkesar
tags: [CFReDS, NIST, Hacking Case]
---


<br>
<div class="eleven">
  <h1 style="color:cyan;">CFReDS NIST Hacking Case </h1>
</div>

## Scenario <br>

### [cfreds.nist.gov](https://cfreds.nist.gov/)
On `09/20/04` , a `Dell CPi notebook computer`, serial # VLQLW, was found abandoned along with a wireless PCMCIA card and an external homemade 802.11b antennae. It is suspected that this computer was used for hacking purposes, although cannot be tied to a hacking suspect, `G=r=e=g S=c=h=a=r=d=t`. (The equal signs are just to prevent web crawlers from indexing this name; there are no equal signs in the image files.)  Schardt also goes by the online nickname of “Mr. Evil” and some of his associates have said that he would park his vehicle within range of Wireless Access Points (like Starbucks and other T-Mobile Hotspots) where he would then intercept internet traffic, attempting to get credit card numbers, usernames & passwords.

 Find any hacking software, evidence of their use, and any data that might have been generated. Attempt to tie the computer to the suspect,   `G=r=e=g S=c=h=a=r=d=t`

 A DD image (in seven parts: [1](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.001), [2](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.002), [3](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.003), [4](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.004), [5](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.005), [6](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.006), [7](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.007), [8](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.008), and [notes](https://cfreds-archive.nist.gov/images/hacking-dd/SCHARDT.LOG)) and a [EnCase image (second part)](https://cfreds-archive.nist.gov/images/4Dell%20Latitude%20CPi.E01) of the abandoned computer have already been made.

<br>

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.tees.ac.uk%2FImages%2FCommonImages%2Fprospectus%2Fcourse_images%2Fmain%2Fdigital_forensics.jpg&f=1&nofb=1&ipt=efad171612896529a00bcb05b6bd07bbe217058dbda789699914c434602eeaab&ipo=images)

<br>

## Tasks

<!-- Question 1 -->

<form onsubmit="verifyAnswer(); return false;">
  <label for="answer">1. What is the image hash? Does the acquisition and verification hash match? </label>
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
    var correctAnswer = "aee4fcd9301c03b3b054623ca261959a";
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
  <label for="answer2">2. What operating system was used on the computer? </label>
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
    var correctAnswer = "Windows XP";
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
  <label for="answer3">3. When was the install date?</label>
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
    var correctAnswer = "08/19/04 05:48:27PM";
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


<!-- Question 4 -->
<form onsubmit="verifyAnswer4(); return false;">
  <label for="answer4">4. What is the timezone settings?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer4" required="" placeholder="Type here...">
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

<div id="verificationResult4"></div>

<script>
  function verifyAnswer4() {
    var userAnswer = document.getElementById("answer4").value;
    var correctAnswer = "Central Daylight Time (-05hrs GMT)";
    var resultDisplay = document.getElementById("verificationResult4");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 5 -->
<form onsubmit="verifyAnswer5(); return false;">
  <label for="answer5">5. Who is the registered owner?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer5" required="" placeholder="Type here...">
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

<div id="verificationResult5"></div>

<script>
  function verifyAnswer5() {
    var userAnswer = document.getElementById("answer5").value;
    var correctAnswer = "G=r=e=g S=c=h=a=r=d=t";
    var resultDisplay = document.getElementById("verificationResult5");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 6 -->
<form onsubmit="verifyAnswer6(); return false;">
  <label for="answer6">6. What is the computer account name?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer6" required="" placeholder="Type here...">
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

<div id="verificationResult6"></div>

<script>
  function verifyAnswer6() {
    var userAnswer = document.getElementById("answer6").value;
    var correctAnswer = "N-1A9ODN6ZXK4LQ";
    var resultDisplay = document.getElementById("verificationResult6");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 7 -->
<form onsubmit="verifyAnswer7(); return false;">
  <label for="answer7">7. What is the primary domain name?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer7" required="" placeholder="Type here...">
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

<div id="verificationResult7"></div>

<script>
  function verifyAnswer7() {
    var userAnswer = document.getElementById("answer7").value;
    var correctAnswer = "Evil";
    var resultDisplay = document.getElementById("verificationResult7");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>

<!-- Question 8 -->
<form onsubmit="verifyAnswer8(); return false;">
  <label for="answer8">8. When was the last recorded computer shutdown date/time?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer8" required="" placeholder="Type here...">
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

<div id="verificationResult8"></div>

<script>
  function verifyAnswer8() {
    var userAnswer = document.getElementById("answer8").value;
    var correctAnswer = "08/27/04 10:46:33AM";
    var resultDisplay = document.getElementById("verificationResult8");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>

<!-- Question 9 -->
<form onsubmit="verifyAnswer9(); return false;">
  <label for="answer9">9. How many accounts are recorded (total number)?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer9" required="" placeholder="Type here...">
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
          path fill="none" d="M0 0h24v24H0z"></path>
          <path fill="currentColor" d="M1.946 9.315c-.522-.174-.527-.455.01-.634l19.087-6.362c.529-.176.832.12.684.638l-5.454 19.086c-.15.529-.455.547-.679.045L12 14l6-8-8 6-8.054-2.685z"></path>
        </svg>
      </div>
    </div>
    <span>Submit</span>
  </button>
</form>

<div id="verificationResult9"></div>

<script>
  function verifyAnswer9() {
    var userAnswer = document.getElementById("answer9").value;
    var correctAnswer = "5";
    var resultDisplay = document.getElementById("verificationResult9");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 10 -->
<form onsubmit="verifyAnswer10(); return false;">
  <label for="answer10">10. What is the account name of the user who mostly uses the computer?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer10" required="" placeholder="Type here...">
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

<div id="verificationResult10"></div>

<script>
  function verifyAnswer10() {
    var userAnswer = document.getElementById("answer10").value;
    var correctAnswer = "Mr. Evil";
    var resultDisplay = document.getElementById("verificationResult10");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 11 -->
<form onsubmit="verifyAnswer11(); return false;">
  <label for="answer11">11. Who was the last user to logon to the computer?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer11" required="" placeholder="Type here...">
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

<div id="verificationResult11"></div>

<script>
  function verifyAnswer11() {
    var userAnswer = document.getElementById("answer11").value;
    var correctAnswer = "Mr. Evil";
    var resultDisplay = document.getElementById("verificationResult11");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>



<!-- Question 12 -->
<form onsubmit="verifyAnswer12(); return false;">
  <label for="answer12">12. What file reveals that G=r=e=g S=c=h=a=r=d=t is Mr. Evil and is also the administrator of this computer? What software program does this file relate to?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer12" required="" placeholder="*:\******* *****\****@***">
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

<div id="verificationResult12"></div>

<script>
  function verifyAnswer12() {
    var userAnswer = document.getElementById("answer12").value;
    var correctAnswer = "C:\\Program Files\\Look@LAN";
    var resultDisplay = document.getElementById("verificationResult12");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 13 -->
<form onsubmit="verifyAnswer13(); return false;">
  <label for="answer13">13. List the network cards used by this computer</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer13" required="" placeholder="Type here...">
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

<div id="verificationResult13"></div>

<!-- Include the string-similarity library -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/string-similarity/3.0.0/string-similarity.min.js"></script>

<script>
  function verifyAnswer13() {
    var userAnswer = document.getElementById("answer13").value;
    var correctAnswer = "Xircom CardBus Ethernet 100 + Modem 56 (Ethernet Interface)\nCompaq WL110 Wireless LAN PC Card";
    var resultDisplay = document.getElementById("verificationResult13");

    // Calculate the similarity ratio
    var similarityRatio = stringSimilarity.compareTwoStrings(userAnswer, correctAnswer);

    // Set a threshold for similarity
    var similarityThreshold = 0.8; // Adjust this threshold as needed

    if (similarityRatio >= similarityThreshold) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 14 -->
<form onsubmit="verifyAnswer14(); return false;">
  <label for="answer14">14. This same file reports the IP address and MAC address of the computer. What are they?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer14" required="" placeholder="***.***.*.***,************">
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

<div id="verificationResult14"></div>

<script>
  function verifyAnswer14() {
    var userAnswer = document.getElementById("answer14").value;
    var correctAnswer = "192.168.1.111,0010a4933e09";
    var resultDisplay = document.getElementById("verificationResult14");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>

<!-- Question 15 -->
<form onsubmit="verifyAnswer15(); return false;">
  <label for="answer15">15. In the above answer, the first 3 hex characters of the MAC address report the vendor of the card. Which NIC card was used during the installation and set-up for LOOK@LAN?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer15" required="" placeholder="Type here...">
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

<div id="verificationResult15"></div>

<script>
  function verifyAnswer15() {
    var userAnswer = document.getElementById("answer15").value;
    var correctAnswer = "Xircom";
    var resultDisplay = document.getElementById("verificationResult15");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 16 -->
<form onsubmit="verifyAnswer16(); return false;">
  <label for="answer16">16. Find 6 installed programs that may be used for hacking.</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer16" required="" placeholder="Type here...">
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

<div id="verificationResult16"></div>

<!-- Include the string-similarity library -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/string-similarity/3.0.0/string-similarity.min.js"></script>

<script>
  function verifyAnswer16() {
    var userAnswer = document.getElementById("answer16").value;
    var correctAnswer = "Cain & Abel v2.5 beta45 (password sniffer & cracker)\nEthereal (packet sniffer)\n123 Write All Stored Passwords (finds passwords in registry)\nAnonymizer (hides IP tracks when browsing)\nCuteFTP (FTP software)\nLook&LAN_1.0 (network discovery tool)\nNetStumbler (wireless access point discovery tool)";
    var resultDisplay = document.getElementById("verificationResult16");

    // Calculate the similarity ratio
    var similarityRatio = stringSimilarity.compareTwoStrings(userAnswer, correctAnswer);

    // Set a threshold for similarity
    var similarityThreshold = 0.8; // Adjust this threshold as needed

    if (similarityRatio >= similarityThreshold) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>

<!-- Question 17 -->
<form onsubmit="verifyAnswer17(); return false;">
  <label for="answer17">17. What is the SMTP email address for Mr. Evil?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer17" required="" placeholder="Type here...">
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

<div id="verificationResult17"></div>

<script>
  function verifyAnswer17() {
    var userAnswer = document.getElementById("answer17").value;
    var correctAnswer = "whoknowsme@sbcglobal.net";
    var resultDisplay = document.getElementById("verificationResult17");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 18 -->
<form onsubmit="verifyAnswer18(); return false;">
  <label for="answer18">18. What are the NNTP (news server) settings for Mr. Evil?</label>
  <label class="search-label">
    <input name="text" class="input" id="answer18" required="" placeholder="Type here...">
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

<div id="verificationResult18"></div>

<script>
  function verifyAnswer18() {
    var userAnswer = document.getElementById("answer18").value;
    var correctAnswer = "News.dallas.sbcglobal.net";
    var resultDisplay = document.getElementById("verificationResult18");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>

<!-- Question 19 -->
<form onsubmit="verifyAnswer19(); return false;">
  <label for="answer19">19. What two installed programs show this information?</label>
  <label class="search-label">
    <input name="text" class="input" id="answer19" required="" placeholder="** ******* *******,***** *****">
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

<div id="verificationResult19"></div>

<script>
  function verifyAnswer19() {
    var userAnswer = document.getElementById("answer19").value;
    var correctAnswer = "MS Outlook Express,Forte Agent";
    var resultDisplay = document.getElementById("verificationResult19");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<!-- Question 20 -->
<form onsubmit="printAnswer20(); return false;">
  <label for="answer20">20. List 5 newsgroups that Mr. Evil has subscribed to?</label>
  <label class="search-label">
    <input name="text" class="input" id="answer20" required="" placeholder="Type here...">
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

<script>
  function printAnswer20() {
    var correctAnswer = "Alt.2600.phreakz\nAlt.2600\nAlt.2600.cardz\nAlt.2600codez\nAlt.2600.crackz\nAlt.2600.moderated\nAlt.binaries.hacking.utilities\nAlt.stupidity.hackers.malicious\nFree.binaries.hackers.malicious\nFree.binaries.hacking.talentless.troll_haven\nFree.binaries.hacking.talentless.troll-haven\nalt.nl.binaries.hack\nfree.binaries.hacking.beginner\nfree.binaries.hacking.computers\nfree.binaries.hacking.utilities\nfree.binaries.hacking.websites\nalt.binaries.hacking.computers\nalt.binaries.hacking.websites\nalt.dss.hack\nalt.binaries.hacking.beginner\nalt.hacking\nalt.2600.programz\nalt.2600.hackerz";
    var resultDisplay = document.getElementById("verificationResult20");
    
    resultDisplay.textContent = "Answer: " + correctAnswer;
    resultDisplay.style.color = "green";
  }
</script>

<div id="verificationResult20"></div>


<!-- Question 21 -->
<form onsubmit="printAnswer21(); return false;">
  <label for="answer21">21.A popular IRC (Internet Relay Chat) program called MIRC was installed. What are
the user settings that was shown when the user was online and in a chat channel? </label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer21" required="" placeholder="user=**** **,email=****@**.**,nick=**,anick=***********">
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



<script>
  function printAnswer21() {
    var userAnswer = document.getElementById("answer21").value;
    var correctAnswer = "user=Mini Me,email=none@of.ya,nick=Mr,anick=mrevilrulez";
    var resultDisplay = document.getElementById("verificationResult21");

    if (userAnswer === correctAnswer) {
      resultDisplay.textContent = "Correct! You may proceed.";
      resultDisplay.style.color = "green";
    } else {
      resultDisplay.textContent = "Incorrect. Please try again.";
      resultDisplay.style.color = "red";
    }
  }
</script>


<div id="verificationResult21"></div>



<!-- Question 22 -->
<form onsubmit="printAnswer22(); return false;">
  <label for="answer22">21. A popular IRC (Internet Relay Chat) program called MIRC was installed. What are
the user settings that was shown when the user was online and in a chat channel? 
</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer22" required="" placeholder="user=**** **,email=****@**.**,nick=**,anick=***********">
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


<script>
  function printAnswer22() {
    var correctAnswer = "\nUshells.undernet.log\nElite.hackers.undernet.log\nMp3xserv.undernet.log\nChataholics.undernet.log\nCybercafé.undernet.log\nM5tar.undernet.log\nThedarktower.afternet.log\nFunny.undernet.log\nLuxshell.undernet.log\nEvilfork.efnet.log\nIso-warez.efnet.log\nHouston.undernet.log";
    var resultDisplay = document.getElementById("verificationResult20");
    
    resultDisplay.textContent = "Answer: " + correctAnswer;
    resultDisplay.style.color = "green";
  }
</script>

<div id="verificationResult22"></div>

<!-- Question 23 -->

<form onsubmit="verifyAnswer23(); return false;">
  <label for="answer23">23. Ethereal, a popular “sniffing” program that can be used to intercept wired and wireless internet packets was also found to be installed. When TCP packets are collected and re-assembled, the default save directory is that users \My Documents directory. What is the name of the file that contains the intercepted data?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer23" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult23"></div>

<script>
  function verifyAnswer23() {
    var userAnswer23 = document.getElementById("answer23").value;
    var correctAnswer23 = "Interception";
    var resultDisplay23 = document.getElementById("verificationResult23");

    if (userAnswer23 === correctAnswer23) {
      resultDisplay23.textContent = "Correct! You may proceed.";
      resultDisplay23.style.color = "green";
    } else {
      resultDisplay23.textContent = "Incorrect. Please try again.";
      resultDisplay23.style.color = "red";
    }
  }
</script>


<!-- Question 24 -->

<form onsubmit="verifyAnswer24(); return false;">
  <label for="answer24">24. Viewing the file in a text format reveals much information about who and what was intercepted. What type of wireless computer was the victim (person who had his internet surfing recorded) using?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer24" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult24"></div>

<script>
  function verifyAnswer24() {
    var userAnswer24 = document.getElementById("answer24").value;
    var correctAnswer24 = "Windows CE (Pocket PC)";
    var resultDisplay24 = document.getElementById("verificationResult24");

    if (userAnswer24 === correctAnswer24) {
      resultDisplay24.textContent = "Correct! You may proceed.";
      resultDisplay24.style.color = "green";
    } else {
      resultDisplay24.textContent = "Incorrect. Please try again.";
      resultDisplay24.style.color = "red";
    }
  }
</script>

<!-- Question 25 -->

<form onsubmit="verifyAnswer25(); return false;">
  <label for="answer25">25. What websites was the victim accessing?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer25" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult25"></div>

<script>
  function verifyAnswer25() {
    var userAnswer25 = document.getElementById("answer25").value;
    var correctAnswer25 = "Mobile.msn.com MSN (Hotmail) Email";
    var resultDisplay25 = document.getElementById("verificationResult25");

    if (userAnswer25 === correctAnswer25) {
      resultDisplay25.textContent = "Correct! You may proceed.";
      resultDisplay25.style.color = "green";
    } else {
      resultDisplay25.textContent = "Incorrect. Please try again.";
      resultDisplay25.style.color = "red";
    }
  }
</script>


<!-- Question 26 -->

<form onsubmit="verifyAnswer26(); return false;">
  <label for="answer26">26. Search for the main user's web-based email address. What is it?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer26" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult26"></div>

<script>
  function verifyAnswer26() {
    var userAnswer26 = document.getElementById("answer26").value;
    var correctAnswer26 = "mrevilrulez@yahoo.com";
    var resultDisplay26 = document.getElementById("verificationResult26");

    if (userAnswer26 === correctAnswer26) {
      resultDisplay26.textContent = "Correct! You may proceed.";
      resultDisplay26.style.color = "green";
    } else {
      resultDisplay26.textContent = "Incorrect. Please try again.";
      resultDisplay26.style.color = "red";
    }
  }
</script>


<!-- Question 27 -->

<form onsubmit="verifyAnswer27(); return false;">
  <label for="answer27">27. Yahoo Mail, a popular web-based email service, saves copies of the email under what file name?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer27" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult27"></div>

<script>
  function verifyAnswer27() {
    var userAnswer27 = document.getElementById("answer27").value;
    var correctAnswer27 = "Showletter[1].htm";
    var resultDisplay27 = document.getElementById("verificationResult27");

    if (userAnswer27 === correctAnswer27) {
      resultDisplay27.textContent = "Correct! You may proceed.";
      resultDisplay27.style.color = "green";
    } else {
      resultDisplay27.textContent = "Incorrect. Please try again.";
      resultDisplay27.style.color = "red";
    }
  }
</script>

<!-- Question 28 -->

<form onsubmit="verifyAnswer28(); return false;">
  <label for="answer28">28. How many executable files are in the recycle bin?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer28" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult28"></div>

<script>
  function verifyAnswer28() {
    var userAnswer28 = document.getElementById("answer28").value;
    var correctAnswer28 = "4";
    var resultDisplay28 = document.getElementById("verificationResult28");

    if (userAnswer28 === correctAnswer28) {
      resultDisplay28.textContent = "Correct! You may proceed.";
      resultDisplay28.style.color = "green";
    } else {
      resultDisplay28.textContent = "Incorrect. Please try again.";
      resultDisplay28.style.color = "red";
    }
  }
</script>


<!-- Question 29 -->

<form onsubmit="verifyAnswer29(); return false;">
  <label for="answer29">29. Are these files really deleted?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer29" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult29"></div>

<script>
  function verifyAnswer29() {
    var userAnswer29 = document.getElementById("answer29").value;
    var correctAnswer29 = "No";
    var resultDisplay29 = document.getElementById("verificationResult29");

    if (userAnswer29 === correctAnswer29) {
      resultDisplay29.textContent = "Correct! You may proceed.";
      resultDisplay29.style.color = "green";
    } else {
      resultDisplay29.textContent = "Incorrect. Please try again.";
      resultDisplay29.style.color = "red";
    }
  }
</script>


<!-- Question 30 -->

<form onsubmit="verifyAnswer30(); return false;">
  <label for="answer30">30. How many files are actually reported to be deleted by the file system?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer30" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult30"></div>

<script>
  function verifyAnswer30() {
    var userAnswer30 = document.getElementById("answer30").value;
    var correctAnswer30 = "3";
    var resultDisplay30 = document.getElementById("verificationResult30");

    if (userAnswer30 === correctAnswer30) {
      resultDisplay30.textContent = "Correct! You may proceed.";
      resultDisplay30.style.color = "green";
    } else {
      resultDisplay30.textContent = "Incorrect. Please try again.";
      resultDisplay30.style.color = "red";
    }
  }
</script>


<!-- Question 31 -->

<form onsubmit="verifyAnswer31(); return false;">
  <label for="answer31">31. Perform an Anti-Virus check. Are there any viruses on the computer?</label>
  <label class="search-label">
    <input type="text" name="text" class="input" id="answer31" required="" placeholder="Type here...">
    <kbd class="slash-icon">/</kbd>
    <svg class="search-icon" xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" width="512" height="512" x="0" y="0" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 512 512" xml:space="preserve">
      <!-- Search icon path -->
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

<div id="verificationResult31"></div>

<script>
  function verifyAnswer31() {
    var userAnswer31 = document.getElementById("answer31").value;
    var correctAnswer31 = "Yes";
    var resultDisplay31 = document.getElementById("verificationResult31");

    if (userAnswer31 === correctAnswer31) {
      resultDisplay31.textContent = "Correct! You may proceed.";
      resultDisplay31.style.color = "green";
    } else {
      resultDisplay31.textContent = "Incorrect. Please try again.";
      resultDisplay31.style.color = "red";
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
