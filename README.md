# Batch Connect - Example Spyder App

![GitHub Release](https://img.shields.io/github/release/osc/bc_example_jupyter.svg)
![GitHub License](https://img.shields.io/github/license/osc/bc_example_jupyter.svg)

An example Batch Connect app that launches Spyder within a batch job.

## Prerequisites

This Batch Connect app requires the following software be installed on the
**compute nodes** that the batch job is intended to run on (**NOT** the
OnDemand node):

- [Spyder](https://docs.spyder-ide.org/current/installation.html#conda-based-distributions)
- [Singularity](https://apptainer.org/)
- [TurboVNC](https://www.turbovnc.org/)
- [Lmod](https://www.tacc.utexas.edu/research-development/tacc-projects/lmod)
  6.0.1+ or any other `module purge` and `module load <modules>` based CLI
  used to load appropriate environments within the batch job before launching
  the spyder environment.

## Install

Read the general procedure to develop Open OnDemand apps:
https://osc.github.io/ood-documentation/latest/how-tos/app-development.html

These are command line only installation directions.

Clone this repository to Open OnDemand development directory.

```sh
cd ~/ondemand/dev
git clone git@github.com:SupercomputingWales/scw_ood_spyder.git

# Change the working directory to this new directory
cd scw_ood_spyder
```

From here you will make any modifications to the code that you would like and
version your changes in your own repository:

```sh
#
# Make all your code changes while testing them in the OnDemand Dashboard
#
# ...
#

# Add the files to the Git repository
git add --all

# Commit the staged files to the Git repository
git commit -m "my first commit"
```

## Contributing

1. Fork it ( https://github.com/SupercomputingWales/scw_ood_spyder/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
