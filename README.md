backbone-todo-start
===================

The start of the backbone-todo project

##Objective

Build a functioning (albeit simple) MV* task list project using Backbonejs

##Steps
###1: Create a Todo model.
* Your model should have two attributes: 'title', and 'completed'
* Completed should default to `false`

###2: Create a Todo view (and associated template).
* The structure of your template should look something like this:
<pre><code>
    &lt;script type="text/template" id="todo-template">
      &lt;... template here ...>
    &lt;/script>
</pre></code>
* The template code markup itself should be pretty simple: 
  * An input of `type="checkbox"`
  * A `label` for the title
  * A `button` (with `class="destroy"`) for deletion

Once you've created the template, create the View itself.
* Don't forget to specify the template using underscore's template function
* Make sure to create a render function that places the `model.toJSON()` into the template
* Don't forget to make the use of `this.$el` when rendering

###3: Test your application
* When the user presses 'enter,' create a new Todo model, add it to a new Todo view, and append it to the `.todos-list` div
* Make sure the template renders correctly
* Try adding multiple todos to see what happens
