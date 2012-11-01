This is a script I created in response to the University of Chicago admissions essay question,
"So where is Waldo, really?" It was inspired by [a StackOverflow response](http://stackoverflow.com/questions/8479058/how-do-i-find-waldo-with-mathematica) that implemented rudimentary Waldo detection in Mathematica. This solution follows a more versatile algorithm in Python, supported by NumPy, SciPy, Scikits-Image, and the Python Imaging Library. I have published a version of the accompanying [counselor-friendly essay](https://s3.amazonaws.com/jsevart-web/waldo_public.pdf), though I will not distribute Handford's entire drawings publicly.

If you'd like to run this yourself, it works on Python 2.7.3 with the latest versions of the four aforementioned libraries. You may need to boost the contrast of the images you're working with so that red-white borders are clear, and replace my reference values and color distance thresholds for red, white, and black (in the L*ab colorspace) with your own. Input images must be in RGBA colorspace, and my pixel counts are only tested to work with images where a single page is 1285x666.