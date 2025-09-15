# Challenge 2

Now we have the layout, we want to get some interaction.

Let's create the **Add** component.

For this we need to look into React Router.  This allows us to target components as though they are web pages.  Instead of a page being loaded the react router captures the URL click and instead turns it into a DOM render.

Once you've worked out how to do the react router, you can then create the form which is to add data.

To store the data we will need a state variable.  Since we are working with many records you will need your state variable to be an array of objects.  The state variable, will simply be an array, but each element will be an object.

In your footer you should change the number of visitors count to show the number of records in the database.

Everytime you add a new record to the state you should see the number of records in the database increase in the footer, and that value should be available from any page, since the footer is constant.  Your **button** to add needs to update the parents state, so you'll need to pass the button callback down to the child so that the child can update the parents data.

**NOTE**: it is important where you state is set.  In most cases state goes with the component, but our database state will need to be useable by other components.