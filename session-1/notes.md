**Intro to Vue – Content**

**Why Frameworks?**

![](RackMultipart20200817-4-1yju7e9_html_9017d5de299768d1.png)

Let&#39;s consider a scenario, as illustrated above, where there are 2 inputs to be given by the user and after submitting the form the inputs will be added to the table below. When the page is first loaded, the above picture is the initial view. Suppose we think of implementing without using any frameworks, it would entail using html and css for the static structure of the page while using vanilla javascript to take care of the dynamic content.

Suppose we think of implementing this in vanilla javascript, for the initial load, an array of objects will hold the data. There will be a block of code loading this data, which will be called at the initial page load. When we add a new data using the form, the new object will be added to that array and the function for updating the table, will be run again. Suppose on top of this, we add a delete functionality, this will make the code more complex because that would require a click event listener to delete the row and then again the function will be called to update the UI.

For the simple functionality of adding a new row to the table, we have to write huge code just to update the UI and keep it in sync with the internal data. The more complex the page becomes in terms of features and UI, the more lines of code is added and it becomes all the more difficult to write logic to ensure the code doesn&#39;t break anywhere. If we consider such naïve implementation with huge data we get from server, that&#39;s a huge DOM manipulation for every state change. So in a nutshell, implementing even the simplest scenario using vanilla javascript is a tedious process and involves writing a lot of fragile code.

The ability to sync UI with the internal state of the application, is therefore the biggest advantage of using frameworks. As long as you pertain the frameworks rules and don&#39;t mess with them, you will be able to sync data with UI seamlessly.

**Other Advantages:**

- Frameworks are based on modularity.
- They have debugging tools to make this process easier.

**Angular and React**

Both angular and react though achieving the same goals, have fundamentally different guiding and design principles.

**The first difference comes in the approach of syncing UI with internal state.**

React re-renders the whole DOM for any state change. So when parent re-renders, it triggers rendering of all of it&#39;s children whether they were affected by the change or not.

In Angular the changes are traced so only the affected part of the DOM is rendered on state change.

**Data flow**

Data binding/flow is one way in react. The data flows from parent to child. For updating any data back, additional handlers have to be added.

Angular provides a way to do two-way binging as well. So it&#39;s used for simplicity purpose.

**Design**

Both angular and react have component based architecture and are very similar.

**Structure**

Angular is designed to support all needs and requirements of web application. It&#39;s more structured and the expectation is to use tools provided by angular for various requirements such as api calls, routing, etc. React gives the developer flexibility to use any library to fulfill the requirements of a web application.

**Popularity**

Both angular and react have it&#39;s pros and cons. React is more flexible. You can pair it up with any library for your use cases. React is in javascript. So it&#39;s more adaptable in contrast to typescript as developers don&#39;t want to pick that up. Unless you come from C++ or C# background, developers have aversions to picking up typescript. Therefore react&#39;s flexibility and the fact that it uses javascript, makes it more popular.

Angular is more structure and has a steep learning curve. In addition to this it requires learning typescript. So new developers are less inclined to learn that. Unless a developer feels certain preference for type restricted applications, they don&#39;t flock towards Angular. But main advantage of angular is, if someone doesn&#39;t know which technologies is best to start with, angular is perfect for them as it has all the toolset required for building an application. Unless there is an expert on React and has a curated toolset to use it with, angular is the go to option.

Though not liked by most developers, typescript is the main advantage of using angular. The structure it has is suitable for big applications and no one knows where to start.

In practical usage it&#39;s up to preferences as both Angular and React are extensive frameworks backed by Google and Facebook respectively and therefore wide community support.

**Guiding Principles of Vue**

In terms of design principles, Vue is very similar to React. It&#39;s lightweight and flexible. It has the component architecture and data flow mechanism as that of React but it has also picked some good syntaxes from angular.

The guiding principle of Vue though, is to **make it easy to use and incremental in terms of adaptation**. For starting any of the other frameworks you need to have knowledge of plethora of technologies. Though the technology required are very much worth learning, there isn&#39;t a clear distinct learning path defined, which every one

**For Vue, all you need to know is HTML, CSS and JS and you can start from there.**

With limited knowledge of javascript and knowledge of html, css it&#39;s the easiest framework to learn. **Easy to get productive as well.**

Also Vue provides the capability of importing / using parts of it. If you want to focus on just the view layer i.e html, css then you can use vue with inclusion of a simple cdn. For more feature such as routing, state management, vue has libraries which you can import as per your needs. It doesn&#39;t have to be all or none. Hooking up Vue to existing solution is also very straightforward.

Vuejs provides the perfect learning path to start with building simple apps to building full scale applications.