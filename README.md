# wiki-ing
## _wiki, because I'm No Genius_

.
# Short description
The web-application allows the sharing of knowledge inside a business through writing, reading and sharing of articles.

# Target
Companies that want to give structure and accessibility to their knowhow. The prototype of the application will be created for the Viennese catering business Gaumenfreundinnen.

# Frontend
User can login with username and password.
There are 2 types of users with different “permissions”:
- User+: can read,modify and create articles.
- User: can read articles. This is meant for occasional employees.

Users (user+ and user) can only access articles of their category. E.g. a user with category “kitchen” is not allowed to read (or create/modify) articles where the main category is “back-office”.
User can navigate through the categories or search for an article with the search function.
Once the article is shown, user can:
1. Save it into his “favourite” articles.
2. Save it in a readinglist. It is possible to create different readinglists and
name them. There is the possibility to share the reading list with other
users.
3. User+ can also modify the article.

User+ can write an article specifying:
1. title,
2. content,
3. main category. They can decide:
• to save the article directly into the main category.
• To set the article as “active” (every authorized user can read it) or “inactive” (only the Author (and Admin) will be able to see it and modify it). This is meant to help the writing process that can be interrupted and again continued as many times as user need.
4. There is also the possibility to add pictures
In the prototype application there are 4 main categories (kitchen, various, back- office and service).

# Backend
Admin can create and modify users.
If a user is no longer employee, admin can set his status to “non active” to make sure that former employees can't access the application. The articles created by former employees will still remain available.
Admin can create categories.

# Technical Environment
Script languages: PHP, HTML, CSS, Javascript
Libraries or Frameworks: Laravel 8 (php), JQuery (JavaScript), TinyMce (wysiwyg), Tailwind CSS (css).
Limits:
-no video hosting, just links to videoplayer.
Future implementations:
-subcategories: subcategories can be created by user+ (and Admin). Is intended to limit the nesting of categories to 2 (one main category and one subcategory)
-statistic: how many articles has that user read, how often was this article read/saved in favourites...
-possibility to save documents (pdf) into an article.
-history of an article: who is the author, when was created, when was it modified, why and by whom.
