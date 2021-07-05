# smartcontract
pragma solidity ^0.4.2;
import 'assets.sol';

contract ProductTrack {
    
    
    string id;
    
    function setID(string serial) public{
        
        id=serial;
    }
    
    function getId() public constant returns(string){
        return id;
    }
    
struct Product{
    
    string name;
    string description;
    string manufacturer;
    bool initialized;
}

mapping(string = > Product) private productStore;

productStore[uuid] = Product(name, description, true, producer);

mapping(address = > mapping(string => bool)) ptivate wallet;

walletStore[msg.sender][uuid]=true;

event ProductCreate(address account, string uuid, string producer)
event RejectCreate(address account, string uuid, string message)
event ProductTransfer(address from, string uuid)
event RejectTransfer(address from, string uuid, string message)

function createProduct(string name, string description, string producer){
    
    if(productStore[uuid]initialized){
        RejectCreate(msg.sender,uuid,"Prodect with this UUIS already created")
    }
    
    productStore[uuid] = Product(name, description, true)
    walletStore[msg.sender][uuid]=true;
    ProductCreate[msg.sender,uuid, producer];
}


    



}
