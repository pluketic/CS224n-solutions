# CS224n: Natural Language Processing with Deep Learning

These past weeks I've spent several weeks on the CS224n course from Stanford University. Here are my solutions
to the assignments. These solutions are for the 2017 version of the course.

## Installation
1. Install [Anaconda](https://www.continuum.io/downloads "Anaconda Official Website")
2. go to assignmentX where X is either 1, 2, 3 using a Terminal:
    ```sh
    $ cd \path\to\assignment1
    ```
3. create a python 2.7 environnment using
    ```sh
    $ conda env -n cs224n python=2.7 anaconda
    ```
4. activate your environment using (add source before activate if you're working with Linux/Mac)
    ```sh
    $ activate cs231n
    ```
5. install the dependencies using requirements.txt
    ```sh
    $ pip install -r requirements.txt
    ```
6. Don't forget to deactivate your environment when you're done (add source before deactivate if you're on Linux/Mac)
    ```sh
    $ deactivate cs224n
    ```

## Issues
If you're working on windows you won't be able to do assignment 2 because the code is for **Python 2.7** and **TensorFlow is only available with Python 3.5 on windows** (at the time I'm writting these lines). So you will
need to create another environment for TensorFlow using:

1. create a python 3.5 environnment using
    ```sh
    $ conda env -n tensorflow python=3.5 anaconda
    ```
2. activate your environment using (add source before activate if you're working with Linux/Mac)
    ```sh
    $ activate tensorflow
    ```
3. install the dependencies using requirements.txt
    ```sh
    $ pip install -r requirements.txt
    ```
5. install TensorFlow (you can also install tensorflow-gpu for the gpu support)
    ```sh
    $ pip install tensorflow
    ```

then you need to convert all the python files from Python 2 to Python 3. To do so you can simply use `2to3`
which is a script included in anaconda to convert Python file from version 2 to version 3 automatically. Simply do:

```sh
$ 2to3 --output-dir=python3-version/assignment2 -W -n assignment2
```

**Note**: If you cloned my repository you won't need to transform the code from Python 2.7 to Python 3.5 as I've
already did it

## More informations
I wrote several blog posts accessible from my [website](https://twice22.github.io/ "Twice22's website")
if you want to understand in detail how the code works.
