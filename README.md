Our project in the Artathon competition we used 2 different models to produce painting below


The basic idea is to capture any painting as input, then optimize pixels repeatedly to activate a specific channel (feature extractor) in a trained convolutional network. We reproduce the tensorflow recipe here to read the code in detail. In render_naive, we consider img0 entries, then for iter_n steps, we calculate the pixel pitch in relation to our optimization goal, in other words, the difference between all pixels that we must add to activate the target image. The goal of our pass is a channel in one of the network layers, or an entire layer
![Ai](https://user-images.githubusercontent.com/45241728/73133506-9c225d00-403a-11ea-90f1-fff0fd341cad.png)
