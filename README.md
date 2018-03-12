# Tensorflow "for Humans"

Well, not quite, as I can't claim this is a beautifully crafted library like HTTP for Humans. I wish I had time for such things.

But in the spirit of "for humans" understandability, I made a somewhat "canonical-esque" example of image recognition using TF. I'd rather have spent more time to produce something more in the spirit of Socratic learning, which is a style of "coding" I have found useful with one of my sons. Maybe I'll find time.

In this example, I made a shape generator (using [Pillow](https://pillow.readthedocs.io/en/latest/)) that will enable the student to play with features a bit more than taking the standard MNIST (or similar) datasets.
This is in the [shape_generator file](generate_shapes.ipynb) which also contains some data pre-processing (and notes about such).
Here, the data is also split out into training, validation and testing sets and then pre-packaged (via Pickle) ready to import into the [classifier](tensor_flow_for_humans.ipynb) itself.

I prepend the actual classifier example (i.e. recognizing the shapes) with a gentle introduction to tensors and the graph-based nature of TF.

My goal was to make the example (from end to end) as easy to understand as possible and to be easily fiddled with, which I encourage you to do.
 
To follow along, you will need at least some basic introduction to Deep Learning. I've seen the Udacity one (which inspired my example) and I believe that this example is a more accessible first intro to TF.
All complex math is avoided, as it's not necessary to follow along.

Unlike Udacity's intro, here I use a proper TF optimizer (e.g. a primivite neural layer construct) rather than a manually programmed perceptron layer.
To me, this makes more sense as you can immediately play with other optimizers and the real "juice" of TF.

If you want to get into the real basics of perceptron "math" and hand-crafting a net, then I suggest not using TF and using pure Python.
Something like [Grokking Deep Learning](https://www.manning.com/books/grokking-deep-learning) might serve you well.