Download Link: https://assignmentchef.com/product/solved-32998-net-applications-development-assignment-2
<br>
<strong>Summary </strong>

This assessment requires you to develop a simple text editor with a basic offline user login. It is a windows application that will allow new users to be added, existing users to login, and to create/save/edit text documents. The text documents can be either viewed or modified/created based on the user type. This will be a prototype of a text editor which will provide an overview of the basic underlying programming techniques required to create windows applications and text manipulation.

<strong> </strong>

<strong>Assignment Objectives </strong>

The purpose of this assignment is to demonstrate competence in the following skills.




<ul>

 <li>Windows form and controls</li>

 <li>Communication between multiple windows forms</li>

 <li>Using collections/generics</li>

 <li>Enumerators and properties. q Text file reading and writing</li>

</ul>

<strong><u>Windows/Screens:</u></strong>

Each box is a separate screen which shows the visual elements that should be present. The direction of arrows specify the direction of flow between screens. The text in each box describes some of the components that should be in the screen, though you are free to add more if you feel they are needed / appropriate.

<strong><u>Requirements:</u></strong>

In order to test core C# principles and windows programming skills, the following are required. Any additional functionality should be designed and added as needed. <strong> </strong>

<ol>

 <li>Create appropriate class and methods for handling user login information.

  <ol>

   <li>User information/details are stored in a text file named <strong>“login.txt”</strong> in the following format (each value is separated by a comma):</li>

  </ol></li>

</ol>

<strong>Username, Password</strong><strong>, User_Type</strong><strong>, First_Name</strong><strong>, Last_Name</strong><strong>, dd-mm-yyyy(Date-of-birth) </strong>

<strong> </strong>

<ol>

 <li>Use of appropriate collection/data structure is required for storing the user information from the <strong>“login.txt”</strong></li>

</ol>




<ol>

 <li>The class should have appropriate variables to:

  <ol>

   <li>Track the currently logged user and their user type ii. Accessors for each of the variables.</li>

  </ol></li>

</ol>




<ol>

 <li>The class should have methods to:

  <ol>

   <li>Load all users from the <strong>“login.txt” </strong>file into an appropriate data structure. Save all users back to <strong>“login.txt”</strong>, when a user logs out of the text editor.</li>

  </ol></li>

</ol>

<ul>

 <li>Checking if a user name and password provided by the user is valid.</li>

</ul>

<ol>

 <li>The type of user describes whether a user is allowed to edit any file. There are two type of users:

  <ul>

   <li>“View”: The user can only view any text file. Text editing is disabled in the text editor window.</li>

   <li>“Edit”: The user can create/edit any text file.</li>

  </ul></li>

 <li><strong>Login Form: </strong>

  <ol>

   <li>This is first screen displayed when the program is launched</li>

   <li>All the user information from <strong>“login.txt” </strong>should be loaded into appropriate data structure/collection.</li>

   <li>When <strong>login button</strong> is pressed, the username and password in the textbox are checked with all the available user information. If the login is successful, the text editor form/window is displayed. In case of unsuccessful login, appropriate message is shown using MessageBox() and the login windows remains open.</li>

   <li>When <strong>Exit button</strong> is pressed, the application is closed.</li>

   <li>When <strong>New User button</strong> is pressed, the New user window/form is displayed and hides the login form.</li>

  </ol></li>

</ol>




<ol start="3">

 <li><strong>New User Form: </strong>

  <ol>

   <li>A user is allowed to enter the required information.</li>

   <li>When <strong>submit button</strong> is pressed, the information is added to the data structure/collection, and all information is saved back into the <strong>“login.txt” </strong></li>

   <li>When <strong>cancel button</strong> is pressed, the Login form is display and hides the New user form.</li>

  </ol></li>

</ol>




<ol start="4">

 <li><strong>Text Editor Window: </strong>

  <ol>

   <li>Appropriate common dialog boxes should be used to implement the <strong>open, save and save as</strong> functionality available in the menu strip under <strong>File</strong> menu and also the respective tool strip buttons.</li>

   <li><strong>Open</strong> menu will allow to select a text file and load all the text from the file into the RichTextBox.</li>

   <li>Save and Save as, will save all the text line in the RichTextBox into an <strong>.rtf</strong></li>

   <li>The <strong>Bold, Italic and UnderLine</strong> buttons on the top ToolStrip are used change the selected text style to bold, Italic or UnderLine.</li>

   <li>The ComboBox on the top ToolStrip shows the <strong>font size</strong> from 8 to 20, and is used to change the size of the selected text in the RichTextBox.</li>

   <li>The <strong>Cut, Copy and Paste</strong> buttons on the left ToolStrip and <strong>Edit</strong> Menu are used to cut/copy/paste selected text in the RichTextBox.</li>

   <li>The About form should be used to implement the <strong>About</strong> menu item under <strong>Help</strong>.</li>

   <li>On clicking <strong>Logout</strong> option from the <strong>File</strong> Menu, the text editor window should close and the Login window should be displayed.</li>

   <li>The RichTectBox should be disabled or enabled for editing based on the user type.</li>

  </ol></li>

</ol>




<ol start="5">

 <li><strong>About Window: </strong>

  <ol>

   <li>Should display appropriate information about your text editor, such as name, version number, etc.</li>

   <li>On clicking OK button, the <strong>About</strong> form should close.</li>

  </ol></li>

</ol>

<strong> </strong>

<strong><u>Marking Guide:</u></strong>




Below is the marking guide for this assessment. It is designed to allow you to get a Pass grade with minimal effort while still demonstrating that you understand the core principles of .NET development, to get a Distinction with reasonable effort, and to get a High Distinction with solid effort, and 100% with considerable effort. It is recommended that you pay attention to the grade distribution and work towards your own skill level.




In the demos in the lab, your code needs to be compiled in <strong>Visual Studio</strong> and then the tutor will test for normal functionality as described in the descriptions above. If your code does not compile you will receive zero marks. You need to demonstrate that you understand the functionality of various components in a Windows form and your forms should be easily readable and usable by your tutor.

<strong> </strong>

<table width="593">

 <tbody>

  <tr>

   <td width="98"><strong>Task </strong></td>

   <td width="306"><strong>Items </strong></td>

   <td width="53"><strong>Max </strong><strong>Points </strong></td>

   <td width="135"><strong>Grade </strong>(Assuming full points above this item)</td>

  </tr>

  <tr>

   <td width="98"><strong>Code Design </strong><strong>(Programming </strong><strong>style) </strong></td>

   <td width="306">Includes high cohesion and low coupling for classes and methods, using properties, using enumerations, collections where appropriate, etc.</td>

   <td width="53"><strong>3 </strong></td>

   <td width="135"><strong>9% </strong></td>

  </tr>

  <tr>

   <td width="98"><strong>Code Quality </strong><strong>(Programming </strong><strong>style) </strong></td>

   <td width="306">Includes proper indenting and white spacing, helpfulcomments and meaningful class/method/property/field names.</td>

   <td width="53"><strong>3 </strong></td>

   <td width="135"><strong>18% </strong></td>

  </tr>

  <tr>

   <td width="98"><strong> </strong><strong> </strong><strong>Design </strong></td>

   <td width="306">Includes form/window designs, with basic transition between forms/windows on button clicks or as appropriate:–                Login: 2 marks–                New User: 3 marks–                Text Editor: 6 marks –       About: 1 mark</td>

   <td width="53"><strong>12 </strong></td>

   <td width="135"><strong>52% </strong></td>

  </tr>

  <tr>

   <td rowspan="4" width="98"><strong>Functionality </strong>(in order ofrecommendedimplementation,e.g. start with items higher on the list)</td>

   <td width="306"><em>Text Editor Window</em> – Required Classes, Methods, and Member Variables are correctly implemented, in order to achieve the overall functionality of a simple text editor and code compiles without error.–   All File menu options implemented: 4 marks–   All Edit menu options and buttons: 2 marks–   All text editing buttons (bold, italics, etc): 4 marks</td>

   <td width="53"><strong>10 </strong></td>

   <td width="135"><strong>80% </strong></td>

  </tr>

  <tr>

   <td width="306"><em>Login screen</em> working correctly by reading from and   writing to <em>login.txt</em> file instead of a hardcoded User list</td>

   <td width="53"><strong>3 </strong></td>

   <td width="135"><strong>89% </strong></td>

  </tr>

  <tr>

   <td width="306"><em>Login Screen</em> – successful login and failed login with sample User details are hard coded and appropriate data structure used.</td>

   <td width="53"><strong>2 </strong></td>

   <td width="135"><strong>94% </strong></td>

  </tr>

  <tr>

   <td width="306"><em>New User Screen</em> – successfully add new user and allow that user to then login</td>

   <td width="53"><strong>2 </strong></td>

   <td width="135"><strong>100% </strong></td>

  </tr>

  <tr>

   <td width="98"><strong> </strong></td>

   <td width="306"><strong>                                                                   Total   </strong></td>

   <td width="53"><strong>35 </strong></td>

   <td width="135"><strong> </strong></td>

  </tr>

 </tbody>

</table>







<u>Additional Information:</u>

<strong>Assignment Submission:</strong>

Submission of your assignment is in two parts. You must upload a zip file of the C# solution to Canvas. This must be done by the Due Date. You may submit as many times as you like until the due date. The final submission you make is the one that will be marked. If you have not uploaded your zip file within 7 days of the Due Date, or it cannot be compiled and run in the lab, then your assignment will receive a zero mark




<em>NOTE 1: </em>It is your responsibility to make sure you have thoroughly tested your program to make sure it is working correctly.




<em>NOTE 2: </em>Your final submission to Canvas is the one that is marked. It does not matter if earlier submissions were working; they will be ignored. Download your submission from Canvas and test it thoroughly in your assigned laboratory.




<h2>Queries</h2>

If you have a problem such as illness which will affect your assignment submission contact the subject coordinator as soon as possible.




<strong>Dr. Nabin Sharma  </strong>

<strong>Room: CB11.07.124  </strong>

<strong>Phone: 9514 1835 </strong>

<strong>Email: </strong><strong><u><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="6826090a0106463b00091a0509281d1c1b460d0c1d46091d">[email protected]</a></u></strong>




If you have a question about the assignment, please post it to the Canvas discussion board for this subject so that everyone can see the response.




If serious problems are discovered in assignment specification the class will be informed via an announcement on Canvas. It is your responsibility to make sure you frequently check Canvas.




<strong><em>PLEASE NOTE :</em></strong> If the answer to your questions can be found directly in any of the following

<ul>

 <li>Subject outline</li>

 <li>Assignment specification</li>

 <li>Canvas FAQ</li>

 <li>Canvas discussion board</li>

</ul>




You will be directed to these locations rather than given a direct answer.










<h2>Extensions and Special Consideration</h2>

Please refer to subject outline.

<strong> </strong>

<strong>Academic Standards and Late Penalties </strong>Please refer to subject outline.