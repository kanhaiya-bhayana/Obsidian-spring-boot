

### AOP Aspect Oriented Programming

- Programming technique based on concept of an Aspect
- Aspect encapsulates cross-cutting logic


###### Cross-Cutting Concerns 
	Concerns means logic/functinality

###### Aspects
- Aspect can be reused at multiple locations
- 
- Same aspect/class ... applied based on configuration

###### AOP Solution
- Apply the Proxy design pattern
	- Proxy is **a structural design pattern that provides an object that acts as a substitute for a real service object used by a client**. 
	- A proxy receives client requests, does some work (access control, caching, etc.) and then passes the request to a service object.

###### Benefits of AOP 
- Code for Aspect is defined in a single class
	- Much better than being scattered everywhere
	- Promotes code reuse and easier to change
- Business code in your application is cleaner
	- Only applies to business functionality: add account
	- Reduces code complexity
- Configurable
	- Based on configuration, apply Aspects selectively to different parts of app
	- No need to make changes to main application code ... very important!

##### Additional AOP Use Cases
- Most common
	- logging, security, transactions
- Audit logging
	- who, what, when, where
- Exception handling
	- log exception and notify DevOps team via SMS/email
- API Management
	- how many times has a method been called user
	- analytics: what are peak times? what is average load? who is top user?

###### AOP: Advantages and Disadvantages
	Advantages
		Reusable modules
		Resolve code tangling
		Resolve code scatter
		Applied selectively based on configuration
		   
	Disadvantages
		Too many aspects and app flow is hard to follow
		Minor performance cost for aspect execution (run-time weaving)


##### Weaving
- Connecting aspects to target objects to create an advised object
- Different types of weaving
	- Compile-time, load-time or run time
- Regarding performance: run-time weaving is the slowest
##### AOP Frameworks
- Tow leading AOP Frameworks for JAVA
	- Spring AOP
	- AspectJ

##### Spring AOP Support
- Spring provides AOP support
- Key component of Spring
	- Security, transactions, caching etc
- Uses run-time weaving of aspects

##### AspectJ
- Original AOP framework, release in 2001 - www.eclipse.org/aspectj
- Provides complete support for AOP
- Rich support for
	- Join points: method-level, constructor, field
	- Code weaving: compile-time, post compile-time and load-time

###### Advised Types
- **Before advice:** run before the method | Use Cases - Most common: logging, security, transactions
- **After returning advice:** run after the method (success execution)
- **After throwing advice:** run after method (if exception thrown)
- **After finally advice:** run after the method (finally)
- **Around advice:** run before and after method


> Spring @Transactional - uses AOP behind the scenes

##### Before Advice - Use cases
- Most common
	- logging, security, transactions
- Audit logging
	- who, what, when, where
- API management
	- how many times has a method been called user
	- analytics: what are peak times? what is average load? who is top user?


> @Before("execution(* add*(com.octocat.aopdemo.Account, ..))") // here '..' means match any no. of arguments

![[Pasted image 20240216225329.png]]



##### Pointcut Declarations
![[Pasted image 20240216230418.png]]

![[Pasted image 20240216230443.png]]
![[Pasted image 20240216235046.png]]![[Pasted image 20240216235123.png]]