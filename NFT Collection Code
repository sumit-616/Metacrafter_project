/*
Assessment Requirements
1. Create a variable that can hold a number of NFT's. What type of variable might this be?
2. Create an object inside your mintNFT function that will hold the metadata for your NFTs. 
The metadata values will be passed to the function as parameters. When the NFT is ready, 
you will store it in the variable you created in step 1
3. Your listNFTs() function will print all of your NFTs metadata to the console (i.e. console.log("Name: " + someNFT.name))
4. For good measure, getTotalSupply() should return the number of NFT's you have created
*/

// create a variable to hold your NFT's
const nftCollection = [];

// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT(name, age, occupation, hairColor, eyeColor, creator, mintDate) {
    const nft = {
        name: name,
        age: age,
        occupation: occupation,
        hairColor: hairColor,
        eyeColor: eyeColor,
        creator: creator,
        mintDate: mintDate
    };
    nftCollection.push(nft);
}

// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs() {
    for (let i = 0; i < nftCollection.length; i++) {
        console.log("NFT #" + (i + 1));
        console.log("Name: " + nftCollection[i].name);
        console.log("Age: " + nftCollection[i].age);
        console.log("Occupation: " + nftCollection[i].occupation);
        console.log("Hair Color: " + nftCollection[i].hairColor);
        console.log("Eye Color: " + nftCollection[i].eyeColor);
        console.log("Creator: " + nftCollection[i].creator);
        console.log("Mint Date: " + nftCollection[i].mintDate);
        console.log("-------------------------");
    }
}

// print the total number of NFTs we have minted to the console
function getTotalSupply() {
    return nftCollection.length;
}

// call your functions below this line
mintNFT("Sumit Kumar", 20, "Software Engineer", "Black", "Blue", "Akash", "2023-05-01");
mintNFT("Bhaskar Kumar", 22, "Doctor", "Blue", "Green", "Arjun", "2023-05-02");
mintNFT("Adarsh RAi", 21, "Artist", "Black", "Brown", "Saurav", "2023-05-03");

listNFTs();

console.log("Total Supply: " + getTotalSupply());
