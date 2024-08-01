'use strict';
//JSON templates for differnt Days [ template name, JSON ]

let schedules;
if (typeof custSched == 'undefined') {
  schedules = [
  `{
    "title"   : "MWF Bell Schedule 1",
    "blocks"  : [
      {  "period" : "Period 1" , "start" : "09:20" , "end" : "10:20" ,
               "alarmsBeforeEnd" : [] } ,
      {  "period" : "Period 2" , "start" : "10:25" , "end" : "11:25" } ,
      {  "period" : "Period 3" , "start" : "11:30" , "end" : "12:30" } ,
      {  "period" : "Period 4" , "start" : "13:00" , "end" : "14:00" } ,
      {  "period" : "Period 5" , "start" : "14:05" , "end" : "15:05" } ,
      {  "period" : "Period 6" , "start" : "15:10" , "end" : "16:10" } ,
         ] ,
        "defaultAlarmsBeforeEnd"   : [ "2:00" ]
  }`,
  `{
    "title"   : "TR Bell Schedule 2",
    "blocks"  : [
      {  "period" : "Period 7" , "start" : "09:20" , "end" : "10:55" ,
             "alarmsBeforeEnd" : [] } ,
      {  "period" : "Period 8" , "start" : "11:00" , "end" : "12:35" } ,
      {  "period" : "Period 9" , "start" : "13:05" , "end" : "14:35" } ,
      {  "period" : "Period 10" , "start" : "14:40" , "end" : "16:10" } ,
        ] ,
        "defaultAlarmsBeforeEnd"   : [ "2:00" ]
  }`
  ];
} else {
  schedules = custSched;
}


function chooseInitOption(key) {

  if (key != 'custom' ) { 
    initializeClock(schedules[key]);
    document.getElementById('customJSONEntry').value = schedules[key];
    document.getElementById(`initOption-${key}`);
  }

  for (let i = 0; i < buttonElements.length; i++) {
    if (i == key) {
      buttonElements[i].classList.add('is-active');
    } else {
      buttonElements[i].classList.remove('is-active');
    }
  }

}

function closeModal() {
  document.getElementById('customJSONContainer').classList.remove('is-active');
  refreshAllTimers();
}

function openModal() {
  document.getElementById('customJSONContainer').classList.add('is-active');
}



//////////////////////////////////////////////////
///////// INITIALIZE THE HTML DOCUMENT ///////////
//////////////////////////////////////////////////


let buttonElements = [];
const placeToPut = document.getElementById('schedOptions');

for (let i = 0; i < schedules.length; i++) {
  //parse the schedule
  const data = JSON.parse(schedules[i]);
  
  //make a new entry into the nav ul
  let newLI = document.createElement('li');
  let newLink = document.createElement('a');
  newLI.appendChild(newLink);
  newLink.addEventListener('click', function() { chooseInitOption(i) });
  newLink.addEventListener('mouseup', function() { return false; });
  newLink.textContent = data.title;

  //append the new entry
  buttonElements.push(newLI)
  placeToPut.appendChild(newLI);
}

function handleAddListeners(stmt, fn) {
  const elementArray = document.querySelectorAll(stmt);
  for (let i = 0; i < elementArray.length; i++) {
    elementArray[i].addEventListener('click', fn);
  }
}

handleAddListeners('.modal-close, .modal-background', closeModal)
handleAddListeners('.open-modal', openModal)

document.getElementById('loadNewJSON').addEventListener('click', function() {
  const textareaField = document.getElementById('customJSONEntry');
  const btn = document.getElementById('loadNewJSON');
  try {
    textareaField.classList.remove('is-danger');
    btn.classList.remove('is-danger')
    initializeClock(textareaField.value);
    chooseInitOption('custom');
    closeModal();
  } catch(e) {
    textareaField.classList.add('is-danger');
    btn.classList.add('is-danger')
    alert(e.message);
  }

});

document.getElementById('loadNewJSON').addEventListener('mouseup', function() { return false; });
