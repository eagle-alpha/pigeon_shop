## Pigeon Beta Storefront

For this techincal test we want you to build a simple basket in this storefront boilerplate code.

The app was built using Ruby 3.0.1 and Rails 7.0.4

The code was generated using the following commands. __You do not need to run these commands this is just for reference__

```rails new pigeon_shop --css tailwind --database=postgresql```

```rails g scaffold Product name:string code:string price:float```

```rails g scaffold Basket total:float discount:float to_pay:float```


You can run the server using the ```bin/dev``` to make use of tailwindcss rebuilding in rails 7.

If you have any issues setting up the app we used this post as a reference, you can re-create the setup yourself: https://www.simplethread.com/how-to-create-a-new-rails-7-app-with-tailwind/

The app is using tailwindcss, if you're not familiar with it you can find the docs here [Tailwindcss Docs](https://tailwindcss.com/docs/installation)

It's not a requirement to use Tailwindcss, if you're more comfortable writing plain CSS please feel free to do so.

The root URL is set to the product#index page where you can add products and you'll see an empty space on the right hand side of the page for the basket.

_There are no restrictions on how you complete these tasks, you can remove the current migrations and create your own if you have a different idea of how to structure the objects._

#### Task 1:

We want the ability to add products to a basket. Can you create the migrations to allow for this functionality.

#### Task 2:

Create an "Add To Basket" button in the "_product.html.erb" template.

When a user clicks this button it should generate a new Basket object and associate the product with the basket. If a basket already exists add the product to the basket.

#### Task 3:

Render the products in the basket on the right hand side of the products index page, the total of the basket should update as products are added to it.

#### Task 4:

Add a test to the repo, you can choose the type of test and the testing framework you want to use.


#### New Feature:

_This is not part of the tech test we will talk briefly about this feature request during the interview, we want to see your thought process if you were asked to develop this feature_

The marketing department wants to add a deal to give users 10% off if they spend more than 100 euro. Build functionality to apply a discount if the total in the basket is greater than 100 euros.