# ReactJS-practise-guidelines
All the react js practise notes and information.
<!-- [comment]: # (Comment should be link this)  -->

<details>
	<summary>All terms and its detail</summary>
	<ul>
		<li>
			<details><summary><strong>Intro</strong></summary>
				<ul>
					<li>Single page Applications</li>
					<li>Build & Reusable UI components</li>
  			</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Virtual DOM</strong></summary>
				<ul>
				 <!--  (Virtual DOM - no contetn, add this later) -->
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>ES6 – ECMAScript 6</strong></summary>
				<ul>
					<li>Classes</li>
					<li><details><summary><strong>Arrow Function</strong></summary>
						<ul>
							<li>Hello = () => { return “Hello There!”;}</li>
							<li>Hello = () => return “Hello There!”;</li>
						</ul>
					</li>
					<li>Vaiables</li>
					<li><details><summary><strong>Array Methods</strong></summary>
						<ul>
							<li>.map() method allows you to run a fxn on each item in the array</li>
							<li>Const myArray = [‘a’,’b,’,c’];</li>
							<li>Const myList = myArray.map((i)=><p>{i}</p>)</li>
						</ul>
					</li>
					<li><details><summary><strong>Destructuring</strong></summary>
						<ul>
							<li>Extract only what is needed</li>
							<li>const vechicles = [“mustang”, “f-150”, “expendition”];</li>
							<li>old: const car = vehicles[0];</li>
							<li>const truck = vechicles[1];</li>
							<li>const suv = vechicles[2];</li>
							<li>new : const [ car, truck, suv ] = vechicles;</li>
							<li>the order that variables are declared is important</li>
							<li>truck cancel out</li>
							<li>const [car,,suv]=vechicles;</li>
							<li>destructuring useful when fxn return array : const [add,sub,mul,div] = cal(4,7);</li>
							<li>obj – obj pass as para only send attributes</li>
							<li>object no specific order </li>
							<li>nested obj : {a,b:{ba,bb}} </li>
						</ul>
					</li>
					<li><details><summary><strong>Spread Operator</strong></summary>
						<ul>
							<li>Copy all or part of array or object</li>
							<li>Used in combination with destructuring</li>
							<li>Ar=[1,2,3,4,5,6,7]</li>
							<li>[one,two, …rest]=Ar</li>
							<li>New property name is new,</li>
							<li>But old property is overwritten</li>
						</ul>
					</li>
					<li><details><summary><strong>Modules</strong></summary>
						<ul>
							<li>Import and export</li>
							<li>In-line : export const name = “arjun”</li>
							<li>At the end: Export {name, age}</li>
							<li>Default export only one</li>
							<li>Import time: named exports or default export</li>
							<li>Named : destructured using { }</li>
						</ul>
					</li>
					<li><details><summary><strong>Ternary Operator</strong></summary>
						&ltCondition&gt ? &lttrue&gt : &ltfalse&gt
					</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Render HTML</strong></summary>
				<ul>
					<li>ReactDOM.render()</li>
					<li>Two args: html code and Html element</li>
					<li>Element not mandatory to root, but it Is stnd conv</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>JSX</strong></summary>
				<ul>
					<li>JavaScript XML</li>
					<li>No createElement and appendChild</li>
					<li>JSX: &lth1&gt I love you &lt/h1&gt </li>
					<li>JSX: React.createElement(‘h1’, {}, ‘I love you’);</li>
					<li>Expression : { 5 + 5} | JS exp</li>
					<li>insert large block of html : html inside parentheses</li>
					<li>html block in One Top Level Element <></></li>
					<li>single tag element must be closed</li>
					<li>class -> className</li>
					<li>if outside JSX or use Ternary</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Components</strong></summary>
				<ul>
					<li>Reusable, =js fxn but work in isolation</li>
					<li>Class | Function Components</li>
					<li>Use the component : &ltName /&gt</li>
					<li>Class Components</li>
					<li>Function Component</li>
					<li>Component inside component</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Class</strong></summary>
				<ul>
					<li>skip for now</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Props</strong></summary>
				<ul>
					<li>Properties – arguments in js and attributes in html</li>
					<li>To pass add attributes &lt Car brand=”ford”/&gt</li>
					<li>Fxn’s (props) {props.brand}</li>
					<li>Pass data from Component to Component</li>
					<li>Brand=”name” for string</li>
					<li>Brand={ carName} for variable / object</li>
					<li>Props are read only. If change = error</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Events</strong></summary>
				<ul>
					<li>onClick instead of onclick</li>
					<li>onClick={shoot} , not onClick=”shoot()”</li>
					<li>onClick={arrow fxn} – to pass </li>
					<li>react event object: event.type</li> 
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Conditionals</strong></summary>
				<ul>
					<li>&& - true-condition && render</li>					
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>List</strong></summary>
				<ul>
					<li>List – Garage in car list</li>
					<li>Cars – including car list</li>
					<li>Cars – list</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Forms</strong></summary>
				<ul>
					<li>HTML – DOM | React – component</li>
					<li>Control changes by event handler</li>
					<li>useState Hook to keep track of inputs</li>
					<li>slight change in textarea and select, it handle a;; input elements in the same way</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Router</strong></summary>
				<ul>
					<li>Add react router: npm i –D react-router-dom</li>
					<li>Src/pages/Home.js|Blogs.js|Contact.js</li>
					<li>&ltRouter&gt wrap</li>
					<li>&ltLink&gt set URL and track browsing history</li>
					<li>&ltLink to=”/”&gt instead of &lta href=””></li>
					<li>&ltSwitch&gt similar to switch  in JS, it render &ltRouter that matches &ltLink&gt</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Memo</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>CSS Styling</strong></summary>
				<ul>
					<li>Inline Styling {{}} double curly | camelCase</li>
					<li>CSS Stylesheets – making new .css</li>
					<li>CSS Modules – only the imported component can use</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Sass Styling</strong></summary>
				<ul>
					<li>CSS pre-prossor</li>
					<li>Executed on server and send css to browser</li>
					<li>Npm I sass : install sass</li>
					<li>Like css with .scss – use var and othe scss fxn</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Hook</strong></summary>
				<ul>
					<li>Since –v 16.8</li>
					<li>Allow fxn comp to have access to state and other React features. Class comp no longer needed</li>
					<li>Allow us to “Hook” into react features such as state and lifecycle methods</li>
					<li>useState Hook to keep track of the application state. State refers to application data and properties</li>
					<li>rule : only called inside React Fxn component</li>
					<li>rule : only called at top level of a component</li>
					<li>rule : cannot be conditional</li>
					<li>not work in class component</li>
					<li>if you have stateful logic that needs to be reused in several components, build custom Hooks </li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useState</strong></summary>
				<ul>
					<li>Named export so import {useState}</li>
					<li>initialize by calling useState in our fxn component</li>
					<li>accepts an initial state  and return 2 values</li>
					<li>the current state | a fxn that updates the state</li>
					<li>const [color, setColor] = useState(“”)</li>
					<li>color is current state | setColor is fxn that update our state</li>
					<li>useState(“”) is initial state</li>
					<li>now can use {color} anywhere in the fxn component</li>
					<li>no direct update like color = “red” but setColor(“red”)</li>
					<li>if object then call by obj.attributes, and update by setObject ( () => {attr1:””, attr2:””});</li>
					<li>object : setCar({color: “blue”}) – removes other attributes</li>
					<li>object all attributes change and only one attributes change</li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useEffect</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useContext</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useRef</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useReducer</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>useCallback</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
		<li>
			<details><summary><strong>Custom Hooks</strong></summary>
				<ul>
					<li></li>
				</ul>
			</details>
		</li>
	</ul>
</details>
