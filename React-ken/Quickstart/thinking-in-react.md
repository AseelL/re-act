
# Thinking in React
- __so basically when we're doing UI we want to think the way react is built / designed.__
we're supposed to break our data down and think or how it can look as a hierarchy.
with that said, there's 3 ways to do that: 
###
1 - think programming-wise : think of making components that have a singular responsibility 
2 - think css : think how different parts of the app will have the same css class
3 - think design: think how you'd organize the layers of the webpage
######
- __start off with static__
do a completely dumb version with no quirks, think hierarchy only, and top-down if small project, bottom-up if bigol' goat
think what static data will go into the components, and make room for them in props.
######
- __think interactivity, go on__
think what should go in a state and what shouldn't 
beware of making too much states everywhere (common noob mistake, don't be a noob)
we have 3 base points to keep in mind if shaytan is telling you to use a state
- is data changing over time?
- is data not passed down from a parent?
- is data not computable based on existing state/props?
if he still convinces you to do it, sure, go ahead, that's probably your guardian angel not shaytan
-__state is alive, where should I shelter her?__
now you know it's certainly alive, think where you should let her live, don't scatter her all over the board, take a step back and plan it out:
- find every component that changes when the state changes
- find the common dominator for these component
- if you find out that they're fatherless,or their father is a good for nothing drunkard , adopt them into a component that its job is solely bearing that state, place it above the father

-__now we make the state actually change and render stuff__
depending on how you built your components to change. again, think of the simplest tools in hand and built-in functions