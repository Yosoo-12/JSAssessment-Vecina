/*
Assessment Requirements
1. Create a variable that can hold a number of NFTs. What type of variable might this be?
2. Create an object inside your mintNFT function that will hold the metadata for your NFTs. 
   The metadata values will be passed to the function as parameters. When the NFT is ready, 
   you will store it in the variable you created in step 1.
3. Your listNFTs() function will print all of your NFTs metadata to the console (i.e. console.log("Name: " + someNFT.name)).
4. For good measure, getTotalSupply() should return the number of NFTs you have created.
*/

// Create a variable to hold your NFTs
let nfts = [];  // This will hold an array of NFT objects
let idCounter = 1;  // Initialize a counter for NFT IDs

// This function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT(name, eyeColor, shirtType, bling, shoes) {
    // Create an NFT object
    const nft = {
        id: idCounter,
        name: name,
        eyeColor: eyeColor,
        shirtType: shirtType,
        bling: bling,
        shoes: shoes,
    };

    // Store the NFT in the array
    nfts.push(nft);
    console.log("Minted: ID #" + idCounter + " " + name); // Log the minting message
    idCounter++;  // Increment the ID for the next NFT
}

// Create a "loop" that will go through an "array" of NFTs
// and print their metadata with console.log()
function listNFTs() {
    for (let nft of nfts) {
        console.log("ID: " + nft.id);
        console.log("Name: " + nft.name);
        console.log("Eye Color: " + nft.eyeColor);
        console.log("Shirt Type: " + nft.shirtType);
        console.log("Bling: " + nft.bling);
        console.log("Shoes: " + nft.shoes);
        console.log('---------------------------');  // Separator for better readability
    }
}

// Print the total number of NFTs we have minted to the console
function getTotalSupply() {
    return nfts.length;  // Return the count of NFTs in the array
}

// Call your functions below this line

// Mint some NFTs
mintNFT("Alfer", "Red", "T-shirt", "Watch", "Nike");
mintNFT("Clarence", "Blue", "Jacket", "Necklace", "Jordan");
mintNFT("Kyle", "Gray", "Hoodie", "Bracelet", "Adidas");
mintNFT("Brian", "Green", "Tuxedo", "Earrings", "New Balance");

// List NFTs
console.log("\nList of NFTs:");
listNFTs();

// Get total supply of NFTs
console.log("Total NFTs minted: " + getTotalSupply());
