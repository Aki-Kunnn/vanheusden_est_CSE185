# CSE-185-Final-Project

This is a demonstration project for CSE185. It implements a recreation of the kmergenie tool. See the [Kmergenie](http://kmergenie.bx.psu.edu/) page for more details.

# Install Instructions

Clone the repository and change directory:

```bash
git clone https://github.com/Aki-Kunnn/vanheusden_est_CSE185.git

cd ~/vanheusden_est_CSE185

pip install -r requirements.txt

pip install .

cd vanheusden
```

# Example Usage
The following command generated a random genome of length 10,000 and used that to simulate a fasta file with 10,000 reads of length 100 and an error rate of 0.001.

```
python3 vanheusden.py generate -g 10000 -n 10000 -l 100 -e 0.001
```

Then the following command estimated the genome size to be 10142: 

```
python3 vanheusden.py estimate -k 30 g10000_n10000_l100_e0.001.fastq
```

# Options
python3 vanheusden.py generate -g [genome size] -n [number of reads] -l [length of reads] -e [error rate]

python3 vanheusden.py estimate [fasta file]

# Contributors

This repository was generated by Jonathan Lam, Edward Tang, and Richard Xu, with inspiration from Kmergenie as the main project.

We'd also like to thank Rohan Vanheusden for inspiring the name of this project!

Please submit a pull request with any corrections or suggestions.
