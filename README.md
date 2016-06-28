# Friend-Search

var friends = {
    bill: {
        firstName: "Bill",
        lastName: "Gates",
        number: "(555) 555 - 5556",
        address: ["One Way" , "Seattle", "WA"]
    } ,
    
   steve: {
        firstName: "Steve",
        lastName: "Jobs",
        number: "(555) 554 - 5555",
        address: ["One Way" , "Cupertino", "CA"]
    }
}

var list = function (friends){
    for (var firstName in friends) { 
        console.log(firstName);
    }
}

var search = function(name) {
    for (var key in friends) {
        if (friends[key].firstName === name){
        console.log(friends[key]);
        return friends[key];
    }
}
};
