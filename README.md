# ITU-R_P.452_Interference_Prediction
A Python implementation of Recommendation ITU-R P.452-16



# Usage:
```python
from p452_loss import p452_loss as p452
Lb = p452_loss(f, p, d, h, zone, htg, hrg, phi_t, phi_r, Gt, Gr, pol, dct, dcr, DN, N0, pressure, temp)
# or in case of tx, rx clutter losses:
Lb = p452_loss(f, p, d, h, zone, htg, hrg, phi_t, phi_r, Gt, Gr, pol, dct, dcr, DN, N0, pressure, temp,
               ha_t=hat, ha_r=har, dk_r=dkr, dk_t=dkt)

```

'p676-12_table_a.csv' and 'p676-12_table_b.csv' should be also downloaded to source directory, as they are needed to compute specific attenuation due to dry air and water vapour, according to ITU-R P.676-12. 

numpy package should be installed (pip install numpy)





# More info:
ITU-R P.452: Prediction procedure for the evaluation of interference between stations on the surface of the Earth at frequencies above about 0.1 GHz

visit for more info: 

https://www.itu.int/rec/R-REC-P.452-16-201507-I/en


There is a matlab implementation already published by ITU-R Study Group 3, you can download it from below url (validation examples also provided in the site):

https://www.itu.int/en/ITU-R/study-groups/rsg3/Pages/iono-tropo-spheric.aspx
