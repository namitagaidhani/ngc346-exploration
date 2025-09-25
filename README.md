# ngc346-exploration

This project started in March 2025, when I decided to dive deeper into astronomy and coding out of pure passion and curiosity. I wanted to learn how to handle real telescope data instead of just reading about stars in textbooks. My goal with this project was to verify known information about NGC 346 with Python, Google Colab, and JWST datasets. This program begins my exploration into space with real-world applications of astrophysics principles that I have learned through USAAAO preparation.

For my first target, I chose NGC 346, a young star-forming region in the Small Magellanic Cloud (SMC), one of our neighboring galaxies.

I worked with two filters from JWST:
* F090W (near-infrared, shorter wavelength, roughly comparable to “blue” light for JWST’s detectors)
* F150W (near-infrared, a bit longer wavelength, somewhat like “red”)
By comparing these two filters, I calculated the color index of stars. The color index shows the difference in brightness of a star between two wavelengths and is defined as:

    _Color Index_ = Magnitude(F090W) – Magnitude(F150W)
* Negative color index (blue side): Hot, young stars.
* Positive color index (red side): Cooler stars, often older or at different evolutionary stages.

The raw data was downloaded from the MAST (Mikulski Archive for Space Telescopes) in FITS format (Flexible Image Transport System), which is the standard for astronomy data. Using Python, I did the following steps:
1. Open and explore the FITS images.
2. Detect stars and measure their brightness (flux) in both filters.
3. Convert flux into magnitudes.
4. Match stars across both filters to calculate color indices.
5. Plot a Color-Magnitude Diagram (CMD) for NGC 346.

The Color-Magnitude Diagram (CMD) plots:
* X-axis = color index (F090W – F150W) → gives information about temperature.
* Y-axis = magnitude in F150W → measures brightness (with brighter stars at the top).

**Result**: From the CMD, I could see that NGC 346 contains many bright, blue stars, which makes sense since it is a region of ongoing star formation. At the same time, there are stars scattered toward the red side, representing cooler or more evolved stars.
