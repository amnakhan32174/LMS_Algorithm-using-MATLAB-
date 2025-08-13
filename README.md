# LMS Adaptive Noise Cancellation in MATLAB

This project implements an **adaptive noise cancellation system** using the **Least Mean Squares (LMS) algorithm** in MATLAB. The system is designed to remove additive noise from a clean sinusoidal signal, demonstrating real-time adaptive filtering and performance evaluation.


## Features

- Generates a clean sine wave as the desired signal.
- Adds **additive white Gaussian noise** to simulate a noisy environment.
- Implements an **LMS adaptive filter** to reduce noise.
- Tracks **Mean Squared Error (MSE)** over iterations to monitor convergence.
- Provides **visualizations**:
  - Error vs Iteration
  - Comparison of Clean, Noisy, and Filtered Signals
  - Error before and after filtering
- Calculates a **confusion matrix** to quantify detection of noise removal.
- Exports confusion matrix to an Excel file (`LMS.xlsx`) for further analysis.


## Parameters

- `N` – Number of samples
- `fs` – Sampling frequency
- `f` – Frequency of the sine wave
- `mu` – Step size of LMS algorithm
- `M` – Filter length
- `MSEth` – Threshold for declaring successful noise removal

## Usage

1. Open MATLAB and navigate to the project folder.
2. Run the script `main.m` (or the filename containing this code).
3. Observe outputs:
   - Iterative MSE printed in the command window
   - Plots showing filtering performance
   - Confusion matrix saved/appended in `LMS.xlsx`



## Example Plots

- **Error vs Iteration**: Visualizes squared error reduction over time.  
- **Noise Cancellation Result**: Compares clean signal, noisy input, and LMS output.  
- **Error Before vs After Filtering**: Shows the improvement in signal quality after adaptive filtering.


## MSE Evaluation

- `MSE_before` – Error between noisy input and desired signal.  
- `MSE_after` – Error between LMS output and desired signal.  
- If `MSE_after < MSEth`, the system declares successful noise removal.

## Author

Amna Nadeem Khan – https://github.com/amnakhan32174

---

## License

This project is open-source and free to use under the MIT License.
