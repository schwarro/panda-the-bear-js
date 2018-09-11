<!-- Exercise 1 -->

var profileImage = document.querySelector(".profile-image");
profileImage.src = "https://placebear.com/400/400";

var skyImage = document.querySelector(".photography");
skyImage.src = "https://placebear.com/325/225";

var title = document.querySelector("h1");
title.innerHTML = "Rob";
title.style.fontFamily = "monospace"

var employment = document.querySelector("#employment h3.info-title");
employment.textContent = "Previous Employment";

var body = document.querySelector("body");
body.style.color = "yellow";

var highlights = document.querySelectorAll(".highlight");
for (var i = 0; i < Highlights.length; i++) {
  highlights[i].style.color = "red";
}

var roundIcons = document.querySelectorAll("a.action-icon-bg");
for (var i = 0; i < roundIcons.length; i++) {
  roundIcons[i].style.backgroundColor = 'black';
}

var placeHolderName = document.querySelector ( "#name");
placeHolderName.placeholder = "identify yourself";

var placeHolderMessage = document.querySelector ("#message");
placeHolderMessage.placeholder = "state your business";

var placeHolderName = document.querySelector ( "#name");
placeHolderName.setAttribute("value", "your nemisis");

var placeHolderEmail = document.querySelector ( "#email");

placeHolderEmail.setAttribute("value", "koalathebear@gmail.com");

var placeHolderSubmit = document.querySelector ("#submit");
placeHolderSubmit.setAttribute("value", "En garde!");
placeHolderSubmit.setAttribute("disabled", true);

var info = document.querySelectorAll(".bio-info");
for (var i = 0; i < info.length; i++) {info[i].textContent = "";}

<!-- Exercise 2 -->
var timeTravel = document.querySelector("#time-travel");
timeTravel.parentNode.removeChild(timeTravel);

var pikachu = document.querySelector("#right-image img");
var clonePikachu = pikachu.cloneNode(true);
for (var i = 0; i < 10; i++) {
  var pikachu = document.querySelector("#right-image img");
  var clonePikachu = pikachu.cloneNode(true);
  document.querySelector(".portfolio-container").appendChild(clonePikachu);
};

var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
var bio = document.querySelector(".bio-info");
bio.appendChild(listItem);
var currentDate = new Date();
var rightSpan = document.createElement('span');
var updatedOn = document.createTextNode(currentDate);
rightSpan.appendChild(updatedOn);
listItem.appendChild(rightSpan);
