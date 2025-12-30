# Rate Distortion Theory Tutorial

An interactive Docker-based Jupyter Notebook application that teaches the fundamental concepts of **Rate Distortion Theory**, a cornerstone of information theory developed by Claude Shannon.

## Overview

This tutorial provides:
- 📚 Clear explanations of rate distortion theory concepts
- 🧮 Mathematical foundations with the rate-distortion function
- 📊 Interactive visualizations and examples
- 🎛️ Adjustable parameters to explore trade-offs
- 💡 Practical applications in communications and compression

## What is Rate Distortion Theory?

Rate Distortion Theory addresses the fundamental trade-off between:
- **Rate (R)**: The number of bits per symbol needed for compression
- **Distortion (D)**: The quality loss from compression

Shannon proved that for any distortion level D, there exists a theoretical minimum rate R(D) that cannot be improved upon.

## Prerequisites

- Docker installed on your system ([Get Docker](https://docs.docker.com/get-docker/))
- Docker Compose (usually included with Docker Desktop)

## Quick Start

### Option 1: Using Docker Compose (Recommended)

1. Clone this repository:
```bash
git clone https://github.com/mjs161803/rate-distortion-theory-tutorial.git
cd rate-distortion-theory-tutorial
```

2. Build and run the container:
```bash
docker-compose up --build
```

3. Open your browser and navigate to:
```
http://localhost:8888
```

4. Open the `rate_distortion_tutorial.ipynb` notebook and start learning!

### Option 2: Using Docker directly

1. Build the Docker image:
```bash
docker build -t rate-distortion-tutorial .
```

2. Run the container:
```bash
docker run -p 8888:8888 -v $(pwd):/app rate-distortion-tutorial
```

3. Access the notebook at `http://localhost:8888`

## Tutorial Contents

The notebook includes:

1. **Introduction to Rate Distortion Theory**
   - Historical context and Claude Shannon's contributions
   - Key concepts and terminology

2. **Mathematical Foundation**
   - Rate-distortion function definition
   - Gaussian source example with closed-form solution

3. **Interactive Visualizations**
   - Rate-distortion curves with adjustable parameters
   - Real-time exploration of trade-offs

4. **Practical Example: Signal Compression**
   - Gaussian signal generation
   - Uniform quantization demonstration
   - Comparison with theoretical bounds

5. **Interactive Compression Demo**
   - Adjust source variance and quantization levels
   - Observe effects on rate and distortion
   - Visualize original vs. compressed signals

6. **Applications**
   - Image/video compression (JPEG, MPEG, H.264)
   - Audio compression (MP3, AAC)
   - Wireless communications
   - Machine learning model compression

## Key Features

- **Interactive Widgets**: Use sliders to adjust parameters in real-time
- **Comprehensive Visualizations**: Multiple plots showing different aspects of compression
- **Theoretical Bounds**: Compare practical methods with Shannon's limits
- **Educational Focus**: Clear explanations suitable for students and professionals

## Learning Objectives

After completing this tutorial, you will understand:
- The fundamental trade-off between compression rate and quality
- How to calculate and interpret rate-distortion functions
- Why certain compression ratios are theoretically impossible
- How practical compression schemes relate to theoretical limits
- Applications of rate distortion theory in modern technology

## Stopping the Container

Press `Ctrl+C` in the terminal where docker-compose is running, or:

```bash
docker-compose down
```

## Security Note

⚠️ **For Local Use Only**: This application is configured for ease of use in a local development/educational environment with no authentication. It should **NOT** be deployed to production or exposed to the internet without proper security measures:

- Add authentication tokens
- Use HTTPS
- Implement proper access controls
- Review and harden Docker security settings

For local educational purposes, the current configuration is appropriate and convenient.

## Technologies Used

- **Python 3.11**: Core programming language
- **Jupyter Notebook**: Interactive computing environment
- **NumPy**: Numerical computations
- **Matplotlib**: Plotting and visualization
- **SciPy**: Scientific computing
- **ipywidgets**: Interactive widgets
- **Docker**: Containerization

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest improvements
- Add new examples
- Enhance visualizations

## License

This project is open source and available for educational purposes.

## References

1. Shannon, C. E. (1959). "Coding theorems for a discrete source with a fidelity criterion"
2. Cover, T. M., & Thomas, J. A. (2006). "Elements of Information Theory"
3. Berger, T. (1971). "Rate Distortion Theory: A Mathematical Basis for Data Compression"

## Author

Created as an educational resource to make information theory concepts accessible and interactive.

---

**Start exploring the fascinating world of rate distortion theory!** 🚀
