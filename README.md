# 441-e2
//Atlas Jiang Jiawei 223190706 
// Define a function to display a thank you message  
function thankUser() {    
    console.log("Thank you for using the program");    
}    
    
// Define a function to collect user information, grades, and calculate the total and average  
function collectAndCalculateGrades() {    
    // Output "Enter your full name"  
    const userName = prompt("Enter your full name");    
    let total = 0;    
    // For each unit from 1 to 4  
    for (let unit = 1; unit <= 4; unit++) {    
        // Output "Enter grade" for the current unit  
        const grade = prompt(`Enter grade for unit ${unit}`);    
        // Add the grade to the total  
        total += parseFloat(grade);    
    }    
    // Calculate the average  
    const average = total / 4;    
    // Output the total and average  
    console.log(`Total: ${total}, Average: ${average}`);    
    // Display the thank you message  
    thankUser();    
}    
    
// Start the program  
console.log("Need help with calculation?");    
// Input user response  
const userResponse = prompt();    
if (userResponse.toLowerCase() === "yes") {    
    // If the user needs help, collect and calculate grades  
    collectAndCalculateGrades();    
} else {    
    // Otherwise, just display the thank you message  
    thankUser();    
}
