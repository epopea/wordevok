# The <tt>wordevok</tt> package

This repository contains the <tt>wordevok</tt> <tt>R</tt> package, which transforms evocation data from the *Free Association of Words* survey instrument into relational data for cognitive affinity networks. Two different types of networks are allowed:

* **Network of meanings**  ![\rightarrow](https://render.githubusercontent.com/render/math?math=%5Crightarrow) vertices are words and edges are based on a formula to link words by order of importance and distance, as described in Guedes et al. (2018);
* **Network of individuals** ![\rightarrow](https://render.githubusercontent.com/render/math?math=%5Crightarrow) vertices are individuals and edges are based on a formula to link individuals based on their word vectors, described in Guedes et al. (2018). Two individuals are more cognitive alike the more they share words of same order of importance and distance.

The <tt>wordevok</tt> package contains the following functions:

* <tt>affinity:</tt>	Measures the degree of cognitive affinity between two individuals.
* <tt>as.wordevok:</tt>	Creates an wordevok object.
* <tt>meaning_weighted:</tt>	Calculates the weights attributed to edges in a network of persons linked by cognitive affinity.
* <tt>removing_loops_wordevok:</tt>	Removes loops of a wordevok object.
* <tt>split_list_wordevok:</tt>	Creates subsets of a list according to an object (such as a matrix, data.frame or list) identifying the groups.
* <tt>telp_wordevok:</tt>	Stores the frequency and average order of importance for each evocation.
* <tt>telp_wordevok_plot:</tt> Plots the classical Vergés quadrants.
* <tt>telp_wordevok_quad:</tt>	Split evocations based on in which Vergés quadrant is assigned according to the selected method (mode, median or mean).
* <tt>wordevok_adjacency_to_list:</tt> Transforms an adjacency matrix into an edge list.
* <tt>wordevok_affinity_adjacency:</tt>	Creates a valued adjacency matrix using the affinity coefficient.
* <tt>wordevok_binary_adjacency:</tt>	Creates a non-valued (binary) adjacency matrix, where links are defined if the affinity coefficient is not null.
* <tt>wordevok_comm_submatrix:</tt>	Extracts the adjacency submatrices from the overall adjacency matrix. The extraction is based on an object that identifies groups (or communities).
* <tt>wordevok_comm_subsets:</tt>	Extracts a list containing the evocations of each groug (or community) of the wordevok object.
* <tt>wordevok_intersection_adjacency:</tt>	Creates an adjacency matrix by intersection.
* <tt>wordevok_laplacian_adjacency:</tt>	Creates an adjacency matrix by the Laplacian method.
* <tt>wordevok_meaning_adjacency:</tt>	Creates an adjacency matrix by the weighted meaning method.
* <tt>wordevok_meaning_list:</tt>	Creates an edge list by weighted meaning method.
* <tt>wordevok_quad_class:</tt>	Estimates the relevant coordinates (average evocation order and frequency) for each Vergés quadrant of a given group (or community).
* <tt>wordevok_radar_attr:</tt>	Estimates the relevant coordinates (average evocation order and frequency) for each Vergés quadrant of multiple groups (or communities).
* <tt>wordevok_radar_gg:</tt>	Adjusts the coordinates to be ready to use in radar plots using the <tt>ggplot2 R</>> package.
* <tt>wordevok_radar_plot:</tt>	Generates radar plots of the collective thinking (social representation) of a group (or community) using the <tt>ggplot2 R</>> package. It works for both, network of meanings or network of cognitive affinity. It also accepts multigroup (communities) plotting.

# How to cite

Please, when you use the package give the appropriate credit to the package repository at GitHub and the journal article that provides the methodology and formulas.

* **Traditional format**:
  - For the <tt>wordevok</tt> <tt>R</tt> package:
  Pereira, W., Guedes, G., & Duarte, D. (2020). The wordevok R package for cognitive affinity networks. Github respository. Available at: <https://github.com/epopea/wordevok>.
  - For the formulas and methodology that supports the cognitive affinity network approach:
    Guedes, G. R., Coutinho, R. Z., Marteleto, L., Pereira, W. H. S., & Duarte, D. (2018). Signifying Zika: heterogeneity in the representations of the virus by history of infection. Cadernos de saude publica, 34, e00003217.
* **Bibtex format**:
  - For the <tt>wordevok</tt> <tt>R</tt> package:\
  \
  <code>@misc{pereira_guedes_duarte_2020,</code>\
  <code>author = {Pereira, Wesley and Guedes, Gilvan Ramalho and Duarte, Denise},</code>\
  <code>title = {The wordevok R package for cognitive affinity networks},</code>\
  <code>year = {2020},</code>\
  <code>publisher = {GitHub},</code>\
  <code>journal = {GitHub repository},</code>\
  <code>howpublished = {\url{https://github.com/epopea/wordevok}},</code>\
  <code>commit = {4f57d6a0e4c030202a07a60bc1bb1ed1544bf679}</code>\
  <code>}</code>
  
  - For the formulas and methodology that supports the cognitive affinity network approach:\
  \
  <code>@article{guedes2018signifying,</code>\
  <code>title={Signifying Zika: heterogeneity in the representations of the virus by history of infection},</code>\
  <code>author={Guedes, Gilvan Ramalho and Coutinho, Raquel Zanatta and Marteleto, Leticia and Pereira, Wesley Henrique Silva and Duarte, Denise},</code>\
  <code>journal={Cadernos de saude publica},</code>\
  <code>volume={34},</code>\
  <code>pages={e00003217},</code>\
  <code>year={2018},</code>\
  <code>publisher={SciELO Public Health}</code>\
  <code>}</code>
