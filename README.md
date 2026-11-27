# all-day-socket
Designing prosthetic sockets that remain comfortable as the residual limb experiences volume changes throughout the day through simulations and machine learning.

## Getting Started
### Prerequisites
Everything runs in Google Colab to allow for heavy training, regardless of user hardware. Obtain a free Google Colab account.

Notebooks 03 and 04 need a GPU. Click the following: Runtime > Change runtime type > T4 GPU.

## Executing Program
Data is not stored in this repo. It is all fully regenerated when running the notebooks.

Run the notebooks in order. Every notebook save its results to Google Drive (MyDrive/all-day-socket/data/)

| # | Notebook | Purpose | Saves |
| :--- | :--- | :--- | :--- |
| 01 | Virtual Patients | Creates 200 synthetic limbs and fluctuating volume versions | `virtual_patients_v1.npz` |
| 02 | Socket Simulator | Converts limbs to a grid, identifies bony zones, creates pressure simulator and PTB baseline | `socket_grids_v1.npz` |
| 03 | Socket Designer | Differentiable simulator, expert optimizer, and the AI designer | `expert_knobs_v1.npz`, `designer_v1.pt` |
| 04 | Experiments | Comparisons, statistics, stress test, liner and sensitivity analysis, learning curve, and figures | `main_results.csv`, `figures/` |

## Credits
OpenLimbTT residual limb shape model from University of Southampton, licensed CC BY-SA 4.0.