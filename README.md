# MyContarct2
#ARRAYS IN SOLIDITY

pragma solidity ^0.6.0;

contract MyContract2 {
    //ARRAY 
    //In Solidity, an array can be of compile-time fixed size or of dynamic size. 
    //For storage array, it can have different types of elements as well.
    uint[] public uintArray = [1,2,3];
    string[] public stringArray = ["PAVAN", "PARDHU", "SOMU"];
    string[] public values;
    uint[][] public array2D = [ [1,2,3], [4,5,6] ];
    
    function addValue(string memory _value) public{
        values.push(_value);
    }
        
    function valueCount() public view returns (uint) {
        return values.length;
    }
}
