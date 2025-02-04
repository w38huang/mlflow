Deep Learning
=============

The realm of deep learning has witnessed an unprecedented surge, revolutionizing numerous sectors with its ability to
process vast amounts of data and capture intricate patterns. From the real-time object detection in autonomous vehicles
to the generation of art through Generative Adversarial Networks, and from natural language processing applications in
chatbots to predictive analytics in e-commerce, deep learning models are at the forefront of today's AI-driven innovations.

In the deep learning realm, libraries such as PyTorch, Keras, Tensorflow provide handy tools to build and train deep learning
models. MLflow, on the other hand, targets the problem of experiment tracking in deep learning, including logging your
experiment setup (learning rate, batch size, etc) along with training metrics (loss, accuracy, etc) and the model
(architecture, weights, etc). MLflow provides native integrations with deep learning libraries, so you can plug MLflow
into your existing deep learning workflow with minimal changes to your code, and view your experiments in the MLflow UI.

Why MLflow for Deep Learning?
-----------------------------
MLflow offers a list of features that power your deep learning workflows:

* **Experiments Tracking**: MLflow tracks your deep learning experiments, including parameters, metrics, and models.
  Your experiments will be stored in the MLflow server, so you can compare across different experiments and share them.
* **Model Registry**: You can register your trained deep learning models in the MLflow server, so you can easily
  retrieve them later for inference.
* **Model Deployment**: After training, you can serve the trained model with MLflow as a REST API endpoint, so you can
  easily integrate it with your application.

Experiments Tracking
^^^^^^^^^^^^^^^^^^^^
Tracking is the cornerstone of the MLflow ecosystem, and especially vital for the iterative nature of deep learning:

- **Experiments and Runs**: Organize your deep learning projects into experiments, with each experiment containing multiple runs.
  Each run captures essential data like metrics at various training steps, hyperparameters, and the code state.
- **Artifacts**: Store vital outputs such as deep learning models, visualizations, or even tensorboard logs. This artifact
  repository ensures traceability and easy access.
- **Metrics at Steps**: With deep learning's iterative nature, MLflow allows logging metrics at various training steps,
  offering a granular view of the model's progress.
- **Dependencies and Environment**: Capture the computational environment, including deep learning frameworks' versions,
  ensuring reproducibility.
- **Input Examples and Model Signatures**: Define the expected format of the model's inputs, crucial for complex data like
  images or sequences.
- **UI Integration**: The enhanced UI provides a visual overview of deep learning runs, facilitating comparison and insights
  into training progress.
- **Search Functionality**: Efficiently navigate through your deep learning experiments using robust search capabilities.
- **APIs**: Interact with the tracking system programmatically, integrating deep learning workflows seamlessly.


Model Registry
^^^^^^^^^^^^^^
A centralized repository for your deep learning models:

- **Versioning**: Handle multiple iterations and versions of deep learning models, facilitating comparison or reversion.
- **Annotations**: Attach notes, training datasets, or other relevant metadata to models.
- **Lifecycle Stages**: Clearly define the stage of each model version, ensuring clarity in deployment and further fine-tuning.

Model Deployment
^^^^^^^^^^^^^^^^
Transition deep learning models from training to real-world applications:

- **Consistency**: Ensure models, especially those with GPU dependencies, behave consistently across different deployment environments.
- **Docker and GPU Support**: Deploy in containerized environments, ensuring all dependencies, including GPU support, are encapsulated.
- **Scalability**: From deploying a single model to serving multiple distributed deep learning models, MLflow scales as per
  your requirements.

Native Library Support
----------------------
MLflow has native integrations with common deep learning libraries, such as PyTorch, Keras and Tensorflow, so you can plug
MLflow into your workflow easily. The officially supported integrations for deep learning libraries in MLflow encompass:

.. raw:: html

    <section>
        <div class="logo-grid">
            <a href="../models.html#pytorch-pytorch">
                <div class="logo-card">
                    <img src="../_static/images/logos/pytorch-logo.svg" alt="pytorch Logo"/>
                </div>
            </a>
            <a href="../models.html#keras-keras">
                <div class="logo-card">
                    <img src="../_static/images/logos/keras-logo.svg" alt="keras Logo"/>
                </div>
            </a>
            <a href="../models.html#tensorflow-tensorflow">
                <div class="logo-card">
                    <img src="../_static/images/logos/TensorFlow-logo.svg" alt="TensorFlow Logo"/>
                </div>
            </a>
            <a href="../models.html#spacy-spacy">
                <div class="logo-card">
                    <img src="../_static/images/logos/spacy-logo.svg" alt="spaCy Logo"/>
                </div>
            </a>
            <a href="../models.html#fastai-fastai">
                <div class="logo-card">
                    <img src="../_static/images/logos/fastai-logo.png" alt="fast.ai Logo"/>
                </div>
            </a>
        </div>
    </section>

Harness the power of these integrations and elevate your deep learning projects with MLflow's comprehensive support.
For detailed guide on how to integrate MLflow with these libraries, refer to the following pages:

.. raw:: html

    <section>
        <article class="simple-grid">
            <div class="simple-card">
                <a href="tensorflow/index.html">
                    <div class="header">
                        Tensorflow
                    </div>
                    <p>
                        Learn about MLflow's native integration with the Tensorflow library and see example notebooks that leverage
                        MLflow and Tensorflow to build deep learning workflows.
                    </p>
                </a>
            </div>
            <div class="simple-card">
                <a href="pytorch/index.html">
                    <div class="header">
                        Pytorch
                    </div>
                    <p>
                        Learn about MLflow's native integration with the PyTorch library and see example notebooks that leverage
                        MLflow and PyTorch to build deep learning workflows.
                    </p>
                </a>
            </div>

            <div class="simple-card">
                <a href="keras/index.html">
                    <div class="header">
                        Keras
                    </div>
                    <p>
                        Learn about MLflow's native integration with the Keras library and see example notebooks that leverage
                        MLflow and Keras to build deep learning workflows.
                    </p>
                </a>
            </div>
        </article>
    </section>

.. toctree::
    :maxdepth: 1
    :hidden:

    keras/index
    tensorflow/index
    pytorch/index
