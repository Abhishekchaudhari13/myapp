# reactjs-onboarding
----------------------------------------------------------


> Better introductions for websites and features with a step-by-step guide for your projects. 

[![NPM](https://img.shields.io/npm/v/reactjs-onboarding.svg)](https://www.npmjs.com/package/reactjs-onboarding) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)


![grab-landing-page](https://media.giphy.com/media/hQu9D1RzMJolsjtvbL/giphy.gif)

## Install
----------------------------------------------------------

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

**1)** This github repository, using ```git clone```

**2)** Using npm ```npm install reactjs-onboarding.js --save```


## Usage
----------------------------------------------------------


reactjs-onboarding.js can be added to your project in four simple steps:



**1)** Include named imports of `Onboarding.js` and `OnboardingItem.js` in your project



```jsx
import {Onboarding} from 'reactjs-onboarding'
import {OnboardingItem} from 'reactjs-onboarding'
```


**2)** Create a state variable `visible` in the class and set it to false



```jsx
state = { visible:false };
```


**3)** Set `visible` parameter to true when you want the Onboarding to get called



```jsx
  this.setState({ visible: true })
```


**4)** Passing the coordinates


* Give unique Id to the element that you want to point the arrow to


```jsx
<div id="example">
 Pass the co-ordinates by id
</div>
<Onboarding name="testing" visible={this.state.visible}>
  <OnboardingItem elementCoOrdinate="example" message="This is the onborading message 1" />
</Onboarding>

```

* Give unique reference to the element you want to point the arrow to


```jsx
<div ref={(e) => this.reference = e}
 Pass the co-ordinates by reference
</div>
<Onboarding name="testing" visible={this.state.visible}>
  <OnboardingItem elementCoOrdinate={this.reference} message="This is the onboarding message 2" />
</Onboarding>

```


## Contributing
----------------------------------------------------------

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.



## License
----------------------------------------------------------


MIT � [](https://github.com/)
