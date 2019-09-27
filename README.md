# blogstrapi
Personal blog using a Dynamic CMS for development with a Static HTML for deployment.

---
### Project Structure
     blogstrapi/                 <-- Root of your project
       |- package.json           <-- Node.js project entries
       |- _harp.json             <-- Global variables goes here
       |- _data.json             <-- Page variables goes here
       |- _layout.ejs            <-- Global layout for every page
       |- index.ejs              <-- Home page of your blog, Harp will produce an index.html
       +- css/                   <-- Holds any CSS or SCSS theme files
          |- bootstrap.min.css   <-- At a minimum, the bootstrap CSS file
          |- mytheme.css         <-- Our custom CSS theme goes here
       +- js/                    <-- Holds any JS files
          |- bootstrap.min.js    <-- At a minimum, the bootstrap JS file
       +- layout/                <-- Holds any Page layouts, prefixed with "_"
          |- _header.ejs         <-- Header layout, i.e. called by partial() function
          |- _footer.ejs         <-- Footer layout, i.e. called by partial() function

---
### Example Usage
In the following example, the default application will be created in the folder "myproject/".

     harp init myproject --boilerplate dennislwm/blogstrapi

