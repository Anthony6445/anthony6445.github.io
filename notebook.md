# My Coding Notebook

At the top, begin a table of contents, Ex.:
## Table of Contents
- [Flutter Notes](#flutter-notes)
  - [What is Flutter?](#what-is-flutter)
  - [Key Terms and Definitions](#key-terms-and-definitions)
  - [Layout and Design Widgets](layout-and-design-widgets)
  - [Flutter Definitions with Structures ](#flutter-definitions-with-structures)
- [Code Definitions](#code-definitions)
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)




## Flutter Notes 

### What is Flutter?
- Definition: made by Google for building apps that work on web, Android,and iOS-with one codebase.
- Why is it useful?
Uses the Dort programming language.


---


### Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building block of a Flutter app. Everything is a widget.          |            Text, Image, Container, Colum               |
| MaterialApp      |  The root of the app. Sets up routes and themes.                                               | Found in main. dart                                           |
| Scaffold         |  Provides basic visual layout-like a header,body, floating button     |                         Each screen uses it                     |                                           |
| StatelessWidget  |  A widget that doesn't change                                               |  Most of the screen files                                         |
| StatefulWidget   |  A widget that can change over time                                               | Used in MyHomePage()                                          |
| Navigator        |  Manages screen transitions                                               |Navigator.pushNamed(context, '/page2');                                           |
| AppBar           |  Top navigation bar                                               | Title of each page appears here                                          |
| Column           |  vertical layout                                 |                                          |
| Row              | horizontal layout                                |                                           |
| Container        |  wraps content with padding, margin, or color    |                                           |
| Text             |  displays text                                   |                                           |
| Image.network    |  displays images from a URL                      |                                           |
|  Padding         |  adds space around a widget                      |                                           |
|  Center          |   centers its child                              |                                           |

---

### 🎨 Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?

## Flutter Definitions with Structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |

|------|----------------------------|----------------|-------------------|-------------|

| Main     | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |Opening an app on your phone.  |in main.dart, void main () => runapp(MyPortfolioApp());  |

| MaterialApp     | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |The table of contents located in a book since it sets up how you move through different sections.  |return MaterialApp(debugShowCheckedModeBanner: false, title: 'TSA Portfolio', theme: ThemeData(  |

| Scaffold     | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |The table you are putting your definitions in.  |return Scaffold( body: Column(mainAxisAlignment: MainAxisAlignment.start,children: [  |
     
 

| Columns     | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |Stacking things up.  |foregroundColor: Colors.white,backgroundColor:Colors.blue, //Button text color padding:const EdgeInsets.symmetric(horizontal:40,vertical: 15), // EdgeInsets.symmetric textStyle: const TextStyle( fontSize: 18, fontWeight: FontWeight.bold), // TextStyle  |

| Row     | A widget that shows things side-by-side. | `Row(...)` |Putting things side by side.  |color: Colors.white, fontSize: 28, fontWeight:FontWeight.bold,  |

|Container      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |A lunchbox holding foods inside and you can decorate it, or change the other things that makes the lunchbox look different on its own design.  |  Container(width:200,height:200,decoration:BoxDecoration(border:Border.all(color:Colors.blue,width:5),),//BoxDecoration child:Image.asset('assets/images/dove-couple.jpg',// <--MODIFIED TO LOCAL ASSET fit:BoxFit.cover, ),//Image.asset|

| Text     | A widget to display text on the screen. | `Text('Hello')` |Writing a message to your mom.  |"Text": "This is Luna, a cheerful retriever who loves playing fetch.",},  |

| Image Network     | A widget to show an image using a link from the internet. | `Image.network('https://...')` |Google images  |child:Image.asset('assets/imagesdove-couple.jpg',// <-- MODIFIED TO LOCAL ASSET fit: BoxFit.cover,),//Image.asset)  |

| Elevated Button     | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |Clicking on the keyboard while texting.  |child:const Text('Next'),  |

| onPressed     | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |Text is being written after tapping on your keyboard.  |onPressed: () => Navigator .pushNamed(context, '/background'),  |

| StatelessWidget     | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |Like a screen on your homepage.  |class HomeScreen extends StatelessWidget {  |

| Statefullwidget     | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |When you submit an assignment and you get a confirm page.  |class CounterScreen extends StatefulWidger {  |

| Navigator     | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |Going to your about page.  |Navigator .pushNamed(context, '/background'),  |

|Padding      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |Making more space for your living room.  |padding:const EdgeInsets.symmetric(  |

|Center      | Aligns content in the center of the screen or container. | `Center(child: ...)` |Title in the center of your app.  |body: Center(  |

|Wrap     | Automatically puts widgets onto a new line when there's no space. | When your're typing a text in a doc and it goes down by itself.  | `Wrap(children: [...])` |Wrap(alignment:WrapAlignment.center,children:puppyUrls.map((urL) => puppyImage(urL)).toList()), |

|Override      | This marks a method as one that’s replacing a method in a parent class. | `@override` |Making our own build method.  |@override Widget build(BuildContext context) {  |

|Build      | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |Reading the signs on how to park your car on the parking lots behind the park.  |line 8 Widget build(BuildContext context) { -----down ----- line 81 ); // Scaffold  |

| Build     | Required in every widget class to describe what to show. | `build` |Drawing a house to build in real life.  |line 15 Widget build(BuildContext context) { ---down----line 59 ); // Scaffold  |

| BuildContext     | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |When the blinking cursor occurs in a text document to show you the exact spot where the next thing you type will appear.  |ElevatedButton (onPressed:()=> Navigator. pushNamed(context, '/showcase'),child: const Text ('Next'),  |

| Super.key     | A keyword used to pass a value to the parent widget. | `super.key` |Emailing your teacher.  |const BackgroundScreen ({super.key});  |

|Const      | A keyword that means the value won't change and is set once. | `const` |Title  | padding: const EdgeInsets.all(12), |















# Code Definitions

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|------------|
| variable     | A named container used to store a value that may change. | `var x = 5;` |Weight is 125  |title: 'TSA Portfolio'  |
| constant     | A fixed value that cannot change once set. | `const PI = 3.14;` |The 7 days in a week never changes.  |main.dart, const MyPortfolioApp ({super.key)  |
| Data Type     | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` | Age vs Words in a sentence. |main.dart,bool,debugShowCheckedModeBanner:false  |
| String     | A sequence of characters used to represent words or text. | `"Hello World"` |A title  |  |
| Integer    | Whole number values. | `int age = 16;` |Seeing your health score number from 100 - 0  |  |
| Double     | Number values with decimals. | `double age = 16.2;` |Calculations  |  |
|Boolean      | A value that can be true or false. | `bool isLoggedIn = false;` |If I practice that day, will my streak go up?  |  |
|List      | A collection of values in a specific order. | `List<String> names = [];` |Newest to oldest release  |  |
|Null     | A special value that means “nothing.” | `String? name = null;` |Unloaded level  |  |
|Function      | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |Repeating the level again on a game.  |  |
| Parameter     | The information passed into a function to change how it works. | `greet(String name)` |Choosing your video game character color or style.   |  |
| Return     | The result a function gives back. | `return total;` |Are you part of the militray? If yes, the result will be entering in the militray. If no, the result will be leaving the area.  |  |
| Scope     | Where a variable or function can be used. | (No set syntax — concept-based) |Gift cards for specific places.  |  |
| Class     | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |Creating a waterbottle with a defined structure.  |  |
| Object     | A specific version of a class. | `Dog myDog = Dog();` |The tablet is the main object used for relaxation like watching videos.  |  |
| Property     | A variable that belongs to a class/object. | `String name;` |My brother weights 135 pounds.  |  |
| Method     | A function that belongs to a class. | `void bark() {}` |Turning your car on.  |  |
| Constructor     | A special function used to set up a class when it’s created. | `Dog(this.name);` |Knowing how to play Minecraft before you play the game.  |  |
| Abstraction     | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |We hit A and the cumputer shows it as 32.  |  |
| Override     | Changing how a built-in or inherited function behaves. | `@override` |You have characters and they all run the same and you override so you can see what happens between them.  |  |
| Void     | A function that does not return a value. | `void printMessage() {}` |You turn the lights on but you don't get anything back.  |  |
| Scanner | Creates a scanner object to take input from user | Scanner in = new Scanner(System.in);  |||
|import Scanner | Gives access to Scanner class, required at top | import java.util.Scanner;  |||
|print line statement | prints what's in the parenthesis, adds line after |  |||
|print statement  | prints the content in the parenthesis  |  |||
|input nextLine  |  |  |||
|input nextInt  |  |  |||
|input nextDouble|||||
|input nextBoolean|||||
|Arithmetic operators|||||
|Compound operators (applies the result to the variable)|||||


























## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
