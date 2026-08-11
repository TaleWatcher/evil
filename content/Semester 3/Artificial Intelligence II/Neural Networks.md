- Method of computing based on the interaction of multiple connected processing elements called neurons
- Learns from experience to improve their performance
- Can deal with incomplete information
- Comprised of one or more layers of neurons

---

1. Recieves inputs
2. Multiplies each input by its weight
3. Applies activation function to the sum of results
4. Outputs result

# Activation Functions

- Controls whether a neuron is active or inactive
- Different types of activation functions
	- Threshold function
		- Outputs 1 when input is positive, and 0 otherwise
	- Sigmoid function
		- $1/(1+e^{-x})$

# Types of Neural Networks

- Can be classified in different ways
	- Connection type
		- Static (feedforward)
		- Dynamic (feedback)
	- Topology
		- Single layer
		- Multi-layer
		- Recurrent
	- Learning Methods
		- [[Supervized & Unsupervized Learning#Supervized Learning|Supervized]]
		- [[Supervized & Unsupervized Learning#Unsupervized Learning|Unsupervized]]
		- [[Reinforcement Learning|Reinforcement]]

# Applications

- Pattern recognition
- Investment analysis
- Control systems & monitoring
- Mobile computing
- Marketing and financial applications
- Forecasting - sales, market research, meteorology

# Advantages

- Can perform tasks a linear program cannot
- If an element of the neural network fails, it can continue without any problem due to their parallel nature
- Learns and does not need to be programmed
- Can be implemented in any application
- Can be implemented without any problem (??)

# Disadvantages

- Needs training to operate
- Architecture is different from the architecture of microprocessors, and therefore needs to be emulated
- Requires high processing time for large neural networks