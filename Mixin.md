**Mixin** is a way of adding features to a class or an object (or some other thing).

### Alternative explanations
I. A mixin is a class that defines a set of functions relating to a type (e.g. Person, Circle, Observer). Mixins classes are usually considered abstract in that they will not themselves be instantiated – instead their functions are copied (or 'borrowed') by concrete classes as a means of 'inheriting' behaviour without entering into a formal relationship with the behaviour provider.<sup>1</sup>

II. In object-oriented programming languages, a mixin is a class that contains methods for use by other classes without having to be the parent class of those other classes. How those other classes gain access to the mixin's methods depends on the language. Mixins are sometimes described as being "included" rather than "inherited".<sup>2</sup>

### Mixin vs trait
Generally, mixins add logic, while [traits](Trait) add data.

1. Mixins may contain state, (traditional) traits don't.
2. Mixins use "implicit conflict resolution", traits use "explicit conflict resolution"
3. Mixins depends on linearization, traits are flattened.<sup>3</sup>

Martin Odersky in [Programming in Scala](https://www.amazon.co.uk/Programming-Scala-Martin-Odersky/dp/0981531644/) calls traits with behaviour “mixin traits”.

### Examples

#### Python

```python
class Mixin1(object):
    def test(self):
        print "Mixin1"

class Mixin2(object):
    def test(self):
        print "Mixin2"

class MyClass(Mixin2, Mixin1, BaseClass):
    pass
```

#### Ruby

In Ruby, a Module that is included into a Class can be considered a mixin. When you “mixin” a Module into a Class, the Class will have access to the methods of the Module.<sup>4</sup>

```ruby
module Greetings
  def hello
    puts "Hello!"
  end
end

class User
  include Greetings
end
```

#### Sass Mixins
Sass is a CSS extension language. A mixin lets you make groups of CSS declarations that you want to reuse throughout your site. You can even pass in values to make your mixin more flexible. A good use of a mixin is for vendor prefixes. Here's an example for `border-radius`.

```scss
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
}

.box { @include border-radius(10px); }
```

### Articles
1. [JavaScript Code Reuse Patterns: Composition](https://github.com/petsel/javascript-code-reuse-patterns/tree/master/source/components/composition/)
2. [Mixins and C#](https://blogs.msdn.microsoft.com/abhinaba/2006/01/06/mixins-and-c/)
3. [Implementing Mixins with C# Extension Methods](https://www.zorched.net/2008/01/03/implementing-mixins-with-c-extension-methods/)

### Videos
1. [Implementing Mix-ins in Python (Jeff Fischer)](https://www.youtube.com/watch?v=v_uKI2NOLEM)
2. [Demystifying Mixins with Django (Ana Balica)](https://www.youtube.com/watch?v=rMn2wC0PuXw)

---
<div class="footnotes">
1. [[https://javascriptweblog.wordpress.com/2011/05/31/a-fresh-look-at-javascript-mixins/]]
<br>
2. [[https://en.wikipedia.org/wiki/Mixin]]
<br>
3. [[http://stackoverflow.com/questions/925609/mixins-vs-traits]]
<br>
4. [[http://culttt.com/2015/07/08/working-with-mixins-in-ruby/]]
</div>
