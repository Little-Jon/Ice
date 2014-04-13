Ice
===

Ice is a GUI automation library written in Java and C#. The end goal is to be able to automate nearly any application. Currently, three key frameworks are used. The first is the Windows UI Automation framework, which was released as part of the .NET 3.0 framework. This framework allows automation of all Windows applications that implement UI Automation, which includes Win32, Windows Form, Java SWT (in some cases), and WPF applications. The second framework used is mshtml (mshtml.dll is part of the CLR on Windows). Mshtml is used to automate Internet Explorer applications on Windows. The last framework - the implementation of which is still in progress - is Oracle Sun's JemmyFX framework. JemmyFX allows automation of Java AWT and SWT applications.

Ultimately, I hope to have this project written in Java and C#. Because I started writing the project in C#, that's the aspect which is the most complete. As it stands, the UI Automation and mshtml frameworks are controlled by the C# version, and the Jemmy framework by Java; I expect to implement interopability between the two such that both aspects can take advantage of the frameworks which the other controls, while not requiring such interoperation. This will theoretically allow a user to automate using UI Automation, mshtml, and Jemmy frameworks in either Java or C#. Additionally, I hope to structure things such that Linux users will have no issue using Ice to automate Java AWT/SWT applications.
