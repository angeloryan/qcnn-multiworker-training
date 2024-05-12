# qcnn-multiworker-training

DISCLAIMER: This codebase is sampled from Tensorflow Quantum and Google's [Training with Multiple Workers using TensorFlow Quantum](https://blog.tensorflow.org/2021/06/training-with-multiple-workers-using-tensorflow-quantum.html) blog. Google Cloud is utilized to create multiple workers.

Steps:
1. Use `./setup.sh infra` followed by `./setup.sh params` to set up the necessary Google Cloud resources and initalize parameters into the rest of the code files.
The parameters inside `setup.sh` will need to be modified according to your Google Cloud setup.
2. Run `make training` to create two workers that will then initalize a quantum circuit, respectively, and begin to train data. From here, the edges and weights as well as loss and accuracy should be stored in Google Cloud.