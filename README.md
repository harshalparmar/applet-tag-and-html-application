# applet-tag-and-html-application
Today, we will be discussing the Applet Tag and how to add an Applet to an HTML file in Java programming.

First, let us define what an Applet is. An Applet is a Java program that can be embedded in a web page and run in a browser. It is a client-side technology that runs on the client's machine, not on the server.

Now, let's move on to the Applet Tag. The Applet Tag is used to specify an applet in an HTML document. It has the following syntax:
```
<applet code="AppletClassName.class" width="width" height="height">
```

`code` specifies the name of the class file that contains the applet's code.<br/>
`width` and `height` specify the size of the applet's display area in pixels.


You can also include other attributes such as name, archive, and codebase in the Applet Tag to provide more information about the applet.<br/>
To add an Applet to an HTML file, you need to follow these steps:
1. Create a Java Applet program
```
import java.applet.Applet;
import java.awt.Graphics;

public class MyApplet extends Applet {
	public void paint(Graphics g) {
		g.drawString("Hello, World!", 20, 20);
	}
}
```
2. Compile the program using a Java compiler to generate a `.class` file.
3. Place the `.class` file in the same directory as the HTML file or in a directory specified in the `codebase` attribute of the Applet Tag.
4. Insert the Applet Tag in the HTML file, with the code attribute pointing to the `.class` file.

# HTML
Here's an example of an HTML file that contains an Applet:

```
<!DOCTYPE html>
<html>
   <head>
    <title>My Applet Example</title>
  </head>
  <body>
    <applet code="MyApplet.class" width="400" height="300">
    Your browser does not support Java applets.
    </applet>
  </body>
</html>
```

In this example, we assume that `MyApplet.class` is located in the same directory as the HTML file.

In summary, the Applet Tag is used to specify an applet in an HTML document, and it requires the `code` attribute to point to the `.class` file that contains the applet's code. To add an Applet to an HTML file, you need to create a Java Applet program, compile it, and then insert the Applet Tag in the HTML file with the appropriate `code`, `width`, and `height` attributes.


Java applets are no longer widely used in modern web development. They have been largely replaced by other technologies such as HTML5, CSS, and JavaScript. In addition, modern web browsers are increasingly dropping support for Java applets due to security concerns.<br/>

As of Java SE 9, the Java plugin used to run applets in web browsers has been deprecated and will be removed in a future release of the Java Development Kit (JDK). This means that running Java applets in web browsers will become more difficult as time goes on.<br/>

However, Java applets can still be run using standalone Java applications or applet viewers, such as the Applet Viewer tool that comes with the JDK. Additionally, some legacy applications may still rely on Java applets.<br/>

Overall, Java applets are no longer a popular or recommended technology for web development.<br/>

# Error enconterd while compiling code in vscode using JDK 17
![alt text](https://raw.githubusercontent.com/harshalparmar/applet-tag-and-html-application/main/vscode-error.png)

# Problems enconterd while compiling code in vscode using JDK 17
![alt text](https://raw.githubusercontent.com/harshalparmar/applet-tag-and-html-application/main/vscode-problem.png)
