# CNN
## Razorback Logo Detector
- **Objective:** flag Etsy product images that contain the officially licensed Razorback logo so the compliance team can follow up with vendors.
- **Dataset:** 56 manually downloaded Etsy photos + the official mark. Images were labeled into `official` and `not_official` folders, then stratified into 32 train / 12 validation / 12 test items under the standard `ImageFolder` directory structure (`./train`, `./valid`, `./test`).
- **Preprocessing:** every pipeline ends with `Resize((500, 500))` per the project rules, after optional augmentations (cropping/flipping/rotation) meant to fight overfitting on the tiny dataset.
