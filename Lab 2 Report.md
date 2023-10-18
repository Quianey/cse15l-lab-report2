Part 1
**Code for StringServer:**
![StringServer](https://github.com/Quianey/cse15l-lab-report2/assets/147276821/913880ab-74dc-4b34-ab4f-a297c96e1e55)

**Using /add-message**

![first add](https://github.com/Quianey/cse15l-lab-report2/assets/147276821/1400b220-bbe9-46f5-8a38-83c7011dab1f)
![second add](https://github.com/Quianey/cse15l-lab-report2/assets/147276821/59650fb0-3674-44b9-bb25-e531219c0ea3)

**Which methods in your code are called?**
public String handleRequest(URI url) is called. 

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
For the first call, the argument is *https://0-0-0-0-4000-vtn7ngm7vnn9jo8sc7nmgpo88o.us.edusercontent.com/add-message?s=Hello*
For the second call, the argument is *https://0-0-0-0-4000-vtn7ngm7vnn9jo8sc7nmgpo88o.us.edusercontent.com/add-message?s=How%20are%20you*
*https://0-0-0-0-4000-vtn7ngm7vnn9jo8sc7nmgpo88o.us.edusercontent.com* is domain
*/add-message* is path
*?s=Hello* and *?s=How%20are%20you* are qiery. 
When the method is called, java will first find */add-message* in the url. Then, it will split the queryto *s* and *Hello*, for example. Then, if will check the first part of query. In our example, it is *s*, so this pass the if statement. *num*, which is the count of lines, will plus one. And what we want to print on the web will be stored into *result*. Finally, it return result. 

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**
*num* and *result* get changed. 
For the first call, *num* should be *1*. For the second coo, *num* should be *2*
For the first call, *result* should be *1. Hello*. For the second call, *result* should be *1. Hello\n 2.How are you*

