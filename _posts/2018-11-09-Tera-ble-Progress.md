---
title: Tera-ble Progress
date: 2018-11-09 15:47
---
### A more modular hyena
Our dear friend, and colleague Arlo (aka Asonix), has once again blessed us with several metric tonnes of code.  Not the least of which is a more modular backend.  Short version, 
it is now possible to build with either Rocket.rs, or Actix.  This is really cool because it means that we can do some serious side-by-side testing down the road.  It also has the 
benefit of providing more choices.  Sadly I am not *quite* versed enough to explain why choose one over the other but hey, glad to have the option ;)

<br />
Just a few moments ago [PR #159](https://github.com/Aardwolf-Social/aardwolf/pull/159) was merged, thus finally nailing down Tera as our templating language (syntax?) of choice!
Also included in this is the i18n translation functionality, which has become a pretty important part of the project.  Unfortunately these translations are only with the aardwolf-rocket
feature, and will not (yet) work on Actix.  Given that the i18n_rocket crate (what we are using for the i18n support) will soon see a major update the decision has been made to hold off 
on making it work with Actix.  Once the updates have been released, we will look at it with fresh eyes.

Cheers!

- Banjo

<br />
***
