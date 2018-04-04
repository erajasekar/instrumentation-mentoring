## Spring

+++

### What is dependecy Injection?

Instead of 

```java
public class A {
  private B b;

  public A() {
    this.b = new B(); // A *depends on* B
  }
  public void DoSomeStuff() {
    // Do something with B here
  }
}
public static void Main(string[] args) {
  A a = new A();
  a.DoSomeStuff();
}

```
+++

You write 

```java
public class A {
  private B b;

  public A(B b) { // A now takes its dependencies as arguments
    this.b = b; // 
  }
  public void DoSomeStuff() {
    // Do something with B here
  }
}
public static void Main(string[] args) {
  B b = new B(); // B is constructed here instead
  A a = new A(b);
  a.DoSomeStuff();
}

```
+++

### Why use dependency injection?

* Give you ton of advantages
* Ability to control functionality from a central place instead of spreading it throughout your program
* Ablity to easily test each class in isolation because you can pass along mocked objects
* But the drawback is you have to deal with complexity of wiring all your references in a central place.
* This is what the DI Framework like Spring helps.

+++
### How Spring annotation works?

+++

### Configuration

+++

### Caveats in storing state

---

## Concurrency Best practices

### Immutability

+++

### How Functional programming helps

---

## Functional programming

+++

### Why FP?

+++

### Imperative vs Declartive

+++

### Requires a paradigm shift

+++

### Example

---

## Important requirements for delivering any feature

+++

### Automated testing

* Have I written automated tests  to verify my feature?

* Learn to use Mocking libraries & Test frameworks

+++

### Logging

* Do I have enough logging to verify my feature works in production?

* Do I have enough information to trouble shoot when something on working?

* Make sure to properly handle and log exceptions.

+++

### Monitoring/Instrumentation

* Do I have easy way to check my feature is working well in production?

* Can I get automated notifications when something goes wrong?

---

## Day to Day productivity

* I use intellij and highly recommending it for editing

* I still use eclipse for debugging/hot deploy

* Always whitelist the projects in workspace-user.xml

* Try to use git for incremental checkin




