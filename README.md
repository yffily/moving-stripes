# moving-stripes

## Purpose

This program creates a movie showing alternating light and dark vertical stripes moving horizontally at constant speed, first left to right, then right to left. The stripes' brightness, width, and speed are tunable. Multiple video segments with different brightnesses, widths, and/or speeds can also be assembled into a single movie.

The program was developed to test the optomotor response (OMR) in fish by measuring their motion in response to the moving stripes.

## Installation and Use

- Install miniconda (instructions at https://docs.anaconda.com/miniconda/).
- Open either the terminal (linux/macOS) or the anaconda prompt (windows). Navigate to the folder containing this README as well as "OMR.yml" and "OMR.ipynb".
- Create a new conda environment using "OMR.yml": in the terminal, execute "conda env create -f OMR.yml".
- Start jupyter notebook: in the same terminal, execute "conda activate OMR", then "jupyter notebook". The jupyter notebook should appear in an internet browser window.
- Open "OMR.ipynb": Initially the jupyter notebook behaves like a file browser, i.e., it shows the files present in the current directory. One of them should be "OMR.ipynb". Click on it.
- Once "OMR.ipynb" is open in the jupyter notebook, edit the following parameter values as needed for your use case:
    * Edit height_cm, width_cm, and cm_to_px to reflect the size and resolution of the screen on which you intend to play the movie.
    * Edit period_list, speed_list, contrast_list, n_repeat, and pattern_duration to create the desired stripe pattern.
- Still in the jupyter notebook, click "Run", then "Run All Cells". If the notebook runs properly, two new files and one new subfolder will appear in the folder containing the notebook: the movie itself (movie.mp4), spreadsheet recapping the stripe patterns used in the movie (pattern_sequence.xlsx), and a subfolder containing the single-pattern movies used to assemble the final movie (tmp).

## Questions

If you have a question about the program, ask Yaouen Fily (yfily@fau.edu).

If you have a question about the optomotor response assay for which the program was developed, ask Johanna Kowalko (jok421@lehigh.edu).