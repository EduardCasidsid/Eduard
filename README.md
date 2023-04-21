let collectionNFT = []; 

function mintNFT (_name, _color, _age, _weight) {
    const Dog ={
        "name":_name,
        "color":_color,
        "age":_age,
        "weight":_weight,
    }
    collectionNFT.push(Dog);
console.log("minted: " + _name);

}    
function listNFTs () {
    for(let i = 0; i < collectionNFT.length; i++){
        console.log("\nId: \t\t" + (i+1));
        console.log("name: \t\t"+ collectionNFT[i].name);
        console.log("color: \t\t"+ collectionNFT[i].color);
        console.log("age: "+ collectionNFT[i].age);
        console.log("weight: \t\t"+ collectionNFT[i].weight);
    }    
}
function getTotalSupply() {
    console.log("TOTALNFTs" + collectionNFT.length);
}
mintNFT("Browny","White","5 years old", "10KG")
mintNFT("Zoey","bROWN","6years old", "14KG")
mintNFT("Toothless","Dark","5 years old", "8KG")
mintNFT("Luna","YELlow","3 years old", "9KG")
listNFTs();
getTotalSupply()
