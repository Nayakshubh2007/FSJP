# Full Stack Java Programming Practical Questions

Solutions for all 16 questions from the supplied practical question sheet.

## Folder guide

| Question | Folder | Main file |
|---|---|---|
| Q1 Student details | `Q01_Student_Details` | `StudentDetails.java` |
| Q2 Constructor overloading | `Q02_Constructor_Overloading` | `ConstructorOverloading.java` |
| Q3 Method overloading | `Q03_Method_Overloading` | `MethodOverloading.java` |
| Q4 Single inheritance | `Q04_Single_Inheritance` | `SingleInheritance.java` |
| Q5 Multilevel inheritance | `Q05_Multilevel_Inheritance` | `MultilevelInheritance.java` |
| Q6 Hierarchical inheritance | `Q06_Hierarchical_Inheritance` | `HierarchicalInheritance.java` |
| Q7 Welcome Servlet | `Q07_Servlet_Welcome` | `WelcomeServlet.java` |
| Q8 Servlet form | `Q08_Servlet_Form` | `name-form.html`, `ShowNameServlet.java` |
| Q9 Welcome JSP | `Q09_JSP_Welcome` | `welcome.jsp` |
| Q10 Student info JSP | `Q10_JSP_Student_Info` | `student-info.jsp` |
| Q11 JDBC student CRUD | `Q11_JDBC_Student_CRUD` | `StudentCRUD.java`, `schema.sql` |
| Q12 Registration form and CSS | `Q12_Student_Registration_Form` | `registration.html`, `style.css` |
| Q13 Department webpage | `Q13_Department_Webpage` | `department.html`, `department.css` |
| Q14 Email validation | `Q14_Email_Validation` | `email-validation.html` |
| Q15 Registration validation | `Q15_Registration_Validation` | `registration-validation.html` |
| Q16 DOM background change | `Q16_DOM_Background_Color` | `background-color.html` |

## Running the Java programs (Q1 to Q6)

Install a JDK, open a terminal in the question folder, then run:

```bash
javac StudentDetails.java
java StudentDetails
```

Use the matching `.java` filename and public class name for each question.

## Running Servlets (Q7 and Q8)

These examples use `jakarta.servlet` annotations and are intended for a Jakarta EE compatible servlet container such as Tomcat 10 or later. Add the Servlet API dependency to the web application, deploy it to the server, and visit `/welcome` for Q7. For Q8, open `name-form.html` from the deployed web application and submit the form. If your college lab uses Tomcat 9 or older, replace `jakarta.servlet` imports with the corresponding `javax.servlet` imports.

## Running JSP (Q9 and Q10)

Place the `.jsp` file in a deployed web application on a JSP compatible servlet container, then open its URL in a browser. In Q10, replace `Your Name` and `YOUR_REGISTER_NUMBER` with your own details before the practical.

## Running JDBC (Q11)

1. Install MySQL and the MySQL Connector/J JDBC driver.
2. Run the SQL in `schema.sql`.
3. In `StudentCRUD.java`, set `USER` and `PASSWORD` to your local MySQL credentials.
4. Add the Connector/J JAR to the classpath and compile/run the program. Example on Windows:

```bat
javac -cp .;mysql-connector-j.jar StudentCRUD.java
java -cp .;mysql-connector-j.jar StudentCRUD
```

On macOS/Linux, use `:` instead of `;` between classpath entries. The example creates the table automatically and uses prepared statements for data changes.

## Running HTML, CSS and JavaScript (Q12 to Q16)

Open the `.html` file directly in a modern browser. Q12 uses a separate CSS file, so keep both files in the same folder. Q13 uses placeholder faculty and contact details for demonstrating the layout; use details provided by your college if required.

## Exam tip

Practise typing the class declaration, `main` method, constructor, `extends`, form submit handler, and JDBC `PreparedStatement` flow. For web server questions, remember the endpoint URL and the server setup required to run it.
