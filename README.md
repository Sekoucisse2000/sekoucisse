import * as readline from 'node:readline/promises';
import { stdin as input, stdout as output } from 'node:process';
import { log } from 'node:console';
const userInput = readline.createInterface({ input, output });

let dag = await userInput.question('welke dag van de week is vandaag; ');
let maand = parseFloat(await userInput.question('de hoeveelstedag van de maand is het; '));
let datum = await userInput.question('welke maand zijn we vandaag; ');
console.log(" Het is vandaag " +  dag + datum + maand);

process.exit()
