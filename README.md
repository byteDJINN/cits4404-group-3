# cits4404-group-3

## Dependencies

You will need the following libraries installed:

- `numpy`: Used for numerical operations. Install with `pip install numpy`.
- `imageio`: Provides an easy interface to read and write a wide range of image data. Install with `pip install imageio`.
- `matplotlib`: A plotting library which offers similar functionality to MATLAB. Install with `pip install matplotlib`.
- `scikit-learn`: Machine learning library used in this script for calculating euclidean distances. Install with `pip install scikit-learn`.
- `opencv-python`: Open Source Computer Vision Library, used here for image processing tasks. Install with `pip install opencv-python`.
- `Shapely`: Used for manipulation and analysis of planar geometric objects. Install with `pip install Shapely`.

Ensure you have the latest versions of these libraries to avoid any compatibility issues.

## Running the Code

To run the script, you will need to define six variables.

In the `genetic algorithm` itself: 
- `iterations`: The number of iterations the genetic algorithm will run for. We have selected `200` as a benchmark.
- `swarm_size`: The population size used by the genetic algorithm to position a single worm within the image. `20` is our benchmark.
- `n_worms`: The number of worms to go into the image. `200` is our benchmark.

In the cost function within the `Fitness` class:
- `internal_weight`: The influence of the internal factors of the worm.
- `group_weight`: The influence of group factors of the worm.
- `environmental_weight`: The influence of environmental factors of the worm.
All of these weight values default to 1, and produce decent results at this value.

1. Run through the notebook running each of the classes until you reach `Fitness`. At the bottom of the fitness class you will see:
    # driver weights 
    Wi = 1
    Wg = 1
    We = 1

    tweak these values with your desired driver weights.

2. Keep running through the notebook until you reach `The Genetic Algorithm`. Towards the top you will see:
    # constants
    iterations = 200
    swarm_size = 30
    num_swarms = 10

    tweak these values to your liking.
3. Run `The Genetic Algorithm` code block and watch as the algorithm prints out its progress, yielding a final result.
