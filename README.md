# React Google Chart(gchart-react)

This is simple and reliable Implementation of Google Chart with React js.

## Live demo 

https://munna.github.io/React-Google-Chart/

## How it is structured

The source code has two separate parts – the library and the documentation (demo) page. Both are written in ES6 and JSX, and therefore have to be transpiled by Babel but in different ways.
## Installation

With your favorite package manager (yarn, pnpm or npm) :
`
yarn add gchart-react
# or
npm i -s gchart-react
`

## Quick Start
`
import React from "react";
import { render } from "react-dom";
import { GoogleChart } from "gchart-react";

export default class App extends React.Component {
  render() {
    return (
      <div className={"my-pretty-chart-container"}>
        <GoogleChart  chart="Pie" style={{height:"300px"}} data={[
  ['Task', 'Hours per Day'],
  ['Work',     11],
  ['Eat',      2],
  ['Commute',  2],
  ['Watch TV', 2],
  ['Sleep',    7]
]} options={{title:"Pie Chart"}}></GoogleChart>
      </div>
    );
  }
}
render(<App />, document.querySelector("#app"));
`
## Other Chart
`
<GoogleChart  chart="Pie" style={{height:"300px"}} data={pieData} options={{title:"Pie Chart"}}></GoogleChart>

 <GoogleChart  chart="Bar" style={{height:"300px"}} data={barData} options={{title:"Pie Chart"}}></GoogleChart>

<GoogleChart  chart="Bubble" style={{height:"300px"}} data={bubbleData} options={{title:"Pie Chart"}}></GoogleChart>

<GoogleChart  chart="Geo" style={{height:"300px"}} data={geoData} options={{title:"Pie Chart"}}></GoogleChart>
<GoogleChart chart="Geo" style={{height:"300px"}} data={geoData} options={{title:"Pie Chart"}}></GoogleChart>
`
## Getting started

Follow these steps to get started developing your own react component:

* `git clone https://github.com/munna/React-Google-Chart.git`
* `npm install`
* `npm run dev` to transpile both the lib and docs folder in watch mode and serve the docs page for you.
* Go to http://127.0.0.1:8000 to see the demo in action. Whenever you change the code in either src/lib or src/docs, the page will automatically update.

