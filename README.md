# Lyft-EDA-Ensemble

The data in this competition is packed into .zarr files, which can be loaded with the Python zarr module. Taken from the competition Data description, each .zarr file contains a set of:

scenes: driving episodes acquired from a given vehicle.
frames: snapshots in time of the pose of the vehicle.
agents: a generic entity captured by the vehicle's sensors. Note that only 4 of the 17 possible agent label_probabilities are present in this dataset.
agents_mask: a mask that (for train and validation) masks out objects that aren't useful for training. In test, the mask (provided in files as mask.npz) masks out any test object for which predictions are NOT required.
traffic_light_faces: traffic light information.
