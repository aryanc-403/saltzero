

see the python stuff for the "reference impl", this will have much fewer comments


Libraries like frugally-deep were tested to predict directly in C++ but end up being significantly slower (by a factor of about 5x on every 1000 queries) than calling the python interpreter (probably because batching is not possible in frugally-deep, but is possible in tensorflow). 