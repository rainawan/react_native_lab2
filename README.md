# ⚡️React Native Lab 2

Welcome to this crash course on how to create a mobile app with React Native! Today's lab has three parts. We're gonna make a **UberEats / DoorDash / Postmates / GrubHub clone**!

### To run

1. Fork this repo!
2. Git clone the forked repo.
3. In your terminal, run `yarn install`
4. Then launch the project with `expo start`

### Remember, the first time you clone a React Native repo, you'll need to `yarn install`!

There are some `TODO` comments in the code to help you along. Feel free to delete them when you're done with the task.

# Part 1: Custom Component with Props

We're gonna spruce up out `MenuItem` component by using props! Recall that we can access props using the `props` variable that gets passed into our component function. We access a specific prop by doing `props.propName`. And the props are *passed into* our component by doing `<ComponentName propName={propValue} />`.

Top Tip: When you want to use JavaScript variables or code within JSX code, you need to put it inside curly braces `{}`

[https://reactnative.dev/docs/intro-react#custom-components](https://reactnative.dev/docs/intro-react#custom-components)

[https://reactnative.dev/docs/intro-react#props](https://reactnative.dev/docs/intro-react#props)

1. Update the props in the `<MenuItem ... />` component in `App.js` with a new name, price, and image source. Remember that image source has to be using `require(...)` or `{uri: "..."}`. **NOTE**: you won't see any changes yet. We still need to update our component to *use these props*...
2. Go to `MenuItem.js`. Update the FOOD NAME to use the `name` prop.
3. Update the price to use the `price` prop
4. Update the image source to use the `imageSource` prop

Amazing! Look at that delicious food 😋.

### 👇🏼 When you're finished with part 1, add a screenshot to the Google Classroom 👇🏼

[React Native Lab 2](https://classroom.google.com/c/NTAwNzM2MDgwMzgy/a/NDk2ODc2Mjg4NzMz/details)

# Part 2: State

Every React component has the ability to keep track of its own **state**. We're gonna keep track of the desired *quantity* for each menu item.

[https://reactnative.dev/docs/intro-react#state](https://reactnative.dev/docs/intro-react#state)

1. First things first, let's go to `App.js` make another `<MenuItem ...>` ! You can copy and paste, and change the name, price, and image source to another food item. Wow! So easy! Hooray for reusable components!
2. Now let's go back to `MenuItem.js` and look at the `useState(0)` . **Discuss with your partner:** what does this line do? Check out the link above for more info.
3. In the "plus button" `onPress` function, try doing `quantity++` to increase the quantity state directly. What goes wrong? **Discuss with dat partner of yours!**
4. Now try again with `setQuantity()` . Yay! Why does this work? Why do we need to do this? #**DISCUSS**
5. Update the `onPress` function for the "minus" button to *decrease* the quantity. Don't let the quantity go negative!

Now play around with those buttons! Notice how each menu item keeps track of its own quantity. Hooray for reusable components, again!

# Part 3: TextInput

Last but not least, we're gonna add the ability for “Special Instructions” in case you want extra cheese, or less ice!

[https://reactnative.dev/docs/textinput](https://reactnative.dev/docs/textinput)

1. Make a **new state variable** for the special instructions text
2. Use that new state variable in the “Special Instructions: {}” `<Text>` component
3. Update that state variable in the `onSubmitEditing` function of the `<TextInput>` component

You did it!! A nice custom component, complete with multiple props and multiple state variables!

# [Optional] Part 4: Extensions

- Do some fancy styling! Make that main page and those menu items look ~~~beautiful ✨
- Add another prop to `MenuItem` !
- Make another custom component from scratch!
