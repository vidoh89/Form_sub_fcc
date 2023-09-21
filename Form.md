HTML CSS Form 
``The rem unit stands for root em, and is relative to the font size of the html element.``

``As label elements are inline by default, they are all displayed side by side on the same line, making their text hard to read. To make them appear on separate lines, add display: block to the label element, and add a margin of 0.5rem 0, to separate them from each other.``

``Following accessibility best practices, link the input elements and the label elements together using the for attribute.``

``
The first input element with a type of submit 
is automatically set to submit its nearest parent form element.
``
``minlength attribute ,prevents inputs of less than X characters from being submitted.
Example
  <label for="new-password">Create a New Password: <input id="new-password" type="password"  minlength=8 required /></label>
``
``pattern attribute(regular expression)requites password to match certain crieteria to be valid.
<label for="new-password">Create a New Password: <input id="new-password" type="password" pattern=[a-z0-5]{8,} required /></label>

``
``Radio button value
Allowing only one radio button to be selected at any given time
form does not know the radio inputs are related.

To relate the radio inputs, give them the same name attribute

``
``
Follow accessibility best practices by linking the 
input elements and the label elements by giving them 
a id attribute that matches the label's for attribute.
``
``file input type allows users to upload files such as profile pictures
  Example

  <fieldset>
      <label>Upload a profile picture:<input type="file"/></label>
      </fieldset>
``
``Using min and max attributes to validate age
 <fieldset>
        <label>Upload a profile picture: <input type="file" /></label>
        <label>Input your age(years):<input type="number" min="13" max="120"/></label>
      </fieldset>
``
``Adding a dropdown menu with the select element which is the 
container for a group of option elements..
options elements act as a label for each dropdown option.
Both elements require closing tags
--Submitting the form with an option selected would not send a useful value to the server. As such, each option needs to be given a value attribute. Without which, the text content of the option will be submitted to the server.
--------------------------
Example:placed inside forms fieldset element.
<label>How did you hear about us?
        <select>
          <option value="">(select one)</option>
            <option value="1">freeCodeCamp News</option>
            <option value="2">freeCodeCamp YouTube Channel</option>
            <option value="3">freeCodeCamp Forum</option>
            <option value="4">Other</option>
        </select>
        </label>

``
``adding a textarea
The textarea element acts like an input element of type text, but comes with the added benefit of being able to receive multi-line text, and an initial number of text rows and columns.
The textarea appears too small. To give it an initial size, 
you can add the rows and cols attributes.
``

example:
  <label for="bio">Provide a bio:
          <textarea id="bio" rows="3" cols="30"></textarea>
        </label>
 --
 ``adding a name attribute to the elements
 With form submissions, it is useful, and good practice, to provide each submittable element with a name attribute. This attribute is used to identify the element in the form submission.``
 ----------------
 ``CSS``
 Center the form element, by giving it a margin of 0 auto. 
 Then, fix its size to a maximum width of 500px, 
 and a minimum width of 300px. In between that range, 
 allow it to have a width of 60vw.
 ``
 Example:
 form{
  margin:0 auto;
  max-width:500px;
  min-width:300px;
  width:60vw;
}
---
``last-of-type CSS pseudo class selector
  You can select the last element of a specific type
``
Example:
element:last-of-type{}
---
``width:unset; removes preset width  settings;``
``vertical-align:adjust the vertical alignment of an element``

``styling a submit button with a attribute selector``
``style an input element with the attribute of password``
Example:
input[name="password"]
----
The above selects input elements with a 
name attribute value of password.
``centering the submit button``
example:
margin:0 auto;
```
