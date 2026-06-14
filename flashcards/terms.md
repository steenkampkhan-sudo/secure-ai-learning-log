neural network; A machine learning model, loosely inspired by biological neurons, built from layers of simple units whose connection strengths are learned from data.
neuron; A unit that sums a group of weighted inputs plus a bias, applies an activation function to that sum, and returns the result as its output.
weights; Learned values that control the strength of the connection between two neurons, set during training and fixed thereafter.
bias; A learned constant added to a neuron's weighted input before the activation function is applied.
parameters; A model's complete set of learned values (its weights and biases), fixed after training; a "70-billion-parameter model" has that many of them.
activation function; A function applied to a neuron's weighted-sum-plus-bias that introduces nonlinearity, without which a network of any depth would collapse into a single linear transformation.
input layer; The first layer of a network, which receives the input as numbers (one neuron per attribute in a tabular model, or one embedding vector per token in an LLM).
output layer; The final layer of a network, which produces the model's prediction (for an LLM, a probability across the whole vocabulary for the next token).
token; A discrete chunk of text that the vocabulary maps to an integer ID.
discrete chunk; A subword fragment of text that is a single member of the vocabulary.
vocabulary; The model's fixed, finite list of every possible token, each paired with an integer ID.
tokenisation; The process of segmenting raw text into subword tokens and encoding each as its integer ID from the vocabulary.
dense vector; A vector whose entries are (mostly) meaningful non-zero numbers, unlike a sparse vector, which is almost entirely zeros.
embedding vector; A learned, dense vector of real numbers, retrieved from the embedding matrix by a token's ID, that places the token in a continuous space where distance and direction between vectors encode semantic and syntactic relationships.
embedding matrix; The lookup table holding one learned embedding vector for every token in the vocabulary.
attention; A mechanism in which each token compares itself against every other token and absorbs information from the ones it finds most relevant, so a word's representation shifts with its context.
transformer; A neural network architecture that uses attention to let every token draw on every other token, processing the whole sequence in parallel through many stacked layers.
loss; A single number measuring how wrong a model's prediction is on a training example, which training works to minimise.
gradient; For a given parameter, a measure of how much and in which direction the loss would change if that parameter were nudged, which is what tells training which way to adjust it.
backpropagation; The algorithm that computes, for every parameter, how much it contributed to the loss (its gradient), so each can be nudged to reduce that loss.
gradient descent; The optimisation step that adjusts each parameter a small amount in the direction that most reduces the loss, repeated until the loss stops falling.
training; The iterative process of adjusting a model's parameters to minimise the loss, using backpropagation to find each parameter's gradient and gradient descent to step it in the loss-reducing direction.
gradient;
gradient descent;
cost function;
