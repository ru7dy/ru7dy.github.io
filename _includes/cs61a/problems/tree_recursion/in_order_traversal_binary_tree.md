{% capture question %}
This problem uses the Tree Class defined [here.]({% code tree %})

This problem is a challenge problem and might touch on some concepts taught mainly in CS61B. However, as a CS61A student who has learned all about tree recursion, you should be able to complete a problem like this.

We like to be able to traverse our trees in order to get all of the elements back into some sort of list. We can traverse the tree in many different ways. In Order Traversal is one of them and the algorithm goes like this. First, we will recursively print out all the values to our left, then, we will print out the current node's entry, then recursively print out all the values on the right. Take a look at the doctests below if you are still confused. Post in the comments section if you are still confused after reading the doctests.

    def in_order_traversal(tree):
        """
        >>> t = Tree(5, Tree(1, None, Tree(4)), Tree(7, Tree(6), Tree(8)))
        >>> in_order_traversal(t)
        1
        4
        5
        6
        7
        8
        """
        "***YOUR CODE HERE***"
{% endcapture %}

{% capture solution %}
    def in_order_traversal(tree):
        """
        >>> t = Tree(5, Tree(1, None, Tree(4)), Tree(7, Tree(6), Tree(8)))
        >>> in_order_traversal(t)
        1
        4
        5
        6
        7
        8
        """
        if tree is None:
            return
        in_order_traversal(tree.left)
        print(tree.entry)
        in_order_traversal(tree.right)
{% endcapture %}

{% include cs61a/problem_template.md %}
