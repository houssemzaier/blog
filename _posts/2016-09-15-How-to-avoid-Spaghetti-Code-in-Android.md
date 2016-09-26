---
layout: post
title: "How to avoid Spaghetti Code in Android?"
description: "Some useful advices that will avoid you a lot of problems"
#author: "Ajinkya"
coverImg: "SpaghettiCode.jpg"

---

 <h1>How to avoid Spaghetti Code in Android?</h1>
<p>Even if you may love Spaghetti or not, I don’t really think that you are a big fun of <a href="https://fr.wikipedia.org/wiki/Programmation_spaghetti">Spaghetti code</a>…</p>
<p>Whether you are building a complex or simple app, keeping your code clear to be read by other developers is not a simple thing I can say it’s even harder if it’s for a big complex project. 
Remember that when you first start building an app, you don't know how you're going to build everything in it. And when you are working with new team mates they may be not familiar with the way you write and organize your code. So is how can we get a clean code readable and written for humans?  
Here I can recommend some rules known buy code enthusiast and it is not exhaustive... I will try also to give you some samples for client apps using Android as I am a big fun of these two worlds!
So how to organize my code for Android?</p>

<h2>Refactor early, refactor often</h2>
You should know that if we don't continually modify, simplify and unify the existing code along with the new code that's being written, we can easily end up with a really big, messy app.
Sometimes as a developer you may hesitate to touch code you've already written, but believe me deleting and updating code is a regular and one of the most important part of building an app.
I remember when I was told one day during my first internship with LG Electronics: “Don't be scared of refactoring. Be scared of building an unmaintainable piece of crap.”
Running into an ugly code may cost you much more than you may think, even if it was written by yourself. We are humans and humans may forget about many things, so imagine that you come back to and old code that you’d wrote not last months but last year. I think that now you know what I mean. 
In addition to all that, if your app is separated into clean simple modules the risk of accidentally breaking something else is dramatically lower for sure... 

<h2>Choose a style guide</h2>
As you know not all developers have the same coding style, which makes it difficult to understand or work with another developer's code. Consistent coding styles make it easier for other developers to read your code by sticking to a standard set of rules. The solution for me to choose one guide style as a standard for you and your team, and I really recommend that you choose the 
<a href="https://github.com/google/styleguide/blob/gh-pages/intellij-java-google-style.xml"> Google Style Guide </a>.  You can import it into your Android studio as it basically comes from the IntelliJ IDE.
It is very popular and chosen by the creator of the Android SDK. You can more read about it <a href="http://google.github.io/styleguide/javaguide.html">here<a>. 

<p>I recommend also this  Android Best Practices by Futurice, which contains guidelines about things like how to organizing Java files into packages, naming resources for better readability, what to use for testing, dealing with data storage and much more.
</p>
<h2>Choose a client side architecture</h2>
<p>As an Android Architect, whaterver the architecture that you may choose you will have to prepare some arguments. When it comes to the client side apps there is a very common architecture called MV* or MV(whatever). As you may think (M) for the model, (V) for the View part, but what is this star * (or the whatever)? It stands indeed for whatever, as in whatever works for you.
</p>
<p>MVC vs MVVM vs MVP. What a controversial topic that many developers can spend hours and hours debating and arguing about.
For several years Android was closer to MVC, but over time and thanks to many refactorings and api improvements, it's now closer to  MVP or even MVVM with the data-binding library.
Being able to categorize a framework and put it into one of the MV* buckets has some advantages. It can help developers get more comfortable with its apis by making it easier to create a mental model that represents the application that is being built with the framework. It can also help to establish terminology that is used by developers.
This will gives you a lot of flexibility to nicely separate presentation logic from business logic and presentation state. Please use it fuel your productivity and application maintainability rather than heated discussions about things that at the end of the day don't matter that much.
</p>
<p>Well, and because I am a big fun of the MVP design pattern I would love to recommand a very well explained <a href="https://code.tutsplus.com/tutorials/how-to-adopt-model-view-presenter-on-android--cms-26206"> tutorial</a> by a brazilian developer called <a href="http://www.tinmegali.com/en/"> Tin Megali</a>. And for those who want to have a comparaison of the MVP VS MVVM I would also give you this repository that showcases 3 Android app architectures: "Standard Android", MVP and MVVM. The exact same app is built 3 times following the different patterns. <a href="https://github.com/ivacf/archi">Iván Carballo's repo</a>.
</p>

<h3>Conclusion</h3> 
<p>Of course there are many other good practices for clean coding that you can fallow as an Android Developer like the gang of four design pattern, SOLID principles and more... Thinking about to create a nice coding project is good but plase you have always to remember that the main purpose is that you respond to the client's need before any other "meta-work".   	
</p>

<p>Useful Resources:</p> 
<ul>
<li><a href="https://developer.android.com/studio/intro/index.html">Android Studio manual.</a></li>
<li><a href="https://github.com/futurice/android-best-practices">android best practices from futurice.</a></li>
</ul>
