---
title: Code Syntax
---
To insert highlight code inside of a post, it's enough to use some specific tags, has directly described into the [Jekyll documentation](http://jekyllrb.com/docs/templates/#code-snippet-highlighting). In this way the code will be included into a ``.highlight`` CSS class and will be highlight according to the [syntax.scss](https://github.com/mojombo/tpw/blob/master/css/syntax.css) file. This is the standard style adopted by **Github** to highlight the code. 

This is a CSS example:
{% highlight css linenos %}

body {
  background-color: #fff;
  }

h1 {
  color: #ffaa33;
  font-size: 1.5em;
  }

{% endhighlight %}

And this is a HTML example, with a linenumber:
{% highlight html linenos %}

<html>
  <a href="example.com">Example</a>
</html>

{% endhighlight %}

Last, a Ruby example:
{% highlight ruby linenos %}

def hello
  puts "Hello World!"
end

{% endhighlight %}


Last, a Julia example:

{% highlight julia linenos %}

function hello()
  print("Hello World!")
end

type CamClay
  a::Int
  b::Vector{Int}
end


"""
Elastic 
\alpha + \beta = 1
"""

#Elastic 
#\alpha + \beta = 1



function De(model::CamClay, x::Int)
  return ones(1,4)
end 

{% endhighlight %}

```
$$ 5 + 5 $$


\$$ 5 + 5 $$

$$ a^2 + b^2 = c^2 $$
```
$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

$$\frac{a}{b} = 1$$

$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$
$$\frac{(n^2+n)(2n+1)}{6}$$
