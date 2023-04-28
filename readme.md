# The Poetry Machine

*"An anthology is an act of civilization."*

In my essay entitled [*An Act of Civilization,*](https://github.com/scottleechua/poetry-machine/blob/main/an%20act%20of%20civilization.pdf) I critique how the print anthology (e.g., of "mid-century poetry") perpetuates a colonial, taxonomic way of recording history. I prototype the Poetry Machine---a machine learning model trained on the works to be archived---as a more dynamic, generative way to "anthologize" written works.

I created this in 2019 as the final project for Lawrence Ypil's class on the history of Philippine literature in English. This was way, way before the explosion of generative AI, and especially ChatGPT and large language models that can do exactly what I was trying to hack together back then.

Part of the joy of the project was that the Poetry Machine was just within reach, but not quite there. I'd love to revisit this work soon---yes, to build a version 2.0 of the Machine with the new technologies available, but also to reflect on how, now that future I had passionately written about has loudly arrived, why I feel so hesitant to step into it.

## Contents of “corpus.txt”

82,868 characters / 15,350 words / 2,527 lines
prepared by Scott Lee Chua, Yale-NUS College

"corpus.txt" is used in a character-based LSTM text-generator model.

## Data Preparation

Line breaks and indentations are retained.

Hyphens "-", em dashes "--", commas ",", periods ".", question marks "?", and exclamation marks "!" are retained.

Skipped lines are retained between poems, but removed from between stanzas.

All letters are in lowercase to reduce the number of unique characters.

Ellipses "..." are replaced by "&".

All titles, bylines, and dates of publication are removed. Instead, poem titles and bylines are listed in order of appearance in "corpus.txt".

Poems from "Man of Earth", which are less readily available either online or in print, also have their dates of publication listed.

## Selection and Sources of Poems

This corpus consists of 148 poems: 134 by Filipinos, 14 by American or British poets.

The poems by Filipinos (not in the public domain) are manually transcribed from:
Abad, G. & Manlapaz, E. (1989). "Man of Earth: An Anthology of Filipino Poetry and Verse from English, 1905 to the Mid-50s." Quezon City: Ateneo de Manila Press.

The excerpt of Justo Juliano's "Sursum Corda!" is from Abad's essay "Inang Bayan Our Muse: Early Filipino Poets in English, 1905 to 1924", which appears in:
Abad, G. (2008). "Our Scene So Fair: Filipino Poetry in English, 1905 to 1955." Quezon City: The University of the Philippines Press.

All other poems (in the public domain) are sourced from the Academy of American Poets (https://poets.org).

The corpus was proofread twice, but any remaining typographical errors are my own.

## Filipino Poets
Amador Daguio
- Man of Earth, 1932
- Land of Our Desire, 1934, 1937

Jose Garcia Villa
- Song of Ripeness, 1929
- The Country that is My Country, 1934
- Tale of the Lover and the Voice, 1934

Horacio dela Costa
- Roads, 1932
- I Face the east, I watch the Painter, Morn c1932
- Literature, 1932
- Friend Cigarette, 1934
- Longing for the Sea, 1932

R. Zulueta y da Costa
- Today's Song, 1933

N.V.M. Gonzalez
- The Law, 1935
- Sun Bird, 1933
- My Tiredness, 1932
- Circus Song, 1934
- Capture, 1935
- Prayer, 1935

Leon Ma. Guerrero, Jr.
- Clouds, 1932
- Rub the Lamp and Command, 1932

Narciso G. Reyes
- Wordless, 1935

Fideo Soriano Duque
- So This is the Fruit, 1935

Angel Rene A. Iturralde
- Bagumbayan, 1934
- After Palanan, c1934

Conrado B. Rigor
- Risus Sardonicus, 1934
- Ghost, 1934

Aurelio Alvero
- 1896, 1932
- O Night!, 1929
- The Fire Tree, 1933
- Truth Lies in the Mirror, 1933
- Palms, 1933
- Nunc Dimittis, 1931

Jose P. Poblador
- Pilgrimage, 1934

- Desiderio F. Aquitania
- Omnipresence, 1934

Carlos P. San Juan
- I Hold You in My Heart, 1933, 1935

Trinidad L. Tarrosa-Subido
- To Manhattan, 1934
- Maria and the City, c1935
- You Shall be Free, 1934
- And the Wounds Bleed Anew..., 1934
- Vanity, 1934

Ben Dizon Garcia
- Saturday Night, 1935

Isidro P. Villar
- Prayer for Faith, 1933

Florizel Diaz
- David and Bathsheba, 1933
- To a Dog, 1932

Guillermo V. Sison
- Ghosts, 1932
- Night-thief, 1932
- Flower of Beauty, 1935

Anatolio S. Litonjua
- A Child Looks at its Mother, 1932
- Song After Deceit, 1935
- Argument in a Circle, 1930
- On the Grass, 1931
- Pagan, 1934

Conrado S. Ramirez
- Love Story, 1933
- Leaf from a Story-book, 1935
- To Hitomaro, 1931
- My Wife's Hands, 1933

Josue Rem. Siat
- Mang Teban and the Weather, 1934

S. P. Lopez
- One Thing at Least is Certain, 1928
- I Sang a Hymn of Faith, 1929
- Brotherhood, 1932
- Questions, 1933

Conrado Pedroche
- If I Should Die Ere All My Songs are Sung, c1935
- Moon-struck, 1929, 1933
- River-winds, 1932
- To a Woman, 1930
- Spiders and Worms, 1932
- Pandora, 1934

Gregorio Estonanto
- One Minute More, 1931
- Song from a Barroom, 1931, 1938
- Answer to Ermengarde, 1934, 1939

Pedro Aguada
- Back in the Old Hometown, 1933

Celestino M. Vega
- Pastoral Song, 1933
- Conquered, 1933
- Last Words, 1935
- For My God, 1934

A. E. Litiatco
- Paradox, 1933

Virgilio F. Floresca
- The Quacks at Helicon, 1931
- Intramuros, c1933
- The Spanish Governor, c1933

Cornelio F. Faigao
- Birds in the Church, 1932
- A Bundle of Old Love Letters, 1932
- Code, 1933
- Cogon Grass, 1934
- Islands, 1935
- Night in a Small Town, 1935

Angela Manalang Gloria
- Apology, 1935
- Power of the Dream, 1938
- But the Western Stars, 1928
- Soledad, 1935

Luis G. Dato
- Cosmos, 1932, 1938
- Day on the Farm, 1934
- The Spouse, 1934
- Harvest, 1933

Francisco B. Icasiano
- Repentance, 1928
- A Year Ago Tonight, 1933

Vicente L. de Fierro
- Night, 1927

Jose M. Hernandez
- The Dream That Was Our Yesterday, 1932
- Nectar, 1926
- Song of the Tide, 1934
- The House of Echoes, 1935

Francisco G. Tonogbanua
- Tranquility, 1932
- My Love, 1931
- The Trailing Arbutus in My Letter, 1935

Natividad Marquez
- The Sampaguita, 1924
- The Stranger at the Gate, 1924
- The Angelus, 1924

Procopio Solidum
- Requiem, c1924
- Fair Rosario of Sagay, 1921
- Babson's Statistics, 1939

Fernando Ma. Guerrero
- Where is My May?, 1914
- Come to Me!, 1924

Juan F. Salazar
- Freedom's Sword, 1925

Maximo M. Kalaw
- Air Castles, 1910

Proceso E. Sebastian
- The Parting Year, 1911

Fernando M. Maramag
- To My Lady in Laoag, 1909
- Sonnet, 1911
- Moonlight on Manila Bay, 1912
- To Melancholy, 1912
- Stanzas, 1912
- Cagayano Peasant Songs, 1912
- The Dreamer's Heritage, 1912

M. de Gracia Concepcion
- A Christ Without a Cross, 1926
- Rim of the World, 1925
- Ili-na, 1925
- Rain, 1931
- Silent Trails, 1931
- Communion, 1931
- Resurrection, 1932

Mauro Mendez
- Your Voice in the Darknes, 1932
- To the Great Plebeian, 1925
- A Christmas Poem, 1931

Lorenzo Paredes
- My Parting Words, 1915

E. Pascua Alcabedas
- Moonrise, 1916

Justo Juliano
- Sursum Corda!, 1907 (excerpt)

---------------------American and British Poets--------------------------
Henry Wadsworth Longfellow
- Paul Revere's Ride

Wallace Stevens
- Peter Quince at the Clavier

Robert Frost
- Fire and Ice
- Stopping by Woods on a Snowy Evening
- Acquainted With the Night
- The Road Not Taken

Dylan Thomas
- The force that through the green fuse drives the flower

e.e. cummings
- what if a much of a which of a wind
- somewhere i have never travelled,gladly beyond

Ralph Waldo Emerson
- Sursum Corda

William Wordsworth
- [I wandered lonely as a Cloud]
- On Seeing a Tuft of Snowdrops in a Storm

William Shakespeare
- Sonnet CXI
- Sonnet LIII
