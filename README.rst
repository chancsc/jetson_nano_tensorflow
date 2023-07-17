Install Tensorflow 2.5 on Jetson Nano
-------------------------------------

.. code:: bash

    Model:   NVIDIA Jetson Nano Developer Kit (4 GB ram)
    Jetpack: 4.6.4
    CUDA:    10.2.300
    Python:  3.6.9

1. Setup python virtual env, follow this `guide <https://pyimagesearch.com/2020/03/25/how-to-configure-your-nvidia-jetson-nano-for-computer-vision-and-deep-learning/>`_

2. Follow this `guide <https://qengineering.eu/install-tensorflow-2.4.0-on-jetson-nano.html/>`_ (the sudo pip3 change and remove the sudo)


3. Ensure numpy version is 1.19.4, else will crash tensorflow

.. code:: bash
  
    pip install numpy==1.19.4

4. choose a version & downlaod

    https://developer.download.nvidia.com/compute/redist/jp/v46/tensorflow/

5. install tensorflow

.. code:: bash
  
    pip install tensorflow-2.5.0+nv21.7-cp36-cp36m-linux_aarch64.whl

6. Follow this guide (the sudo pip3 change and remove the sudo)

  https://qengineering.eu/install-tensorflow-2.4.0-on-jetson-nano.html


Reference: PIP Requirements:

.. code:: bash

    $ pip list
    Package                 Version
    ----------------------- -------------------
    absl-py                 0.15.0
    appdirs                 1.4.4
    astor                   0.8.1
    astunparse              1.6.3
    beautifulsoup4          4.12.2
    bokeh                   2.3.3
    cachetools              4.2.4
    certifi                 2023.5.7
    charset-normalizer      2.0.12
    coverage                6.2
    cycler                  0.11.0
    Cython                  0.29.21
    dataclasses             0.8
    decorator               5.1.1
    filelock                3.4.1
    flatbuffers             1.12
    future                  0.18.3
    futures                 3.0.5
    gast                    0.4.0
    gdown                   4.7.1
    google-auth             2.22.0
    google-auth-oauthlib    0.4.6
    google-pasta            0.2.0
    grpcio                  1.34.1
    h5py                    2.10.0
    idna                    3.4
    importlib-metadata      4.8.3
    importlib-resources     5.4.0
    Jinja2                  3.0.3
    joblib                  1.1.1
    Keras-Applications      1.0.8
    keras-nightly           2.5.0.dev2021032900
    Keras-Preprocessing     1.1.2
    kiwisolver              1.3.1
    lxml                    4.9.3
    Mako                    1.1.6
    Markdown                3.3.7
    MarkupSafe              2.0.1
    matplotlib              3.3.4
    mock                    5.1.0
    multitasking            0.0.11
    mypy                    0.971
    mypy-extensions         1.0.0
    numpy                   1.19.4
    oauthlib                3.2.2
    opt-einsum              3.3.0
    packaging               21.3
    pandas                  1.1.5
    pbr                     5.11.1
    Pillow                  8.4.0
    pip                     21.3.1
    pkgconfig               1.5.5
    platformdirs            2.4.0
    protobuf                3.19.6
    pyaml                   23.5.8
    pyasn1                  0.5.0
    pyasn1-modules          0.3.0
    pybind11                2.10.4
    pycuda                  2020.1
    pyparsing               3.1.0
    PySocks                 1.7.1
    python-dateutil         2.8.2
    pytools                 2022.1.12
    pytz                    2023.3
    PyYAML                  6.0
    requests                2.27.1
    requests-oauthlib       1.3.1
    rsa                     4.9
    scikit-learn            0.24.2
    scikit-optimize         0.9.0
    scipy                   1.5.4
    seaborn                 0.11.2
    setuptools              59.6.0
    six                     1.15.0
    soupsieve               2.3.2.post1
    tensorboard             2.10.1
    tensorboard-data-server 0.6.1
    tensorboard-plugin-wit  1.8.1
    tensorflow              2.5.0+nv21.7
    tensorflow-estimator    2.5.0
    termcolor               1.1.0
    testresources           2.0.1
    tflite-runtime          2.1.0.post1
    threadpoolctl           3.1.0
    tomli                   1.2.3
    tornado                 6.1
    tqdm                    4.64.1
    typed-ast               1.5.5
    typing-extensions       3.7.4.3
    urllib3                 1.26.16
    Werkzeug                2.0.3
    wheel                   0.37.1
    wrapt                   1.12.1
    yfinance                0.1.64
    zipp                    3.6.0

Issues:
=======
Some work around if have error

.. code:: bash

    ln -s /usr/include/locale.h /usr/include/xlocale.h

