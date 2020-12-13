Optimize Performance for React
==============================

Q01. You have a class component that renders too often. You are pretty sure that it takes immutable data props and that you can rely on reference checking to see if any props changed. What should be your first step in addressing the performance issue?  
A. Ensure that you use the constructor to cache expensive results  
B. Refactor all local state in the component to a Redux store  
C. Extend the component from React.PureComponent  
D. Refactor the component to a functional component  
Answer: Extend the component from React.PureComponent  

Q02. You have a functional component that renders too often, what step should you take to ensure that it renders only when it should?  
A. Wrap the Component definition using React.memo  
B. Ensure that the parent component conditionally renders this component  
C. Use the useMemo hook to ensure that anything expensive is cached  
D. Refactor the component to a class component and use PureComponent  
Answer: Wrap the Component definition using React.memo  

Q03. You deployed your app to production but the bundle size seems excessively high. What do you do first?  
A. Configure gzip compression on your web server  
B. Ensure that your build process is building the app in production mode  
C. Remove all npm modules from your app and handcode everything in your app  
D. Use forEach loops instead of for loops because it requires less code  
Answer: Ensure that your build process is building the app in production mode  

Q04. Your app is starting to take longer to load as it becomes bigger. What could you try to make the initial load faster?  
A. Convert all your components to functional components  
B. Find a better CDN to ensure that your files load as fast as possible  
C. Store your app in localstorage so that it loads faster  
D. Use lazy and Suspense to load sections of the app on demand  
Answer: Use lazy and Suspense to load sections of the app on demand  

Q05. Which of the following best describes a "wasted render"?  
A. When a component takes long to render and wastes CPU and memory resources  
B. When a component renders and it outputs the same markup as its previous render  
C. When a component renders and outputs the same markup as a sibling component  
D. When a component renders and it had side-effects in its render function  
Answer: When a component renders and it outputs the same markup as its previous render  

Q06. Why is it recommended that you use immutable data structures for your React component props?  
A. To embrace functional programming paradigms  
B. To lower memory utilization  
C. It's easier to serialize immutable data  
D. It makes it very difficult to compare props with previous props  
Answer: It makes it very difficult to compare props with previous props  

Q07. What React hook can you use to ensure that a handler function only gets recreated when it should?  
A. useMemo  
B. useCallback  
C. useReducer  
D. useSingleton  
Answer: useCallback  

Q08. You have to derive a value from a functional component's props, but the logic is very CPU intensive. Which of the following is a valid approach?  
A. Combine the useEffect and useState hooks to store the value result  
B. Use the useMemo hook to cache the result  
C. Store the value in localStorage so that you can use it again  
D. Use the useReducer hook to ensure that you record all state changes  
Answer: Use the useMemo hook to cache the result  

Q09. How can you control when the value of useMemo should be updated?  
A. By passing it the correct dependencies  
B. By also implementing `useState` to keep track of changes  
C. By also implementing `useCallback` to reset it when it should be cleared  
D. By also implementing `useEffect` to reset it when it should be cleared  
Answer: By passing it the correct dependencies  

Q10. When you wrap a functional component with `React.memo`, how do you control when it renders?  
A. You specify a function on the second parameter that compares props  
B. You can't because it will automatically do reference comparisons  
C. You have to specify a dependency list on its second parameter  
D. You need to use local state to compare properties  
Answer: You specify a function on the second parameter that compares props  

Q11. What is the recommended way to identify wasted renders?  
A. By doing a performance output build  
B. By adding an npm module that help you track it  
C. By using console.log statements  
D. By using the React performance profiler  
Answer: By using the React performance profiler  

Q12. You have a class component that renders too often. The component receives a lot of data on it's props and some parts of the props require the component to re-render and some do not. How do you proceed in addressing this issue?  
A. Implement the shouldComponentUpdate method  
B. Extend the component from React.PureComponent  
C. Ensure that you store all significant data in local state  
D. Refactor the component to a functional component  
Answer: Implement the shouldComponentUpdate method  

Q13. When you implement `shouldComponentUpdate` in a class component, what does it mean to return true from the method?  
A. It means the props are different enough to require a render  
B. It means that the results should be cached in local state  
C. It means that the component should download a newer version of itself  
D. It means that the props are the same and do not require a render  
Answer: It means the props are different enough to require a render  

Q14. What is the biggest benefit of React's virtual DOM approach?  
A. React can run on the server, without a browser  
B. React can be compatible with more browsers  
C. React does not need to do expensive DOM operations on every render  
D. React renders on a Canvas element which makes it faster  
Answer: React does not need to do expensive DOM operations on every render  