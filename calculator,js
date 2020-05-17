// ==UserScript==
// @name         Incremancer Parts Calculator
// @namespace    http://tampermonkey.net/
// @version      1.0
// @description  Shows more information for the Factory tab
// @author       BananaMonkeyTaco
// @match        https://www.kongregate.com/games/jamesg466/incremancer
// @match        https://incremancer.gti.nz/
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    var partDuplicatorRate = 4/3;
    var stampPressRate = 16/5;
    var conveyorRate = 64/8;
    var splitterCombinerRate = 192/10;
    var batchConverterRate = 512/12;

    setInterval(work, 100);

    function work() {
        //console.log("hi");
        //console.log(document.getElementsByClassName("buttons"));
        //console.log(document.childNodes[1].childNodes[2].childNodes[30].childNodes[3].childNodes[1].childNodes[0].childNodes[3].childNodes[12].childNodes[7].childNodes[9].childNodes[3].childNodes[3].childNodes[1].childNodes[1].childNodes[1].childNodes[3].childNodes[1].childNodes[6].childNodes[3]);
        //console.log(document.getElementsByClassName("stats"));
        //console.log(document.firstElementChild.getElementById("gameiframe").childNodes[0].childNodes[1].childNodes[1]);
        if (document.getElementsByTagName("FACTORY-MENU")[0].childNodes[1].childNodes[10].innerHTML != undefined) {
            var factMenu = document.getElementsByTagName("FACTORY-MENU")[0].childNodes[1].childNodes[10];
            let cost;
            let gain;
            let returnOnInvestment;
            let seconds;
            let minutes;
            let hours;
            let days;
            let newLine;

            //Part Duplicator

            cost = findRealNumber(factMenu.childNodes[4].childNodes[3].innerText);
            gain = partDuplicatorRate * GameModel.partsPCMod;
            returnOnInvestment = cost / gain;
            seconds = Math.floor(returnOnInvestment % 60);
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            minutes = returnOnInvestment % 60;
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            hours = returnOnInvestment % 24;
            returnOnInvestment = Math.floor(returnOnInvestment / 24);
            days = returnOnInvestment;
            newLine = document.createElement("p");
            //newLine.ng-show = "generator.selected";
            newLine.class = "ng-binding ng-hide";
            newLine.innerHTML = "Will pay back in ";
            if (days > 0) {
                if (hours < 10) { hours = "0" + hours; }
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += days + ":" + hours + ":" + minutes + ":" + seconds;
            } else if (hours > 0) {
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += hours + ":" + minutes + ":" + seconds;
            } else if (minutes > 0) {
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += minutes + ":" + seconds;
            } else {
                newLine.textContent += seconds;
            }
            if (factMenu.childNodes[4].childNodes[17] != undefined) {
                factMenu.childNodes[4].removeChild(factMenu.childNodes[4].childNodes[17]);
            }
            factMenu.childNodes[4].appendChild(newLine);

            //Stamp Press

            cost = findRealNumber(factMenu.childNodes[6].childNodes[3].innerText);
            gain = stampPressRate * GameModel.partsPCMod;
            returnOnInvestment = cost / gain;
            seconds = Math.floor(returnOnInvestment % 60);
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            minutes = returnOnInvestment % 60;
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            hours = returnOnInvestment % 24;
            returnOnInvestment = Math.floor(returnOnInvestment / 24);
            days = returnOnInvestment;
            newLine = document.createElement("p");
            //newLine.ng-show = "generator.selected";
            newLine.class = "ng-binding ng-hide";
            newLine.innerHTML = "Will pay back in ";
            if (days > 0) {
                if (hours < 10) { hours = "0" + hours; }
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += days + ":" + hours + ":" + minutes + ":" + seconds;
            } else if (hours > 0) {
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += hours + ":" + minutes + ":" + seconds;
            } else if (minutes > 0) {
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += minutes + ":" + seconds;
            } else {
                newLine.textContent += seconds;
            }
            if (factMenu.childNodes[6].childNodes[17] != undefined) {
                factMenu.childNodes[6].removeChild(factMenu.childNodes[6].childNodes[17]);
            }
            factMenu.childNodes[6].appendChild(newLine);

            //Conveyor

            cost = findRealNumber(factMenu.childNodes[8].childNodes[3].innerText);
            gain = conveyorRate * GameModel.partsPCMod;
            returnOnInvestment = cost / gain;
            seconds = Math.floor(returnOnInvestment % 60);
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            minutes = returnOnInvestment % 60;
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            hours = returnOnInvestment % 24;
            returnOnInvestment = Math.floor(returnOnInvestment / 24);
            days = returnOnInvestment;
            newLine = document.createElement("p");
            //newLine.ng-show = "generator.selected";
            newLine.class = "ng-binding ng-hide";
            newLine.innerHTML = "Will pay back in ";
            if (days > 0) {
                if (hours < 10) { hours = "0" + hours; }
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += days + ":" + hours + ":" + minutes + ":" + seconds;
            } else if (hours > 0) {
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += hours + ":" + minutes + ":" + seconds;
            } else if (minutes > 0) {
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += minutes + ":" + seconds;
            } else {
                newLine.textContent += seconds;
            }
            if (factMenu.childNodes[8].childNodes[17] != undefined) {
                factMenu.childNodes[8].removeChild(factMenu.childNodes[8].childNodes[17]);
            }
            factMenu.childNodes[8].appendChild(newLine);

            //Splitter Combiner

            cost = findRealNumber(factMenu.childNodes[10].childNodes[3].innerText);
            gain = splitterCombinerRate * GameModel.partsPCMod;
            returnOnInvestment = cost / gain;
            seconds = Math.floor(returnOnInvestment % 60);
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            minutes = returnOnInvestment % 60;
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            hours = returnOnInvestment % 24;
            returnOnInvestment = Math.floor(returnOnInvestment / 24);
            days = returnOnInvestment;
            newLine = document.createElement("p");
            //newLine.ng-show = "generator.selected";
            newLine.class = "ng-binding ng-hide";
            newLine.innerHTML = "Will pay back in ";
            if (days > 0) {
                if (hours < 10) { hours = "0" + hours; }
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += days + ":" + hours + ":" + minutes + ":" + seconds;
            } else if (hours > 0) {
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += hours + ":" + minutes + ":" + seconds;
            } else if (minutes > 0) {
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += minutes + ":" + seconds;
            } else {
                newLine.textContent += seconds;
            }
            if (factMenu.childNodes[10].childNodes[17] != undefined) {
                factMenu.childNodes[10].removeChild(factMenu.childNodes[10].childNodes[17]);
            }
            factMenu.childNodes[10].appendChild(newLine);

            //Batch Converter

            cost = findRealNumber(factMenu.childNodes[12].childNodes[3].innerText);
            gain = batchConverterRate * GameModel.partsPCMod;
            returnOnInvestment = cost / gain;
            seconds = Math.floor(returnOnInvestment % 60);
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            minutes = returnOnInvestment % 60;
            returnOnInvestment = Math.floor(returnOnInvestment / 60);
            hours = returnOnInvestment % 24;
            returnOnInvestment = Math.floor(returnOnInvestment / 24);
            days = returnOnInvestment;
            newLine = document.createElement("p");
            //newLine.ng-show = "generator.selected";
            newLine.class = "ng-binding ng-hide";
            newLine.innerHTML = "Will pay back in ";
            if (days > 0) {
                if (hours < 10) { hours = "0" + hours; }
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += days + ":" + hours + ":" + minutes + ":" + seconds;
            } else if (hours > 0) {
                if (minutes < 10) { minutes = "0" + minutes; }
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += hours + ":" + minutes + ":" + seconds;
            } else if (minutes > 0) {
                if (seconds < 10) { seconds = "0" + seconds; }
                newLine.textContent += minutes + ":" + seconds;
            } else {
                newLine.textContent += seconds;
            }
            if (factMenu.childNodes[12].childNodes[17] != undefined) {
                factMenu.childNodes[12].removeChild(factMenu.childNodes[12].childNodes[17]);
            }
            factMenu.childNodes[12].appendChild(newLine);

        }
    }

    function findRealNumber(fake) {
        fake = fake.slice(0,-6);
        if (isNaN(fake.slice(-1))) {
            let ending = fake.slice(-1);
            let multiplier;
            if (ending == "K") {
                multiplier = 1000;
            } else if (ending == "M") {
                multiplier = 1000000;
            } else if (ending == "B") {
                multiplier = 1000000000;
            } else if (ending == "T") {
                multiplier = 1000000000000;
            }
            fake = fake.slice(0,-1);
            fake = fake * multiplier;
        }
        fake = Number(fake);
        return fake;
    }

})();
