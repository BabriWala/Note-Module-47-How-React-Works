

<details><summary>What is NPM</summary>
<p>
<b>NPM</b> stands for Node Package Manager. It is a Javascript package manager and the default package manager for Node projects. NPM is installed when NodeJS is installed on a machine. It comes with a command-line interface (CLI) used to interact with the online database of NPM. This database is called the NPM Registry, and it hosts public and private 'packages.' To add or update packages, we use the NPM CLI to interact with this database.

<br>
<b>Isaac Z</b>. Schlueter developed NPM purely in Javascript. It was first released in November 2010. Ever since, NPM has had a lot of updates and has improved in terms of efficiency, speed and security. 

</p>
</details>
<br>
<details><summary>What is NPX</summary>
<p>
<b>NPX</b> stands for Node Package eXecute. It is simply an NPM package runner. It allows developers to execute any Javascript Package available on the NPM registry without even installing it. NPX is installed automatically with NPM version 5.2.0 and above.
</p>
</details>
<br>

<details><summary>What is Create React App</summary>
<p>
<b>Create</b>React App is a comfortable environment for learning React, and is the best way to start building a new single-page application in React. It sets up your development environment so that you can use the latest JavaScript features, provides a nice developer experience, and optimizes your app for production.ed automatically with NPM version 5.2.0 and above.
</p>
</details>
<br>

 [Read Me File Foramtting Link](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

>ctrl shift p = markdown preview || Ctrl + Shift + V

**package.json vs package.lock.json**

<details><summary>What is Babel</summary>
<p>
Babel Holo free and open source JS transpiler(Translate compiler) ja Ecmascript er newer version k previous version e convert kore kajer subidharthe.
</p>
</details>
<br>

<details><summary>What is JSX</summary>
<ul>
    <li>JavasCript XML</li>
    <li>JSX er Shajje html code gulo Javascript er modde sohojei lekha jai. abar html code er modde o javascript expression gulo bebohar kora jai curly braces er sahajje.</li>
    <li>Markup language & logic k alada file e na rekhe ekoi sathe proyojon moto akoi file  e rakha jai er jonno react component bebohar korte hoi</li>
</ul>
</details>
<br>

<details><summary>What are the advantages of using JSX in ReactJS ?</summary>
<ul>
    <li>JSX helps us in keeping our code simpler and elegant when writing large pieces of code.</li>
    <li>According to the React docs, most people find it helpful as a visual aid when working with UI inside the JavaScript code.</li>
    <li>JSX also allows React to show more useful error and warning messages.</li>
    <li>If one is familiar with HTML, it is quite easy to use JSX when building React application</li>
    <li>Faster than normal JavaScript as it performs optimizations while translating to regular JavaScript.</li>
</ul>
</details>
<br>

[For more Reading About JSX Depth](https://reactjs.org/docs/jsx-in-depth.html)


> Unidirectional data flow (One way Binding). Jodi parent tike kisu pathai taile child seta read only hisebe pai se kono change korte parbena tokhon tobe parent e giye change korte partbe. 

>Props Drilling / one way binding

[React Component Article](https://reactjs.org/docs/components-and-props.html)

>State ta j change hoi oita holo ascyncronous way te


```
 const [steps, setSteps] = useState(0);

    const increaseSteps = () => {
        const newStepsCount = steps + 1;
        setSteps(newStepsCount);
        console.log(steps)
    }


//Eikhane ei console log ta hobe na thik moto karon holo eita ascyncronous way te kaj kore jar fole eita tar asol behaviour pabena. Tai amdr uchit use effect ta use kora
```

```
 useEffect( ()=>{
        console.log(steps);
    }, [steps]);

// eikane dependencies list second parameter ta jar fole oi dependencies ta jotobar change hobe totobar ei useeffect ta cholbe.
```

>Hook holo special function

>Akta components er state k apnar child component k o pass kora jai

- props are read only
- props cannot be modified
----------
- state changes can be asynchronous
- state can be modified using this.setState

> jeikhane state tak change kora hoi oitak bole stateful component