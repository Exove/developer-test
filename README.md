# Developer test

**Please read the instructions carefully before starting the test.**

Return the test to jobs@exove.fi

This test has three sections, each having three or four questions. Your task is to choose one question per section. 

**Remember to choose the questions based on the position you are applying for.** It will also affect your overall grading. For example: answering front-end only questions when applying to a back-end position isn't ideal.

You need to answer at least one question per section in order to pass the test. If you end up answering more than one question in a section, we will use the highest grade of these questions to grade the section.

Please note that the use of **AI tools** is not strictly forbidden, as long as they can help with mock data generation or unit testing, for example; but remember that the purpose of the test is to assess your skills in order to make sure you will be able to live up to the expectations in your future work assignments. Your submission will be checked against an AI detector, as specified below.

**Practicalities**

Do the back-end tasks with Javascript or PHP, Drupal tasks in PHP and front-end tasks with HTML, CSS and Javascript. You can use Typescript if you prefer it. Make sure that your implementations can be tested easily.

Do the test yourself, don’t ask for help from outsiders. If you have questions about the test, you might want to check our [FAQ](FAQ.md) first; if you cannot find the answer there, you can contact Exove at coding-test-help@exove.com. We’ll be responding to your questions during office hours (Mon-Fri) between 9-17.

Add a README file to your test that lists the questions you answered and also little background on why and how did you came up with the implementation. You can also add screenshots of your implementation if applicable.

Before returning the tasks, please run your files thru the [QuillBot AI detector](https://quillbot.com/ai-content-detector) and make sure the score is below 50%: we will make the same check and reject any submissions that exceed the threshold.

After you have finished, create a public Github repository, push your work and send us the link to it.

## Section 1
### 1A. Write a sorting algorithm

Write a sorting algorithm that sorts strings based on the ASCII code of the third letter first, then second letter and then the first letter.

Here’s a list of words you can test with:
- BOAT
- Locomotive
- Poet
- Accelerate
- GOLF
- ACCIDENTAL
- Submarine

### 1B. Create a loading animation using css
- Add options to choose between size (large, small)
- Add options to choose between 2 colors
- Add options to modify speed (fast, slow)

### 1C. Create a slider in react
- Have its value stored in state
- Have it fire an event with the value
- Have it fire the event only when the user has stopped moving it

### 1D. Create a module in Drupal

Create a module for Drupal that shows the contents of an RSS feed. The module must create a configuration value for the URL of the RSS feed. The module must create a route (/link-list) and show the link and the title of the RSS feed in the route.

You don't have to style the page.

## Section 2

### 2A. Create a comic book reader/image browser or a carousel

Create a comic book reader/image browser or a carousel with React. Use images from this document or your own. Continued in question 3B. Using TypeScript is recommended.

### 2B. Create an SQL query

You have an SQL database with two tables, people and phones.

```
mysql> select * from people;
+----+------------+-------------+
| id | first_name | last_name   |
+----+------------+-------------+
|  1 | John       | Smith       |
|  2 | Mary       | Jones       |
|  3 | Gerhard    | Feuerhaufen |
|  4 | Rami       | Pitkäniemi  |
|  5 | Anna       | Kråkström   |
+----+------------+-------------+

mysql> select * from phones;
+----+---------+------------------+
| id | user_id | number           |
+----+---------+------------------+
|  1 |       2 | +1 213 621 0002  |
|  2 |       2 | +1 800 444 4444  |
|  3 |       1 | +1 604 444 4444  |
|  4 |       1 | +44 20 8759 9036 |
|  5 |       4 | +358 50 333 3333 |
|  6 |       5 | +46 771 793 336  |
+----+---------+------------------+
```
Create a single SQL query that will produce the following:
```
+---------------------+----------------------------------+
| name                | numbers                          |
+---------------------+----------------------------------+
| Gerhard Feuerhaufen | N/A                              |
| Mary Jones          | +1 213 621 0002,+1 800 444 4444  |
| Anna Kråkström      | +46 771 793 336                  |
| Rami Pitkäniemi     | +358 50 333 3333                 |
| John Smith          | +1 604 444 4444,+44 20 8759 9036 |
+---------------------+----------------------------------+
```

### 2C. Search for errors in the HTML

Search for at least 10 accessibility, validity and style errors in [this HTML](material/code.html) and fix them to the HTML. Return the whole fixed HTML.

## Section 3

### 3A. Get data and save it locally

Write code that gets data from a product API ([URL](material/products.json)) and saves it into an SQL database locally. For extra points note the following:
- Figure a way to save the hierarchical data (see product variations and categories for example)
- Figure a way to handle schemaless data (variations)
- Take into account that the database schema should support translations although the API doesn’t, use ISO 639-1 as language keys
- Add support for extra currencies
- How to update the product data from the API without re-saving everything but only parts that have changed
- Also note that not every object have IDs

### 3B. Continued from 2A, do two of the following:
- Separate elements into components
- Browse multiple comics/images from the top level
- If you chose to use Typescript, correctly type the code
- Use state to toggle dark mode


### 3C. Write a non-directional graph program

Write a program that counts the number of nodes in a non-directional graph and finds out whether there is a cycle in the graph

Examples of non-directional graphs:

Fig 1. A graph with a cycle

![A non-directional graph with a cycle](/material/non-directional-graph-cycle.png)

Fig 2. A graph without a cycle

![A non-directional graph without a cycle](/material/non-directional-graph.png)

### 3D. Write HTML and CSS for a provided layout 

Write the HTML and CSS for the simplified layout underneath. Also note that there might be more than three items present.

Make sure that one row has three columns if the window size exceeds 960 pixels and two if less. The extra item should drop to the next row.

![A mockup of a news site with columns of text](/material/news-site.png)
