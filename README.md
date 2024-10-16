Team name: Tomi és Réka

Team members: Szűcs Tamás (BGDOMU), Boros Réka (AF6LRA)

Project description: Image generation with diffusion models

A projekt célja, hogy két különböző diffúziós modellt (a Denoising Diffusion Probabilistic Modelt (DDPM) és a Denoising Diffusion Implicit Modelt (DDIM)) implementáljuk és betanítsuk, majd ezek segítségével valósághű képeket generáljunk két különböző adatkészleten: a CelebA és a Flowers102 adatokon.

Az első cél a DDPM (Denoising Diffusion Probabilistic Model) megvalósítása. Ez a modell iteratív zajcsökkentési folyamatot alkalmaz, ahol egy kép zajjal kerül bevezetésre, és a modell fokozatosan tanulja meg, hogyan állítsa vissza az eredeti, zajmentes képet.

A második cél a DDIM (Denoising Diffusion Implicit Model) implementálása, amely a DDPM egy optimalizált változata. A DDIM determinisztikus mintavételezést biztosít, így gyorsabb képgenerálást tesz lehetővé, miközben a generált képek minősége nem csökken.
    
Functions of the files in the repository:

image_generation.ipynb: Ez a nootbook tartalmazza az adatok letöltését és előkészítését, a modellt, valamit a tanító ciklust (jelenleg csak az adatok letöltését és előkészítését).
    
requierments.txt: Tartalmazza a szükséges python package-eket verziószámokkal, pip install -r requirements.txt command segítségével a megfelelő könyvtárak telepíthetőek.
    
Related works:

https://arxiv.org/pdf/2006.11239

https://arxiv.org/pdf/2105.05233

Az első cikkben, kiváló minőségű képgenerálást értek el diffúziós probabilisztikus modellekkel (DDPM) a CIFAR10 és a 256x256 LSUN adatkészleteken. A legjobb eredményeinket egy olyan súlyozott variációs határ alapján érték el, amely egy új kapcsolatot használ a diffúziós probabilisztikus modellek és a denoising score matching, valamint a Langevin-dinamika között.

A második cikkben bemutatják a denoising diffusion implicit modelleket (DDIM-eket), amelyek gyorsabb mintavételezést tesznek lehetővé ugyanazzal a tanítási folyamattal, mint a DDPM-ek. A DDIM-ek nem-Markov diffúziós folyamatokat használnak, amelyek gyorsabb generálást eredményeznek, és 10×-50× gyorsabban állítanak elő mintákat.



