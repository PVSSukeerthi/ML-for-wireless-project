# ML for Wireless Project: Beamspace Channel Estimation

This project implements a **Deep Learning-based Beamspace Channel Estimation** method for mmWave Massive MIMO systems using a **Switch-Based Selection Network**.The **DeepMIMO dataset** is used for training and evaluation

---

## DeepMIMO Dataset Setup

This project **requires the DeepMIMO dataset**.

### a. Download DeepMIMO

- Clone the official DeepMIMO repository:
  ```bash
  git clone https://github.com/DeepMIMO/DeepMIMO.git
  ```

### b. Configure Scenario

- Use **Scenario O1** in DeepMIMO.
- Set the following parameters inside the DeepMIMO configuration:
  - `scenario = 'O1'`
  - `active_BS = [1, 2, 3]`
  - `user_rows = range(1200, 2200)`
  - `num_paths = 3`
  - `carrier_frequency = 28e9`
  - Antenna array:
    - UPA: `1 x 16 x 16`
    - ULA: `1 x 256 x 1`

Generate the dataset using the DeepMIMO script you get 2 csv files each for ULA and UPA.The data set we have used are also included into DeepMIMO folder with the code we have use to generate it.

---

## Running

- For  Saleh-Valenzuela  with OMP and Attention UNET for ULA and UPA

  ```bash
  OMP_Unet_SV.ipynb
  ```

- **For  DeepMIMO with OMP and Attention UNET for ULA and UPA**

  ```bash
  OMP_Unet_DeepMIMO.ipynb
  ```

---

## References

- [DeepMIMO Official GitHub](https://github.com/DeepMIMO/DeepMIMO-python)
- [DeepMIMO_scenario](https://www.deepmimo.net/)
- [**Deep Learning-based Beamspace Channel Estimation** method for mmWave Massive MIMO systems using a **Switch-Based Selection Network**](https://ieeexplore.ieee.org/abstract/document/10570856/)
