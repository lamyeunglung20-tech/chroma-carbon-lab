# Chroma Lab

A bilingual 3D teaching game about carbon dioxide, respiration, photosynthesis and hydrogencarbonate indicator.

[Play the public game](https://chroma-carbon-lab-20261020.grassystone9.chatgpt.site/)

Students explain the biological or chemical cause, predict the net change in carbon dioxide and its concentration, then choose the indicator colour. The 3D indicator changes colour only after the complete explanation is correct. The five cases are a mealworm, soda lime, a variegated leaf in bright light, a leaf shielded by aluminium foil and an indicator-only control.

The interface starts in English and can switch to Traditional Chinese. No student account is needed; progress stays in the browser.

## Run locally

Serve the `dist` directory over HTTP; ES modules will not load reliably from a `file:` URL.

```sh
python3 -m http.server 8000 --directory dist
```

Open <http://localhost:8000>.

## Notes for teachers

The tubes are sealed and initially equilibrated with air. Samples are separated from the indicator. The variegated-leaf case assumes whole-leaf photosynthesis exceeds respiration under the stated bright-light condition. The 3D colour transition illustrates the expected result and does not represent a measured reaction time.

References: [Practical Biology](https://practicalbiology.org/energy/photosynthesis/investigating-photosynthesis-using-immobilised-algae) and [SAPS hydrogencarbonate indicator colour chart](https://s3.eu-west-1.amazonaws.com/assets.saps.org.uk/content/uploads/2022/03/SAPS-Colour-chart-showing-hydrogencarbonate-indicator.pdf).

Three.js is bundled in `dist/vendor/` under its MIT licence notice. The app does not collect analytics or student data.
