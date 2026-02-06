#Quantum Fourier Transform on Simulated Chirp Signals

A proof-of-concept exploring how Quantum Fourier Transform (QFT) performs on chirp signals — the kind of waveform produced by events like black hole mergers — using IBM Qiskit's simulator at hyper-low qubit counts.

##Why This Matters
Real quantum hardware is expensive and noisy. Before running anything on actual qubits, you need to validate your approach in simulation. This notebook demonstrates:

-Simulated chirp signal generation — mimicking the frequency sweeps found in gravitational wave data
-QFT at low qubit counts — testing whether meaningful frequency separation is achievable with minimal quantum resources
-Hybrid FFT + QFT workflow — laying groundwork for complementary classical/quantum analysis of chirp signals

##The Idea
Chirp signals are an ideal test case for QFT because their frequency content evolves over time — exactly the kind of structure that Fourier methods need to resolve. By keeping the data window small and the qubit count low, we can prototype quantum signal processing pipelines that could eventually scale to real LIGO data on real quantum hardware.

##Run It
Open the notebook in Google Colab or locally with Jupyter. Requires qiskit and standard scientific Python libraries.

##Build On Top:

Noise modeling from actual IBM quantum backends
Comparison of QFT vs classical FFT resolution at equivalent bit depths
Application to real LIGO strain data segments
