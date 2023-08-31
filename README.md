> This dataset is derived from [@soumendraprasad](https://www.kaggle.com/soumendraprasad)'s [broader image dataset](https://www.kaggle.com/datasets/soumendraprasad/fifa-2022-all-players-image-dataset) of all the players that participated in the [2022 Fifa World Cup](https://en.wikipedia.org/wiki/2022_FIFA_World_Cup). Many thanks to him for putting together such a wonderful dataset.

<img src="./dataset-card.png" height="300">

## General Information

The FIFA World Cup is a professional football tournament held between national football teams, organised by FIFA. The 2022 FWC took place in Qatar from 20th November to 18th December 2022. Argentina were crowned the champions after winning the final against the defending champions France 4–2 on penalties following a 3–3 draw after extra time.

This is an image dataset of 45 of the most elite players that participated in the 2022 FWC. I tailored it to suit an ML project I was working on. The player selection was borne out of my personal opinions and biases, and does not necessarily reflect (current) consensus nor reality. (Yes, Eden Hazard, one of the greatest ever to grace the Premier League is included. 😎 How on earth was Rodrigo De Paul included? Well, if you know you know. 😉)

Unfortunately, since the original dataset by nature only comprised teams that qualified for the World Cup, there are quite a few elite players that were left out (sorry Zinchenko, Ødegaard, Salah, Osimhen, Haaland).

Also, owing to the method utilized to create it (web scraping), the original dataset contained several mistakes (cases of mistaken identity and so on); I have done my best to correct them, i.e, delete and move images accordingly.

Furthermore, in the process of working with the dataset, I realized that real world images of these players will tend to contain multiple players. It would not do, therefore, for the dataset to only contain solo images of the players, as the models we train thus would be fragile, and would fail when provided with images containing more than one player.

Accordingly, in cases where an image contained other players found in the dataset, I copied the image into those players directories as well. This does add quite a bit of noise to the data, so to speak, but there's no way around it if we want to build robust models that are as close to reality as possible.

## Dataset Overview

- The dataset is contains 4 folders that represent different positions on the pitch, namely: _Goalkeepers_, _Defenders_, _Midfielders_ and _Forwards_.
- Each position folder contains several folders of the most elite players in that position.
- Each player folder contains around 40 to 60 images of that player.

That will be all. Go forth and build cool things with the dataset.
