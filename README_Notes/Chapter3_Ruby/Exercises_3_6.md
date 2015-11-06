# Ruby on Rails Tutorial 

## Notes for DRY coding

### Exercise 3.6 Notes

```
$ git checkout static-pages
$ git checkout -b static-pages-exercises
<solve first exercise 3.1>
$ git commit -am "Eliminate repetition"
<solve second exercise 3.2> 
$ git add -A
git commit -m "Add a contact page" second exercise 3.2"
git push -u origin static-pages-exercises
git checkout master
```

#### Exercise 3.6.1

> You may have noticed some repetition in the Static Pages controller test 
(Listing 3.22). In particular, the base title, “Ruby on Rails Tutorial 
Sample App”, is the same for every title test. Using the special function setup, 
which is automatically run before every test, verify that the tests in 
Listing 3.38 are still green. (Listing 3.38 uses an instance variable, 
seen briefly in Section 2.2.2 and covered further in Section 4.4.5, combined 
with string interpolation, which is covered further in Section 4.2.2.)

##### Possible solution

In test/controllers/static_pages_controller.test.rb

```
def setup
    @base_title = "Ruby on Rails Tutorial Sample App"  
  end
```  

See the completed exerecise controller with complete passing tests

* 4 runs, 8 assertions, 0 failures, 0 errors, 0 skips <- YAY!

##### For exercise 2 the solution is to create a contacts.html.erb page