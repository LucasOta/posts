#React: thoughts from an Angular developer

After two years working with [Angular](https://angular.io/) I was assigned to a project where the frontend stack was [React](https://reactjs.org/), [Next.js](https://nextjs.org/) and [Chakra UI](https://chakra-ui.com/). I started without any prior React experience nor knowledge. After three months in this project I’ve decided to put my thoughts of this technology change into a post.

>Disclaimer: this won’t be a full Angular vs React post, but my thoughts about what I like and don’t like about React, what I miss from Angular, etc. Also take into consideration that I’ve only been working with React for 3 months.

#From a Framework (Angular) to a Library (React)
This was one of the biggest changes for me, Angular already provides you a way to do things, elements to help with authentication (Guards), endpoints handling (Interceptors), Routing, Pipes, tools (such as the beloved Angular CLI), etc.
As React is just a library, it’s on you to generate all those things, or to search another external tool or library.

##In React most features must be created from scratch
Let’s suppose that we need to show an alert on our application every time an endpoint returns an error.
In Angular we can just go to the [CLI](https://angular.io/cli), create a new Interceptor with the logic of reading the error and calling an alert, then use the interceptor from the app.module and we are ready to go.
On the other hand, React doesn't provide us with built-in magic to do this. We could use [Redux-Saga](https://redux-saga.js.org/), create an architecture for it to be reusable, think everything from scratch.

##Routing
Since I haven’t worked with pure React, but with Next.js, I’m going to compare its [routing system](https://nextjs.org/docs/routing/introduction) to the [Angular Router](https://angular.io/guide/router).
Nextjs handles routing based on the folder structure inside the *pages/* directory, this is very easy to learn and doesn't need any configuration at all. For simple projects I look at it as a great advantage.
I consider that the Angular Router is a much more powerful and versatile tool, with it you can handle Lazy Loading as you need, and redirection is much more easy than in Nextjs.

##Architecture
In my case, I don’t have a lot of experience in development and even though I was able to start several Angular projects by myself and not die trying since it provides you a way to organize directories (even though you can customize it based on your needs). 
Oppositely, if I had to create a relatively big application by myself with React in this moment of my career, it would be very painful for me to create something well organized and scalable (now that I’ve worked on a project with a lovely architecture created by very experienced React developers it would be easier for sure).

#Javascript after Typescript
Before I started working with React, I loved [TS](https://www.typescriptlang.org/) and I thought that it was a must to have within any application. I learned that it isn’t correct, you can work in a very well organized way by using only javascript and a good Text editor or IDE. Also, if you don’t use Typescript well, it can become a real pain in the neck.
I don’t  think Typescript is useless, I still believe that there are many scenarios in which TS can be a real lifesaver (really big projects, or projects with a lot of different entities).
Another thing that I’ve noticed when using React is that I had to learn much javascript, ES6 syntax is a must, also I wasn’t used to work with `.map` or generator functions.  (This can be also because in this project I’ve worked with real javascript lovers) 

#I really miss the Angular CLI
The ability to create any element you need (Module, Component, Service, you name it) in a single prompt command without having misspelling errors in the code is a real time saver, also by using it, you don’t have to worry about the file structure, which imports you need, etc.

#Simpler files
If you create a new component in Angular, by default it creates three files (and a fourth one if it`s a module) one for the template (HTML), one for styles and the other one to handle all the logic. You can reduce it into one sometimes, but I think that React, by using JSX, handles this in a much more efficient and cleaner way.
Also, by having less files, the project is more maintainable, cleaner and less intimidating to new developers.

#Learning curve
I had heard that React’s learning curve was smaller than Angular’s, but I didn’t understand why until I started with React. If you had to create a simple website with few pages, with React it would be very easy and simple as you don’t need to know a lot of stuff. On the other hand, to do that on angular you’ll have to learn first: Typescript, Routing, Modules, Services, Interceptors, Guards, Pipes, among others things you may need based on your needs.

#Conclusion
I still have a lot to learn about both technologies, but now I know that both have pros and cons, different use cases and it is not one or the other. The next time I have to create a new project I’ll surely be doing a deep research and evaluation before choosing between Angular or React (or other frameworks or libraries that I haven’t tested yet).
I hope this has been in some way helpful for you. May the force be with you.
