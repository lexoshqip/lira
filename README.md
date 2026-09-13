# Lira - Biblioteka Dixhitale Shqipe

Ky depozitor (repository) përditësohet përmbajtjen e librave dhe autorëve shqipë që janë disponueshëm publikisht.

## Të Drejtat e Autorit

Të gjitha veprat e paraqitura në këtë depozitor i përkasin autorëve përkatës dhe mbrohën nga të drejtat e autorit (copyright). Ne nuk pretendojmë asnjë të drejtë pronësie mbi këto vepra.

## Përdorimi i Përmbajtjes

Përmbajtja e këtij depozitori mund të përdoret dhe shpërndahet me qëllimin e vetëm të ruajtjes dhe promovimit të letërsisë shqipe, në mënyrë që ajo të mbijetojë me kalimin e kohës.

## Heqja e Përmbajtjes

Nëse jeni autori ose përfaqësuesi ligjor i autorit dhe dëshironi që përmbajtja juaj të hiqet nga ky depozitor, ju lutemi na kontaktoni në:

**info@lexoshqip.org**

Ne do të heqim përmbajtjen tuaj sa më shpejt që të jetë e mundur pas marrjes së kërkesës.

## Deployment (Backblaze B2)

Çdo push në `main` sync automatikisht përmbajtjen në B2 bucket `lexoshqip-lira`.

Para push, gjeneroni `catalog.json`:

```bash
cd ../web
node scripts/generate-catalog.mjs ../lira
```

`catalog.json` është skedari që web app shkarkon gjatë build-it (1 request në vend të shumëfishtë).
