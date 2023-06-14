# Sage-2.2.0

This repository contains a refit of Sage version 2.1.0, using the same training targets as the original version. However, we have optimized the hyperparameters for better fitting. To achieve this, we have implemented significantly tighter regularization scales on the angles and bonds, which helps maintain their equilibrium values closer to the intended initial values obtained from the Modified-Seminario method. This approach effectively resolves any remaining issues in the description of Sulfamides, which is a subset of sulfonamides.

In this iteration, version 2.2.0, we have utilized these specific regularization scales during valence parameter optimization, 
```
priors
   Angles/Angle/k :  5.0
   Angles/Angle/angle :  1.0
   Bonds/Bond/k :  10.0
   Bonds/Bond/length :  0.01
   ProperTorsions/Proper/k :  5.0
   ImproperTorsions/Improper/k :  5.0
/priors

```

# Improvements in Sulfamides
Sulfamides are a subset of Sulfonamides. Previously, certain Sulfamides encountered discrepancies in earlier versions of force fields, particularly the angle around the Sulfur atom in the functional group appeared overly bent. However, these angle-related anomalies have been successfully resolved in the current refit. 

Here are a few examples of molecules sourced from PubChem that were rectified during this process.

![image](https://github.com/pavankum/sage-2.2.0/assets/16142894/8eeed184-9736-402e-9089-5db48074fdb5)
![image](https://github.com/pavankum/sage-2.2.0/assets/16142894/2f1cb0a0-8f7d-4ac3-9fe2-a22e1cae7b76)
![image](https://github.com/pavankum/sage-2.2.0/assets/16142894/f6355b13-d7b5-4b9d-8cd8-49ea1795e68f)



