## Phase -- 1 ( Project Intialization and cleaning )
* Creating a react project using **npm create vite@latest** .
* Delete unnecessary files & code provided by the default templates, such as CSS, SVG files & the count function snippet in the App.jsx.
* Create a folder named **Hook** then in the Hook folder create a file named *usefetch.js* .

## Phase -- 2 ( In usefetch )
* import hooks like *useState* *useCallback* & *useEffect*.
* Create an arrow function named *usefetch* .
* Create three states *data*, *error* & *loading*, Set the initial value of data and error *null*  & set boolean value "true" for loading.
* Create a constant named *fetchData* and use the useCallback hook to wrap the fetching logic. 
* The two arguments of useCallback is the function itself and the url dependency (for avoid unnecessary re-creation of the function). 
* In the arrow function of useCallback, set setloading to true use the if condition to check the response status and throw an error.. then set setLoading to false in the finally block.
* Use useEffect to trigger fetchData, and include fetchData in the dependency array.
* And in the end return the values (data , error & loading).
