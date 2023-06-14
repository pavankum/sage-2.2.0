# Sage-2.2.0

A refit of the Sage 2.1.0, with the same set of training targets as 2.1.0, but optimized hyperparameters for fitting. A much tighter regularization scale on the angles and bonds keeps their equilibrium values closer to the intended initial values obtained from Modified-Seminario method. This resolves remaining issues in the description of Sulfamides (a subset of sulfonamides). The regularization scales used in this iteration, 2.2.0, were 
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
Few Sulfamides with earlier versions of force fields have shown some discrepancies with an overly bent angle around Sulfur atom in the functional group. These issues were resolved in this refit. Here are some of the molecules that were taken from PubChem which were fixed.


