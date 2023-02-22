# Researching Commands
The command `grep` takes in a given string and searches through files to find that string. 

Command-line options using `grep`:

### 1. `grep -r "string"`
#### Example 1
input: `grep -r "Lucayans"`

output: `travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.`

#### Example 2
input: `grep -r "Mundo"`

output: `non-fiction/OUP/Castro/chL.txt:A folk medicine ritual also called a barrida, from the Spanish verb barrer, meaning a “sweeping,” as in housecleaning. Limpiar means to clean and a limpia is similar to a barrida. Both words mean a cleansing, in a medical and in a spiritual sense. Some people use the word limpieza instead of limpia, but the significance is the same. An individual may seek a limpia from a healer if the person is not feeling well with no specific cause or feels that bad luck or misfortune is prevalent in his or her life. A limpieza can expel the hostile forces and also provide spiritual strength so that the person can effectively fight off negative energy. Spiritual healers who are not curanderos perform limpias, although mostly it is curanderos who perform this ritual. The patient may be standing, sitting in a chair, or lying down while the ritual is performed. The healer will sweep the patient with a little broom made of herbs, such as sage, rosemary, and rue, believed to be effective in eliminating evil influences. Herbal water, holy water, or alcohol is sprinkled over the person in the form of a cross, and the healer’s hands are used to sweep along the whole body, pushing away the evil spirits. While this is being done prayers are recited. The prayers may be the Lord’s Prayer or Las Doce Verdades del Mundo (The Twelve Truths of the World). Instead of herbs some curanderos use an object for the sweeping, such as an egg or a lemon, believing that it will absorb the harm or illness affecting the patient. These objects are burned after the ritual, ensuring the recovery of the person. The person is swept on all sides, front and back, and if there is pain in a particular spot, special attention will be given to that area. Trotter states that “the presence of the curandero, the soothing effect of the sweepings (touching), and the low-key monotone chant of the prayers produces in the patient a light trance state that is comforting and reassuring” (Trotter and Chavira 1997, 82).
travel_guides/berlitz2/Cuba-WhereToGo.txt:Havana’s distant era lives on. Legendary places plucked from the pages of popular novels and the lives of fiction writers need little input from visitors to evoke their storied past: Graham Greene’s Hotel Sevilla, where “Our Man in Havana” went to meet his secret service contact, and Hemingway’s favorite watering holes (El Floridita and La Bodeguita del Medio) and the Hotel Ambos Mundos, where he penned much of For Whom the Bell Tolls.
travel_guides/berlitz2/Cuba-WhereToGo.txt:Much of restored Old Havana is concentrated in only a few blocks at the eastern end of these streets. On the corner of Mercaderes and Obispo is the recently renovated, 1920s-era Hotel Ambos Mundos; Hemingway lived on and off in room 511 for a couple of years during the 1930s. The room contains original artifacts from Hemingway’s many years in Cuba, including the typewriter he used to write most of For Whom the Bell Tolls (those not staying in the hotel can visit the room for US$2).
travel_guides/berlitz2/PuertoRico-WhatToDo.txt:Mundo Submarino (Isla Verde; Tel. 791-5764). Daily diving tours and PADI training.
travel_guides/berlitz2/Vallarta-WhatToDo.txt:There are several waterparks: In Acapulco, the CICI (Centro Internacional de Convivencia Infantil), across from the Convention Center, offers hours of fun with waterslides, a water center for toddlers, a fresh-water pool with waves, plus a dolphin and seal show, all included in the entrance fee of around US$4. Another waterpark is located near Caleta beach, called Mundo Mágico Marino. It features waterslides, an aquarium, pools — one is a saltwater pool — and boat rides. El Rey León, located near Pie de la Cuesta, is a large family-style restaurant with shallow pools and waterslides for children, plus a miniature train.In Puerto Vallarta, the Mayan Palace Waterpark in Marina Vallarta has waterslides, a lazy-river, and a mini-waterpark for young children. Children ten and older will be both moved and amazed by swimming with the dolphins, experiences that are available both in Acapulco and Puerto Vallarta.
travel_guides/berlitz2/Vallarta-WhereToGo.txt:However, Caleta and Caletilla, coves located south of the zócolo on the Peninsula de las Playas, are the most popular public beaches in Acapulco. They are colorful sites, with palapa-topped beach restaurants, bright-hued passenger boats, water sports–equipment rental stands, and fishermen selling their fresh catch to beachgoers. These side-by-side beaches are separated by a narrow, rocky peninsular, which is the site of the Mágico Mundo Marino water park and aquarium.
`

`grep -r "string"` does a recursive search to find files that contain the string inputted inside the command. 


 Citation: [Link](https://alvinalexander.com/linux-unix/recursive-grep-r-searching-egrep-find/)

### 2. `grep -c "String" *.txt`
#### Example 1
input: `grep -c "Lucayans" *.txt`

output: `Algarve-History.txt:0
Algarve-Intro.txt:0
Algarve-WhatToDo.txt:0
Algarve-WhereToGo.txt:0
Amsterdam-History.txt:0
Amsterdam-Intro.txt:0
Amsterdam-WhatToDo.txt:0
Amsterdam-WhereToGo.txt:0
Athens-History.txt:0
Athens-Intro.txt:0
Athens-WhatToDo.txt:0
Athens-WhereToGo.txt:0
Bahamas-History.txt:2
Bahamas-Intro.txt:0
Bahamas-WhatToDo.txt:0
Bahamas-WhereToGo.txt:0
Bali-History.txt:0
Bali-WhatToDo.txt:0
Bali-WhereToGo.txt:0
Barcelona-History.txt:0
Barcelona-WhatToDo.txt:0
Barcelona-WhereToGo.txt:0
Beijing-History.txt:0
Beijing-WhatToDo.txt:0
Beijing-WhereToGo.txt:0
Berlin-History.txt:0
Berlin-WhatToDo.txt:0
Berlin-WhereToGo.txt:0
Bermuda-history.txt:0
Bermuda-WhatToDo.txt:0
Bermuda-WhereToGo.txt:0
Boston-WhereToGo.txt:0
Budapest-History.txt:0
Budapest-WhatToDo.txt:0
Budapest-WhereoGo.txt:0
California-History.txt:0
California-WhatToDo.txt:0
California-WhereToGo.txt:0
Canada-History.txt:0
Canada-WhereToGo.txt:0
CanaryIslands-History.txt:0
CanaryIslands-WhatToDo.txt:0
CanaryIslands-WhereToGo.txt:0
Cancun-History.txt:0
Cancun-WhatToDo.txt:0
Cancun-WhereToGo.txt:0
China-History.txt:0
China-WhatToDo.txt:0
China-WhereToGo.txt:0
CostaBlanca-History.txt:0
CostaBlanca-WhatToDo.txt:0
Costa-History.txt:0
Costa-WhatToDo.txt:0
Costa-WhereToGo.txt:0
Crete-History.txt:0
Crete-WhatToDo.txt:0
Crete-WhereToGo.txt:0
CstaBlanca-WhereToGo.txt:0
Cuba-History.txt:0
Cuba-WhatToDo.txt:0
Cuba-WhereToGo.txt:0
Nepal-History.txt:0
Nepal-WhatToDo.txt:0
Nepal-WhereToGo.txt:0
NewOrleans-History.txt:0
Paris-WhatToDo.txt:0
Paris-WhereToGo.txt:0
Poland-History.txt:0
Poland-WhatToDo.txt:0
Portugal-History.txt:0
Portugal-WhatToDo.txt:0
Portugal-WhereToGo.txt:0
PuertoRico-History.txt:0
PuertoRico-WhatToDo.txt:0
PuertoRico-WhereToGo.txt:0
Vallarta-History.txt:0
Vallarta-WhatToDo.txt:0
Vallarta-WhereToGo.txt:0`

#### Example 2
input: `grep -c "China" *.txt`

output: `Algarve-History.txt:0
Algarve-Intro.txt:0
Algarve-WhatToDo.txt:0
Algarve-WhereToGo.txt:0
Amsterdam-History.txt:1
Amsterdam-Intro.txt:0
Amsterdam-WhatToDo.txt:0
Amsterdam-WhereToGo.txt:0
Athens-History.txt:0
Athens-Intro.txt:0
Athens-WhatToDo.txt:0
Athens-WhereToGo.txt:0
Bahamas-History.txt:0
Bahamas-Intro.txt:0
Bahamas-WhatToDo.txt:1
Bahamas-WhereToGo.txt:0
Bali-History.txt:2
Bali-WhatToDo.txt:0
Bali-WhereToGo.txt:0
Barcelona-History.txt:0
Barcelona-WhatToDo.txt:0
Barcelona-WhereToGo.txt:1
Beijing-History.txt:14
Beijing-WhatToDo.txt:17
Beijing-WhereToGo.txt:40
Berlin-History.txt:0
Berlin-WhatToDo.txt:0
Berlin-WhereToGo.txt:2
Bermuda-history.txt:0
Bermuda-WhatToDo.txt:0
Bermuda-WhereToGo.txt:0
Boston-WhereToGo.txt:2
Budapest-History.txt:0
Budapest-WhatToDo.txt:0
Budapest-WhereoGo.txt:0
California-History.txt:1
California-WhatToDo.txt:0
California-WhereToGo.txt:4
Canada-History.txt:2
Canada-WhereToGo.txt:7
CanaryIslands-History.txt:0
CanaryIslands-WhatToDo.txt:0
CanaryIslands-WhereToGo.txt:0
Cancun-History.txt:0
Cancun-WhatToDo.txt:0
Cancun-WhereToGo.txt:0
China-History.txt:39
China-WhatToDo.txt:8
China-WhereToGo.txt:115
CostaBlanca-History.txt:0
CostaBlanca-WhatToDo.txt:0
Costa-History.txt:0
Costa-WhatToDo.txt:0
Costa-WhereToGo.txt:0
Crete-History.txt:0
Crete-WhatToDo.txt:0
Crete-WhereToGo.txt:0
CstaBlanca-WhereToGo.txt:0
Cuba-History.txt:0
Cuba-WhatToDo.txt:0
Cuba-WhereToGo.txt:1
Nepal-History.txt:2
Nepal-WhatToDo.txt:0
Nepal-WhereToGo.txt:0
NewOrleans-History.txt:0
Paris-WhatToDo.txt:0
Paris-WhereToGo.txt:0
Poland-History.txt:0
Poland-WhatToDo.txt:0
Portugal-History.txt:1
Portugal-WhatToDo.txt:0
Portugal-WhereToGo.txt:0
PuertoRico-History.txt:0
PuertoRico-WhatToDo.txt:0
PuertoRico-WhereToGo.txt:0
Vallarta-History.txt:2
Vallarta-WhatToDo.txt:0
Vallarta-WhereToGo.txt:1
`

`grep -c "string" *.txt` prints out the number of times the inputted string appears in all the text files in the specific directory

Citation: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

### 3. `grep -n "string" *.txt`

#### Example 1
input: `grep -n "Lucayans" *.txt`

output: `Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
Bahamas-History.txt:7:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.`

#### Example 2
input: `grep -n "Mundo" *.txt`

output: `Cuba-WhereToGo.txt:18:Havana’s distant era lives on. Legendary places plucked from the pages of popular novels and the lives of fiction writers need little input from visitors to evoke their storied past: Graham Greene’s Hotel Sevilla, where “Our Man in Havana” went to meet his secret service contact, and Hemingway’s favorite watering holes (El Floridita and La Bodeguita del Medio) and the Hotel Ambos Mundos, where he penned much of For Whom the Bell Tolls.
Cuba-WhereToGo.txt:30:Much of restored Old Havana is concentrated in only a few blocks at the eastern end of these streets. On the corner of Mercaderes and Obispo is the recently renovated, 1920s-era Hotel Ambos Mundos; Hemingway lived on and off in room 511 for a couple of years during the 1930s. The room contains original artifacts from Hemingway’s many years in Cuba, including the typewriter he used to write most of For Whom the Bell Tolls (those not staying in the hotel can visit the room for US$2).
PuertoRico-WhatToDo.txt:83:Mundo Submarino (Isla Verde; Tel. 791-5764). Daily diving tours and PADI training.
Vallarta-WhatToDo.txt:80:There are several waterparks: In Acapulco, the CICI (Centro Internacional de Convivencia Infantil), across from the Convention Center, offers hours of fun with waterslides, a water center for toddlers, a fresh-water pool with waves, plus a dolphin and seal show, all included in the entrance fee of around US$4. Another waterpark is located near Caleta beach, called Mundo Mágico Marino. It features waterslides, an aquarium, pools — one is a saltwater pool — and boat rides. El Rey León, located near Pie de la Cuesta, is a large family-style restaurant with shallow pools and waterslides for children, plus a miniature train.In Puerto Vallarta, the Mayan Palace Waterpark in Marina Vallarta has waterslides, a lazy-river, and a mini-waterpark for young children. Children ten and older will be both moved and amazed by swimming with the dolphins, experiences that are available both in Acapulco and Puerto Vallarta.
Vallarta-WhereToGo.txt:89:However, Caleta and Caletilla, coves located south of the zócolo on the Peninsula de las Playas, are the most popular public beaches in Acapulco. They are colorful sites, with palapa-topped beach restaurants, bright-hued passenger boats, water sports–equipment rental stands, and fishermen selling their fresh catch to beachgoers. These side-by-side beaches are separated by a narrow, rocky peninsular, which is the site of the Mágico Mundo Marino water park and aquarium.`

`grep -n "string" *.txt` displays the file, line number, and the line the string appears in the text files in the directory.

Citation: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

### 4. `grep -o "string" *.txt`
#### Example 1
input: `grep -o "Mundo" *.txt`

output: `Cuba-WhereToGo.txt:Mundo
Cuba-WhereToGo.txt:Mundo
PuertoRico-WhatToDo.txt:Mundo
Vallarta-WhatToDo.txt:Mundo
Vallarta-WhereToGo.txt:Mundo`

#### Example 2
input: `grep -o "Lucayans" *.txt`

output: `Bahamas-History.txt:Lucayans
Bahamas-History.txt:Lucayans`

`grep -o "string" *.txt` prints out the string every time it is found in each text file of the directory.

Citation: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
