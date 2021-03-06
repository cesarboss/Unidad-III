= The Depot Online Store
 
This application implements an online store, with a catalog, cart, and orders.
 
It is divided into two main sections:
 
* The buyer's side of the application manages the catalog, cart, 
  and checkout. It is implementation spans in four models and associated
  controllers and views: Cart, LineItem, Order, and Product.  Additionally,
  there is a StoreController for the store front itself, and a
  SessionsController to manage sessions.
 
* Only administrators can access stuff in the seller's side
  (product maintenance and order fulfillment).  This is implemented by the
  SessionsController, is enforced by the ApplicationController#authorize
  method, and assisted by the Users and Carts resources.
 
This code was produced as an example for the book {Agile Web Development with
Rails}[http://www.pragprog.com/titles/rails4/agile-web-development-with-rails-4th-edition]. It should not be 
run as a real online store.
 
=== Authors
 
 * Sam Ruby, IBM
 * Dave Thomas, The Pragmatic Programmers, LLC
 * David Heinemeier Hansson, 37signals
 
=== Warranty
 
This code is provided for educational purposes only, and comes with 
absolutely no warranty. It should not be used in live applications.
 
== Copyright
 
This code is Copyright (c) 2013 The Pragmatic Programmers, LLC.
 
It is released under the same license as Ruby.