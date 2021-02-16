# Variational_Autoencoder_MNIST_Dataset

Okay !! Now let's talk about the Variational AutoEncoder

# Variational Autoencoder

Variational autoencoder (VAE), one of the approaches to unsupervised learning of complicated distributions. A VAE could do compressing data, reconstructing noisy or corrupted data, interpolating between real data, and are capable of sourcing new concepts and connections from copious amounts of unlabelled data. VAEs are built on top of neural networks.

**A variational autoencoder (VAE) provides a probabilistic manner for describing an observation in latent space. Thus, rather than building an encoder which outputs a single value to describe each latent state attribute, we'll formulate our encoder to describe a probability distribution for each latent attribute.**

So, What the heck mean by probability distribution in the latent space ?
- **Autoencoder** : What we did in autoencoder is we take input and encoding them and store the information in 3D or 5D latent space. And from the bottleneck, we start reconstructing the output with minimum loss function. 
- **VAE** :  We take unlabel input images and apply encoder, then in the latent space we divided into two distribution which are (mean & standard deviation) and other one is sample distribution. We take sample distribution from the mean & standard deviation and from that distribution tried to reconstruct the output with minimum loss. The pictorial view of VAE
<img src = "https://raw.githubusercontent.com/skeydan/whyR2019/master/vae.png">

Let's see an example of the distribution:
<img src = "https://www.jeremyjordan.me/content/images/2018/06/Screen-Shot-2018-06-20-at-2.48.42-PM.png">

Okay now see how the loss function minimize. In the variational autoencoder the loss function is little complex to understand.

One of the approch is the Varitational inference. For this we need to minimize the KL divergence and maximize the marginal likelihood


---

[Jeremy Jordan](https://www.jeremyjordan.me/variational-autoencoders/)<br>
**[Math Expation by Ali Ghodsi](https://youtu.be/uaaqyVS9-rM?list=LL)**<br>
[Math Details](https://davidstutz.de/the-mathematics-of-variational-auto-encoders/)<br>
[Understanding Variational Autoencoders (VAEs)](https://jaan.io/what-is-variational-autoencoder-vae-tutorial/)<br>
[Paper](https://arxiv.org/abs/1312.6114)
