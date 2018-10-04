# Whiskers, Ears and Puppy Dog Tails: finding out what animal pictures are made of

![inline](7a2aa472bbe9a7ecc1985a699c7fe90b973e9ac87f678f979743342f19840b31/thumbnail_medium_haar_cat2_eyes.jpg)

---

# Who am I? Why am I doing this?

* ![inline](bonce.jpg) Mike Moran, Engineer at Skyscanner
* Adopt Animals
* Skyscanner “One Day”
* A general Machine Learning interest

---

# Context: Adopt Animals

![inline](adopt_animals.png)![inline](kale-logo.png)


— [Adopt Animals](https://www.adoptanimals.io/), by [Kale](https://www.kale.org.uk/) charity


---

# What were we trying to do?

![inline](requirement.png)

— ([Sky](https://twitter.com/carrotcodes]) of Adopt Animals)

---

# My constraints

* I ~~am lazy~~ have limited time, so an off-the-shelf solution would be good
* I am *not* a Jupyter expert (yet?)
* I have a non-uniform experience of Data-science algorithms

---

# Ok, so how do I get to this?

![inline](7a2aa472bbe9a7ecc1985a699c7fe90b973e9ac87f678f979743342f19840b31/thumbnail_medium_haar_cat2_eyes.jpg)

---

# Going with something I know: Viola Jones face detection

![left](https://raw.githubusercontent.com/mikemoraned/selfies/master/examples/touristselfies/CLdKagoWoAA379-.faces.jpg)

— from [“Looking for Bobby but found Paris instead”](http://blog.houseofmoran.com/post/126043044893/looking-for-bobby-but-found-paris-instead)

---

# Training: Haar features

![inline](https://www.researchgate.net/profile/Nguyen_Thai-Nghe/publication/278783423/figure/fig2/AS:294390556839937@1447199586590/Haar-like-features-Source-opencvorg.png) ![inline](https://www.researchgate.net/profile/Tomas_Proscevicius2/publication/237049645/figure/fig1/AS:299454470082567@1448406917463/Haar-features-examples-for-face-detection.png)

---

# Training: Adaboost

![inline](https://slideplayer.com/slide/9092209/27/images/20/Algorithm+Adaboost+-+Example.jpg)

---

# Applying: Image Pyramid

* deals with varying feature size

![inline](https://www.pyimagesearch.com/wp-content/uploads/2015/03/pyramid_example.png)

---

# Applying: Integral Image

* efficiently evaluates hear features; O(n²) ➡ O(1)

![inline](https://computersciencesource.files.wordpress.com/2010/09/adding_2.png)![inline](https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Summed_area_table.png/220px-Summed_area_table.png)

---

# Applying: Haar cascade

![inline](http://lh5.ggpht.com/-ui_sWzegVLw/UDMAh6MKx8I/AAAAAAAAKxQ/wdgMMAZW0k0/image_thumb20.png?imgmax=800)

---

# Visualising applying to image

![inline autoplay](https://youtu.be/hPCTwxF0qf4?t=55s)

[YouTube visualisation by Adam Harvey]()

---

# Re-using an off-the-shelf model

![left 75%](detecting_cats.png)

from [pyimagesearch](https://www.pyimagesearch.com/2016/06/20/detecting-cats-in-images-with-opencv/), using a pre-trained cat model from [Joseph Howse](https://twitter.com/CatsAndMonkeys)

---

# Where have I gotten to in this? Job done, ye?

![inline](0b47f51b281802e5b262855dfe84419218df247a9c193ae339ef06774ae5b572/thumbnail_medium_haar_cat2_eyes.jpg)![inline](1c8ca65d3a8a7b547516208313caad43ba347ad9fe836dd68d4af1e05c59d7cf/thumbnail_medium_haar_cat2_eyes.jpg)

---

# Not so fast

![inline](3bc4d1542de3ff380b80713a9dbac2558348603f55b92f9d2ad69608a83d0792/thumbnail_medium_haar_cat2_eyes.jpg)![inline](57ac8ce8c5644c0e7e269a0dd54323d5c931130e5313ca4c6b19f4b42c26f091/thumbnail_medium_haar_cat2_eyes.jpg)


---

# Visualising varying min_size

![loop autoplay](summary_cat.avi)
![loop autoplay](summary_eye.avi)

---

# Learnings / Reinforcements

* Maybe *too* lazy in not focussing on understanding e.g. playing with scale-size instead of max-size parameters. Became clear once I actually spent some time on it.
* Some parameters still seem like magic (min neighbours = 5)
* You don't have to be an expert to be helpful

---

# Backing up: what next?

* Productionising the cats-only thumbnails
* Pre-learned Dogs?
* Auto-learning of parameters on top of same algorithm
* #HASHTAG DEEP LEARNING?
  * Deep learning is expensive, both in terms of cpu cost and collecting of training data, is it worth it?

---

# Thanks / Contact details / Questions

![inline left 35%](RjFZp_zg_400x400.jpg)[Sky](https://twitter.com/carrotcodes]) of [Adopt Animals](https://www.adoptanimals.io/), https://twitter.com/carrotcodes

![inline left 35%](kale-logo.png) [Kale Charity](https://www.kale.org.uk/), https://www.kale.org.uk/ 

![inline left 120%](bonce.jpg) [(that’s me)](https://twitter.com/mike_moran), https://twitter.com/mike_moran

