# Notes

## Problems

*

## **Notes for this project:**

### Prior Notes

* Remove non-fundamental features like gameplay customization from the public display. We may add them in the future. But keep them private and keep the project clean and easy to understand.
* All calculation/economic **elements will be variable** so that we can adjust everything to have a sustainable economic design. For instance, Clan taxes will be a variable called baseClanTax and will be initialized as 10%. After a rebellion, we will multiply rebellionTaxChange with baseClanTax. It can be 5%, 10%, or anything. We can change all of them if we need. All the variables changes can be subject to a DAO confirmation if we can manage to build this type of infrastructure. Maybe it is too complicated and may cause unpredicted problems. Think about it twice!
* **Clan Levels:** Clans will have levels (like 1-100). The required points to level up will increase exponentially as the income will increase exponentially. We can use the same increment formula we use in reward distribution (L^80). Level points = clan incomes. When a clan earns 100 FUKC, their level point will increase by 100 points as well. The Clan earning function should be internal, otherwise, clan members or anybody can send tokens and get them back from the clan leader to level up the clan.&#x20;
* **Earning functions** like clan earnings, taxes, etc. All of them **should be internal.** Nobody should be able to call these functions!
* **Team Allocation Distribution:** We will have a different token for the distribution of team allocation. I will create a token called FukcingTeamToken (FTT). This token contract will have these functionalities: I will add wallets of team members in an array, and in a mapping defining the daily reward for that particular address. The DailyReward function will be called internally every day and will get all the addresses from the array and give rewards accordingly by checking their reward from the mapping. When we have launched the FUKC token, I will pause the daily reward function and remove the ownership of the contract so that I can't change anything in that contract anymore. FUKC token contract will distribute daily allocation by checking the share of each wallet address in teamMembers array. Share = FTT.address.balance / FTT.totalSupply; We will define the FTT contract address in the constructor of the FUKC contract so that we can't redirect it to another contract.
  * I will be able to define and change the daily reward of each address. But I can't change the balance of any once they get their rewards daily. I can only set the daily reward to 0 if a particular team member leaves the project. But his/her allocation will remain. I will have the top daily reward, 10. Unity dev might have 7, blockchain dev 8, artist might get 5-6, etc. We can have agreements. I will have an initial balance for the days that I have worked on this. I will set this balance in the constructor of the contract.
  * With this system, we will have a common and transparent share of team allocation that we can't change once it's initiated. Everyone's allocation and earnings will be saved day by day. Even if someone left the project, their right will be reserved. Nobody needs to trust me, we have code to have a trustless system.
* Everything will be a smart contract. Elections, Bosses, Lords, and even fighters.
  * Boss destructions should leave enough time for everyone to vote. For instance, if someone triggers voting to destroy a boss, there should be a 1 week voting time. After the results, the boss can carry on or die.
* **Branding:** Print on demand our own products. Flags, T-shirts, hats, etc.&#x20;
  * There are two major options to do that. [Printful ](https://www.printful.com/)produces the product and ships it internationally, but [Printify ](https://printify.com/)act as a middleman. You choose the product and producer. In that sense, Printful looks like a better option. For both, you can add the buying page to your own website just like you are selling it. People can order it from all around the world.&#x20;
  * We can add our own products and clan-specific products to our website with Printful. Clans and fighters buy the products. We also order and distribute in our events to create branding.
* Try to select "Me" boss in the first level every seance and make it a tradition. We should judge ourselves first!
  * **Default Bosses:** Me, war, inflation, politics, bear market, Ignorance, Terrorism, fiat money, system, tribalism, fraud, corruption, dictators.
  * **Creative Bosses:** Twitter, Social Media, Facebook, Big Tech, VCs, Banks, Governments, Ethereum, Bitcoin, Avalanche, Shitcoins, DogeCoin, Shiba Inu, Communism, Fascism, Algo Stable Coins, Star Atlas, and other projects that people got ripped off. DAO hack, Mt Gox, FED, Ponzi Dollar, Lords, Stifler's Mom, SJW, Do Kwon, OFAC that banned Tornado.
* **Weekly Reports:** Post weekly reports about the game. How many funds were staked, how many bosses were selected, and elected, and how many funds were used in these elections, or burned in these elections? If there is any rebellion going on or a lord died, the boss died? News from the WeFukc.&#x20;
  * **Burning Gif:** Create a burning gif where the evil throws tokens into flames and burns them. Use it when you post weekly burn reports.
  * Types: Number of players signed, and exist, active. Newly created bosses, died bosses, selected and elected bosses. New clans. Events. Burned tokens by actions. Most fukced boss, best fukcer, fastest fighter, the best team, etc.
* Some stuff
  * **Motto:** Let's Fukc! || #JustForFun #JFF
  * PoF system: Proof-of-Fukc
  * **Our logo:** Broken Black Heart
* <mark style="color:red;">**Legal Problems**</mark>: If the game hits a large number of players or even some people start to sue me because of this, it would be a huge problem for me. Therefore I should act like a big tech platform.
  * Everyone can upload manipulated sexual content about anyone on the internet. It can be on Twitter, Facebook, etc. But if the victim requests from the platform to remove the content, platforms remove it immediately. We will do the same. And we will avoid Gif or video content to be less annoying. Just name, a picture, and our default stickman. People will be able to customize the stickman in our terms to make it more related to the boss. Other features of the boss (such as background image) can be added at first and tested. If it brings too much trouble, we can remove it as well.
  * We should add a warning and "I understand and accept" tick in the boss creation section. We must say: "Please do not use any real identity as a boss. It would be a violation of human rights and subject to removal. Please use only fictional entities as a boss!"
  * <mark style="color:red;">**Mention this in many places:**</mark> "We don't have any problem with names, we have a problem with the current system. Liar politicians, big money laundries, corruption, inequality, etc.
  * **Display this friendly and reasonable warning:** "Dear fellow humans! Please do not create a boss with a real name. This is our rightful protest and we will not violate the laws and human rights. Even though you give the evilest person's name to a boss, it would trigger an endless request for other people. For instance, if you create a boss named Adolf Hitler, some people would want to create a boss named Joseph Stalin and some would want to create bosses with other names. There is no good in this type of chain of reaction. Therefore, please avoid giving a real name to bosses you create. Additionally, please create disputes and vote for the removal on the bosses that have a real name. If you are smart enough, you can name your boss with a nickname so that everyone can figure out who is it ;)"
* Short Movie
  * It should mention bad things in the past and present. The main problems of humans. Like corruption, war, politics, etc.&#x20;
    * "One stickman watching horrible news, another one looking at trading charts, etc."
    * Show some people in different colors (enemy colors) who are happy with their current system. They are buying useless stuff, dying for celebrities, fighting for their politics, etc. A classic, perfect type for the current system

### Others

* We will store the character data in both IPFS and our servers to have an efficient system. When people mint a character, they will have its NFT with metadata that is stored in IPFS but when they play the game we will send the data directly from our server to provide better performance.
* **Discord - Clan Memberships:** Create clan-specific channel groups for major clans. Keep them under one roof and have a more active and energic server. Create a membership moderator class. This membership moderators will add and remove all clan members in discord. Have a specific channel for this communication. For instance: There is a channel called Clan Memberships: Only Membership Moderators and one executive from each clan can see it. Clans will have to assign membership operations to one of their members. It can be the leader of the clan as well. Only that person will see the Clan Memberships channel and will notify which members added or removed to or from the clan. This channel will have maximum slow-mode enabled (6h). Therefore clans can announce their membership changes at some specific times.
* **AMA:** Take AMA questions with a Twitter tag from Twitter. Mods will post our answers under the question posts. In this way, we will increase our digital footprint in the space. Use normal #WeFukc, not AMA specific. We'll see the post from the newest to the latest. Post AMA after editing on Youtube.
* **Marketing:** We can have a contest for each seance. Anything that is beneficial can be subject to winning like fan art, Graffitty, street art, meme, etc. We can use some of this fan art on our t-shirts. Rewards will be distributed from the Marketing allocation. We can do this after we have a decent community.
* **Clan Flags:** Clans will have flags and banners. All clans should have the mark of their lords on their flag/banner. Mark style will be determined by the clan and the lord.
* **Taking back your funds from a selection:** It can be cool but it would give a lot of harm to people and demotivate them to participate in the selection. For instance, a whale can create 2 characters and stake 1000 tokens to one of them and 100 to the other. People stake their funds in the biggest character to guarantee to be on the winning side. Then whale can withdraw its funds from the biggest character right before the ending of the selections.  Then the whale's little character wins the selection and the whale gets all the money for him with a little fund. Making 10x-20x return in just 1 selection. So, we can't implement withdraw function to the selections. Whales still can manipulate the selections by funding multiple characters and making a final move at the last second but in this case whales' earnings would be nothing if we compare it to the scenario when there is a withdraw function. Because they would lose all the tokens they fund on their fake characters. Withdraw function reduces the competitiveness of the low-budget players and ruins the whole game.
* The market price at TGE: 1 cent, therefore 4k market cap
  * **Dumping:** We can it 1 dollar but then the market cap would be 400k and it will be all in the hands of airdrop hunters. They can dump it and if we can't hold it, it goes 0. **Airdrop hunters should be in a mindset not to sell but play and have fun with it.**&#x20;
  * **Liquidity Problem:** We will have 400k FUKC for the liquidity pool. We have to have a number of dollars to support it. If the price would be 1 dollar, then we have to provide 400k dollars with 400k FUKC. This is why 1 cent is a good price. We only have to provide 4k dollars for 400k FUKC.
  * **Pumping:** It can skyrocket from 1 cent but it can't from 1 dollar. If we reach a 4m market cap from 1 dollar, it would make it 10 dollars, which is 10x. But if we reach the same market cap from 1 cent, it would make it again 10 dollars but this time with 1000x instead of 10x. This price action would attract people to invest even though they don't play.
* **Gitcoin:** If we give some percentage of the token allocations (maybe from game development) to indie game developers as a grant, like Gitcoin. We could be seen as a public good that wants to power other indie developers in the ecosystem. We should definitely do that!
  * And create a POAP for people to use for Gitcoin. Create an event for it as well.
* **Smart Contract:**&#x20;
  * **Burn Address:** The default and cheapest burn address for all projects are 0x000..00 but the name of this address is Null. So, when we sent tokens or NFTs to this address and burn, it looks to send them to a null address which is okay. BUT if we create our own burn address and name it Fukcing Hell, it would be awesome. People will see it in our videos, in blockchain explorers, in OpenSea, and maybe even in analysis. It is marketing more and we should do that.&#x20;
  * **Player Account Properties:** Uptier-account, Downtier-balance, fucking-balance, account-balance
* **Community:**
  * We should create gifs, animations, and memes for the community to use.
* **SFX and Sound Ideas:** Meme sounds. Make it a meme game, not normal.
* Items that we use and need to purchase if we make money
  * None for now&#x20;
* **Open Source:** We can make the boss election and other non-game actions fully open source with its interface. If we can make the game open-source, then no authorities can stop us. But if we can't, we can implement a feature that gives us to accept a certain type of NFT as proof of completing a level. For instance, if the community votes on-chain and accepts a different NFT address as a new level 5 success NFT, then the reward would go that the NFTs holders. By doing that, we can have more censorship resistance. But this is quite a far feature that we even not might need.
* **Stickman Colors**
  * Fighter: Black
  * Tier 1-3: <mark style="color:green;">Green</mark> (#00B050)
  * Tier 4-6: <mark style="color:blue;">Blue</mark> (#4472C4)
  * Tier 7-9: <mark style="color:yellow;">Yellow</mark> (#FFC000)
  * Tier 10-12: <mark style="color:orange;">Orange</mark> (#ED7D31)
  * Tier 12-15: <mark style="color:red;">Red</mark> (#C00000)
  * Boss: <mark style="color:purple;">Purple</mark> (Tyrian purple - #66023C)

### Gameplay Notes

* Profit Index: Every level selection will have a profit index to warn or encourage people about the profit/loss they can get. If people lock too many the index should be red and low!
  * Additionally, we should add a warning to the elections that says "Learn the election mechanisms and fund a reasonable amount to protect yourself against the high risks!"
* We will keep players' earnings centrally held but every player can get their funds anytime. Even if players don't get their funds, we will send their funds to their wallets automatically if their funds are worth more than 100 dollars.&#x20;
* Every 5 levels should have a different environment to play like different seasons. Like first 5 levels are green, bright, and a happy environment with easy enemies. But the last 5 levels (16-20) are the hardest and darkest environment. Let's call these different environments chapters.
  * Chapter 1: Green, happy, open space. Human enemies. Easy traps, less dangerous.
  * Chapter 2: Castle, Human enemies with enhanced armament. Tricky traps, give more damage.
  * Chapter 3: Underground, cave-like environment. Creatures start to appear, dreadful traps that give more damage.
  * Chapter 4: Core of the earth. Lava. Deamon-like mini-bosses and creatures. 1 shot traps.
  * Elements of different chapters: **3 types of enemy, 1 mini-boss, traps, and mapping.**
* We should provide a preview of the sex scene on the minting page. People should be able to see what they are minting. It is $100 dollar!
* The whole system resets every seance, the Reward Rate resets every day, and the Path Difficulties resets every hour.
* We should add a **warning** and "I understand and accept" tick in the boss creation section like Binance does in important things. We must say: "Please do not use any real identity as a boss. It would be a violation of human rights and subject to removal. Please use only fictional entities as a boss!"
* Fundamental armamanet:&#x20;
  * Baseball bat, knife, and Axe for handed weapons.
  * Pistol, shotgun, rifle, and grenade for ranged weapons.
  * Helmet and vest for defense.
* Armaments: People will burn FUKC tokens to mint these weapons and their bullets. Bullets and grenades will have a burn method that only can be used by the project owner. We will burn people's bullets after a fight. If a player starts the game with 100 bullets and only fires 20 of them, we will burn 20 bullets of that specific weapon after the fight.
* Higher levels will be longer and harder to pass. Therefore, people will need more health to complete. We can not give them different max health at different levels or increase the defense point of the shields relatively. It would be awful. A better solution is making enemies drop their health when they die. Stronger enemies drop the on the same chance but give more health due to the difficulty of the level. Health drop chance would be a global variable to set and all enemies would fetch it at the beginning of the level.
* Potential Bosses:&#x20;
  * Conceptual: Corruption, politicians, big money laundries, corruption, inequality, war.
  * Harmful stuff for crypto: Do Kwon, Luna, Celcius, AWS Nodes, Bear Market
* **End Scene:** When we start to fukc boss, there should be an option to zoom back smoothly. When the camera makes a zoom-out, players should start to see other gameplay and fukc scenes playing next to them. Above, under, right, and left. All directions. It would be seen as a container. Like windows of an apartment. The purpose of this feature is that players will remember that even though they are playing in the single-player mode, there are many people and they all fukc the same boss.

## **Features:**

### **Initial**

* Add animation on the building in the background. Like a sex scene, murder scene, party scene, etc. The background would look alive.
* **Rage**:&#x20;
  * when the rage is started, stop the background music, scream "FUUUUUUUUUUKC" and play metal music until the rage ends!
  * When it starts to scream, gives a shock wave and damage to near enemies. 4 different damage ranges: the closest ones get -100, then -75, -50, and -25. But all of them fall back hard. The player hits and kills everyone in one shot.

### **Short Term**

* There will be lists like "Most Fukced", "Best Fukcer" and some medals like "The Best Fukcer of Seance #35" or "Serial Fukcer"
* Add hidden places as a bonus. Those hidden places should be randomly selected. But they would be on the most difficult paths more often.
  * There will be different types of fighters that are suitable for different environments. We can hide gems in places where players can't reach the most suitable fighter. For instance, there are two different fighters. One of them is so strong but heavy, the other one light but fast. And you can complete a level with a strong fighter. We can hide a gem in that level in a place where players can only reach with that light and fast fighter. Maybe it jumps higher? The thing is players who discover this truth and play with an unsuitable fighter to find the gem should be able to find it.
  * OR, bonus doors. There would be some doors that are not obvious but easy to find. But they can contain a bonus or a trap! When a player opens a door, sometimes it may find a health, stamina, or helmet/vest. But it may find a "kick", "punch", gunfire, or even an explosion! Risky to open!
* New Weapons and enemies.
* Rage for the bare fight: Every given hit give 1 point, and every taken hit gives 2 points. Just bare fights included
* Dying SFX: Wasted GTA effects.
* Additional Languages
* Bosses will have medals like "the most fukced boss in seance #35"

### **Mid-Term**

* Having and upgrading armament like armor, sword, etc.
* Anti-bot protections.
* There will be some player fighters defined by us like Gorilla, humans, etc. We will add the feature of creating our own fighter with all animations later. From profile photos to all these personalizations will require FUKC to burn.

### **Long Term**

* Boss: At first, players will just change the name and the photo of the boss. But if we can have enough funds for development, players will start to change the whole fucking animation.
  * Future Implementations:
    * Position-based body parts: People will be able to upload drawings of the body parts based on the position. We will provide the default file and they can change it as they wish. Body type, hair, arms, and legs.
    * The whole fucking animation
* Uploading custom fighters with custom animations and armament.
  * People can add their custom fighters and we can check, adjust, and approve their fighters and make them available for everyone to use. Price: $1000 worth of FUKC
  * Custom fighters would have a royalty fee that can be set and changed. Players who play with these fighters will give x% of their earnings to the owner of these fighters. The royalty fee can not be greater than 10%. If the owner changes the royalty fee, the players who chose that fighter will be notified and be switched to a royalty-free genesis fighter. It is important to protect players.
* Multiplayer
  * 3-5 players start together to the level and the first one who reaches the boss, fukcs. Players can't damage each other and the difficulty of the level's paths will reset for each game.
  * PvP Maps: Players start from different parts of the map. They kill each other and the last one fukcs the boss. We can have a new separate boss for this type of gameplay. Maps can include bots or not.
  * In the future, we can add fukc battles. 1vs1 or 5vs5 team battles. Players choose a character and upgrade it. Just like brawl stars, but if you lose your strength (health), you give up and get fucked! And people get your money!
    * Again, after fukc battles, we can make tournaments.
  * Rocket Leauge style communication tool but with sound. Clans have custom sounds and texts.
* Procedural level generation: The system generates a procedural map and random difficulty with its different paths. Maps and their difficulties would change after the player completes the level. All players will have their own unique map. No daily reset. It resets after every win. Therefore, a new continues journey after each win.
* Another future might be betting. Betting can start at an early age. First, people can bet which character will get selected for the next seance, after the fukc battles, people can start betting on tournaments.
* Test: Caricaturized characters rather than stickmen.
