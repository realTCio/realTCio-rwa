/* Tokenization of Real-world Assets
    Asset: Pre-paid Mobile Data
    Tokenization Type: Directly backed with off-chain collateral
    Author: realTCio
*/

/*  Problem:  
        All too often, Pre-paid Mobile Data users do not get to enjoy the full value of their Pre-paid Mobile Data 
        purchases. This happens when the user is unable to use all the data purchased before expiry, probably because they have 
        purchased too much,or because they have spent most of their time in Wi-Fi coverage areas, thus not using their Pre-paid Mobile 
        Data. The user is unable to extract liquidity from excess Pre-paid Mobile Data and ends up losing any excess Pre-paid Mobile 
        Data, and the corresponding residual value.
    Purpose: 
        The purpose of this smart contract is to improve the efficiency of the Pre-paid Mobile Data market and to enhance the liquidity 
        of purchased Pre-paid Mobile Data.
    Solution:
    Directly-backed tokenization of Pre-paid Mobile Data is proposed as one solution to the problem.A cross-chain, dynamic NFT is minted
    to represent off-chain Pre-paid Mobile Data. The solution is expected to enhance the liquidity of Pre-paid Mobile Data and to 
    improve the efficiency of the Pre-paid Mobile Data market.
        1. Upon recharging their Mobile Phone, an ownerOnly Chainlink smart contract mints a cross-chain ERC721 dynamic NFT whose 
            metadata represents:  
            - the mobile phone number
            - the amount of Mobile Data
            - the value in USDC of Mobile Data
            - the expiry date of Mobile Data
        3. In the normal course of depletion of Mobile Data over the data validity period, Chainlink Functions interrogate the 
            mobile phone for the Mobile Data balance, which is then used to update the cross-chain dynamic NFT.
        4. One day before expiry of Pre-paid Mobile Data, if there is a Mobile Data positive balance, Chainlink Functions initiate 
            the sale of remaining Pre-paid Mobile Data for corresponding USDC and stores the USDC in the smart contract for the user 
            to withdraw.
*/
