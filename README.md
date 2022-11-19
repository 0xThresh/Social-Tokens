# Social Tokens Contract
## Contract Overview
The contract is a partial implementation of EIP-4974[https://ethereum-magicians.org/t/eip-4974-fungible-non-tradable-tokens-or-exp/8805], which describes the use of fungible, non-tradable tokens. The main difference between this contract and EIP-4974 is the removal of any concept of a Participant. EIP-4974 defines participants as someone who send a transaction to opt into the system. While the value of this makes sense in many cases, I believe it adds an extra step for end users that isn't necessary in the use cases I explored. I believe a good frontend/ UX engineer could find a way to make this process seamless, but because that's not a skillset I possess, I found it easier for users to remove the concept of a Participant, and assume goodwill of the contract Operator for the sake of this example. The deployment and testing example scripts included with this contract utilize Brownie. 

## Deploying the Contract
The `deploy_social_token.py` script is used for deployment. 

## Testing the Contract
The `test_social_token.py` script is used for testing. 

## Contract Use Cases
A handful of use cases are defined in the EIP, and re-posted below:
- Reddit-like Karma
- DAO delegation of authority levels
- Loyalty points from a business
- Ratings for contenders in sports or other competitive leagues.
- Credit scores (Ugh that feels dystopian, but at least it’d be more transparent and trustworthy than current credit scoring systems around the world…)
- Kudos given for contributions of some sort, i.e. for volunteer hours at a nonprofit
The main use case I have explored is the use of these tokens for loyalty points for an artist to reward their community for purchases. This could be purchases of their physical art from the artist's storefront, or for purchasing NFTs from their PFP collection. The tokens could then be exchanged for prizes, such as a free piece of art or free shipping on a physical piece of art. I have also explored the idea of community credit scores, where members of a community who rely on each other for collaboration are able to transfer tokens as a sign of a job well done from their collaborators. 