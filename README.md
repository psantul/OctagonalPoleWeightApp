# Octagonal Pole Weight Calculator (Android)

- Open in **Android Studio (Giraffe+ / Hedgehog+)**.
- Let Gradle sync, then go to **Build > Build Bundle(s) / APK(s) > Build APK(s)** to generate an APK.
- Inputs: Material, Thickness (mm), Height (m), Top OD (mm), Bottom OD (mm), Base Plate L*W*T (mm).
- Assumes ODs are **across flats** of a regular octagon.
- Formulae:
  - Perimeter P ≈ K·D_af, with K = 3.313708499.
  - Slant height s = √(h² + ((D_bot − D_top)/2)²)/1000 (m) using meters.
  - Lateral area A ≈ ((P_top + P_bottom)/2) · s.
  - Volume V = A · t (t in meters).
  - Weight W = V · density.
