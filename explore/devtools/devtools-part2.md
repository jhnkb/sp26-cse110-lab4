1. The bug is that num1 and num2 are being treated as strings and therefore getting concatenated instead of being added.
2. Convert them to numbers because right now they are strings. For example: 
    let num1 = Number(document.getElementById("num1").value);