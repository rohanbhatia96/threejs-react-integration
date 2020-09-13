# threejs-react-integration

## What Is The Project?
This is a simple project I made to show how [three.js](https://threejs.org/) can be integrated with React without using any wrapper libraries./
This was done for a tutorial I wrote on my personal blog.

## Link Of Tutorial

[Integrating Three.js And React Without Wrapper Libraries](https://therohanbhatia.com/blog/integrating-three-js-with-react/)

## Why Is This Project Relevant?

You can't simply import three.js in React and start using because you’ll face these two problems:

1. If you follow the official docs, you’ll be manipulating the real dom and not the react-dom so technically your 3D scene would be running on top of the react app. Due to this, your 3D component won’t follow the component hierarchy of your react app.
2. The other components in your react app won’t be able to interact with the 3D scene. And more importantly you won’t be able to manipulate your 3D scene with any react functionalities like hooks.

My blog post provides a solution for these problems. After following the tutorial, you would be able to:

1. Inject three.js into the react-dom instead of the real dom.
2. Control your three.js renders with react components like buttons using the useRef hook.

[Read the blog post](https://therohanbhatia.com/blog/integrating-three-js-with-react/)