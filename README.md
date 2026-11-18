# Passport, visa and ID photo requirements

The photo size, background, glasses rule and file limits of **164 passport, visa, residence and ID documents**, each read on the issuing authority's own page and dated. Rules read up to 17 November 2026.

Maintained by [WinPhoto ID](https://winphoto.io/id), a free passport and visa photo checker that runs in the browser. Each row links to a page with the official source, the quoted rules and a free check of your own photo.

## Files

| File | What it holds |
|---|---|
| [`photo-sizes.csv`](photo-sizes.csv) | One row per document, 21 columns |
| [`photo-sizes.json`](photo-sizes.json) | The same rows, with the column list, the method and summary counts |

The live table is at <https://winphoto.io/id/photo-sizes> (also as [CSV](https://winphoto.io/id/photo-sizes.csv) and [JSON](https://winphoto.io/id/photo-sizes.json)). This repository is a copy; the live table is updated first.

## What the table shows

- 164 passport, visa and ID documents from 66 countries are in the table, each read on the issuing authority's own page.
- Of the 93 documents with a printed photo size on record, 52 are 35 x 45 mm, 18 are 51 x 51 mm (2 x 2 inches) and 23 are another size; 12 different sizes appear in all.
- Of the 136 documents with a background rule on record, 87 ask for white; the other 49 do not ask for white alone, and 5 of those say the background must not be white.
- Of the 85 documents whose rules mention glasses, 22 do not allow them at all.
- 10 documents ask for a photo taken by a commercial photographer or studio, and 9 more say someone else must take it: no selfie.
- 79 documents publish a maximum file size for a digital photo, from 20 KB (Pakistani passport photo online) to 10,000 KB.

## Columns

| Column | Meaning |
|---|---|
| `country` | Issuing country |
| `country_code` | ISO 3166-1 alpha-2 code |
| `document` | The document, as its authority names it |
| `id` | Stable identifier of the row |
| `page_url` | The document's page on winphoto.io: quoted rules, sources, free photo check |
| `print_width_mm` | Printed photo width in millimetres, where a print size is published |
| `print_height_mm` | Printed photo height in millimetres |
| `print_size_label` | The size as the authority words it, when it is a range or a minimum |
| `width_px_min` | Smallest accepted width in pixels, for digital photos |
| `width_px_max` | Largest accepted width in pixels |
| `height_px_min` | Smallest accepted height in pixels |
| `height_px_max` | Largest accepted height in pixels |
| `file_formats` | Accepted file types |
| `min_kb` | Smallest accepted file size in kilobytes |
| `max_kb` | Largest accepted file size in kilobytes |
| `background` | The background rule in the authority's words |
| `background_class` | The background rule as a class (white, light, not white, ...) |
| `glasses` | Whether glasses are allowed |
| `taken_by` | Who must take the photo, when the rules say (a professional, someone else) |
| `rules_read` | The date the official page was last read |
| `source_url` | The official page the rule comes from |

An empty cell means the official page states no such rule, or the document needs no photo from the applicant.

## The documents

| Country | Document | Photo size | Background | Rules read |
|---|---|---|---|---|
| Armenia | [Armenia e-Visa (evisa.mfa.am) facial photo upload](https://winphoto.io/id/am_evisa) | 250–6000 x 250–6000 px | not coloured: the photo requirements panel lists 'Back side is colored' among Not Valid Photos; its valid examples are on plain white to light grey | 2026-11-05 |
| Australia | [Australia Electronic Travel Authority (ETA, subclass 601), live photo in the app](https://winphoto.io/id/au_eta) | no photo to prepare, or no size published |  | 2026-11-04 |
| Australia | [Australian citizenship application photo (ImmiAccount upload; 35-40 x 45-50 mm print for paper and Form 1195)](https://winphoto.io/id/au_citizenship) | 35-40 mm wide x 45-50 mm high (35 x 45 mm is the smallest allowed) | neutral or light grey, contrasting with the face; no shadows on the background | 2026-11-04 |
| Australia | [Australian passport (printed photos)](https://winphoto.io/id/au_passport) | 35–40 mm wide x 45–50 mm high (35 x 45 mm is the smallest allowed) | plain white or light grey, contrasting with the face | 2026-11-04 |
| Australia | [Australian passport for a baby or young child (printed photos)](https://winphoto.io/id/au_passport_baby) | 35–40 mm wide x 45–50 mm high (35 x 45 mm is the smallest allowed) | plain white or light grey, contrasting with the face | 2026-11-04 |
| Australia | [Australian visa application photo (ImmiAccount digital upload; passport-size print for paper)](https://winphoto.io/id/au_visa) | 45 mm x 35 mm passport photograph | neutral or light grey, contrasting with the face | 2026-11-04 |
| Australia | [Australian visa photo for a baby or child (ImmiAccount digital upload; passport-size print for paper)](https://winphoto.io/id/au_visa_child) | 45 mm x 35 mm passport photograph | neutral or light grey, contrasting with the face | 2026-11-12 |
| Austria | [Austrian passport (Reisepass) and identity card (Personalausweis), printed photo](https://winphoto.io/id/at_passport) | 35 mm wide x 45 mm high | plain light colour, ideally grey (medium grey behind light hair, light grey behind dark hair); no pattern, no shadows, enough contrast with face and hair | 2026-11-04 |
| Austria | [Austrian residence permit (Aufenthaltstitel) application, printed passport photo 35 x 45 mm](https://winphoto.io/id/at_residence_permit) | 35 mm wide x 45 mm high | plain light colour, ideally grey (medium grey behind light hair, light grey behind dark hair); no pattern, no shadows, enough contrast with face and hair | 2026-11-15 |
| Austria | [Austrian visa application (all visa types, Schengen C and national D included), printed passport photo 35 x 45 mm](https://winphoto.io/id/at_visa) | 35 mm wide x 45 mm high | plain light colour, ideally grey (medium grey behind light hair, light grey behind dark hair); no pattern, enough contrast with face and hair | 2026-11-15 |
| Bangladesh | [Bangladesh e-passport (photo captured at biometric enrolment)](https://winphoto.io/id/bd_epassport) | 3R (under 6 only; no further size rule given) |  | 2026-11-04 |
| Bangladesh | [Bangladesh visa (online MRV application on visa.gov.bd) photo](https://winphoto.io/id/bd_visa) | 45 mm x 35 mm (35 mm wide, 45 mm high) | white (the printed visa form: 'Photograph has to be white background') | 2026-11-16 |
| Belgium | [Belgian passport and electronic identity card (eID), printed photo](https://winphoto.io/id/be_passport) | 35 mm wide x 45 mm high | light-coloured, plain and even, no colour gradient, enough contrast with the head; strong blue or red backgrounds excluded | 2026-11-04 |
| Botswana | [Botswana e-Visa (evisa.gov.bw) applicant photo](https://winphoto.io/id/bw_evisa) | 28 mm x 36 mm (digital upload) | white (the application's photo step says white; the Photo Requirements page says plain light) | 2026-11-16 |
| Brazil | [Brazil e-Visa (VIVIS visit visa online, citizens of Australia, Canada, the US and China) photo](https://winphoto.io/id/br_evisa) | 2 x 2 inches | white | 2026-11-04 |
| Brazil | [Brazilian passport (passaporte comum), applied for in Brazil at the Polícia Federal](https://winphoto.io/id/br_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| Canada | [Canada Electronic Travel Authorization (eTA), no photo](https://winphoto.io/id/ca_eta) | no photo to prepare, or no size published |  | 2026-11-04 |
| Canada | [Canada Temporary Resident (visitor) Visa application photo (IRCC)](https://winphoto.io/id/ca_visitor_visa) | at least 35 mm x 45 mm | plain white or light-coloured | 2026-11-16 |
| Canada | [Canada permanent residence / permanent resident (PR) card photo](https://winphoto.io/id/ca_pr_card) | 50 mm x 70 mm (2 x 2 3/4 inches); 715–2000 x 1000–2800 px | plain, untextured and white | 2026-11-15 |
| Canada | [Canada permanent residence / permanent resident (PR) card photo for a baby or child](https://winphoto.io/id/ca_pr_card_baby) | 50 mm x 70 mm (2 x 2 3/4 inches); 715–2000 x 1000–2800 px | plain, untextured and white; a newborn in a car seat needs a white blanket over the seat behind the head | 2026-11-15 |
| Canada | [Canada study permit application photo (IRCC)](https://winphoto.io/id/ca_study_permit) | at least 35 mm x 45 mm | plain white or light-coloured | 2026-11-15 |
| Canada | [Canada super visa (parents and grandparents) application photo (IRCC)](https://winphoto.io/id/ca_super_visa) | at least 35 mm x 45 mm | plain white or light-coloured | 2026-11-15 |
| Canada | [Canada work permit application photo (IRCC), with the International Experience Canada digital photo](https://winphoto.io/id/ca_work_permit) | at least 35 mm x 45 mm | plain white or light-coloured | 2026-11-15 |
| Canada | [Canadian child passport for a baby or young child (printed photos)](https://winphoto.io/id/ca_passport_baby) | 50 mm x 70 mm (2 x 2 3/4 inches) | plain white or light-coloured, clear difference between the child's face and the background; a newborn in a car seat needs a white blanket over the seat behind the head | 2026-11-04 |
| Canada | [Canadian citizenship application photo (citizenship grant, proof of citizenship certificate, renunciation)](https://winphoto.io/id/ca_citizenship) | 50 mm x 70 mm (2 x 2 3/4 inches); 420 x 540 px | plain white or light-coloured, with a clear difference between the face and the background | 2026-11-04 |
| Canada | [Canadian passport, in person or by mail (printed photos)](https://winphoto.io/id/ca_passport) | 50 mm x 70 mm (2 x 2 3/4 inches) | plain white or light-coloured, clear difference between face and background | 2026-11-04 |
| Canada | [Canadian passport, online renewal (digital photo)](https://winphoto.io/id/ca_passport_online_renewal) | 1200–3000 x 1800–4500 px | plain white or light-coloured, clear difference between face and background | 2026-11-04 |
| China | [Chinese passport and travel document (旅行证) photo for citizens abroad (China Consular app upload; 33x48 mm prints)](https://winphoto.io/id/cn_passport) | 33 mm wide x 48 mm high | pure white, even, no shadows (MFA form: uniform white) | 2026-11-04 |
| China | [Chinese visa application photo (paper 33x48 mm and online-form digital photo)](https://winphoto.io/id/cn_visa) | 33 mm wide x 48 mm high; 354–420 x 472–560 px | white (some posts: white or close to white), no border | 2026-11-04 |
| Colombia | [Colombian visa, online application photo (Cancillería visa form)](https://winphoto.io/id/co_visa) | 3 x 4 cm (the size the form gives for the uploaded photo) | white | 2026-11-04 |
| Czech Republic (Czechia) | [Czech residence permit photo (Ministry of the Interior), printed 35 x 45 mm](https://winphoto.io/id/cz_residence_permit) | 35 mm wide x 45 mm high | white to light blue or light grey; a smooth transition between these colours is allowed | 2026-11-15 |
| Czech Republic (Czechia) | [Czech visa application photo (Schengen and long-term visa), printed 35 x 45 mm](https://winphoto.io/id/cz_visa) | 35 mm wide x 45 mm high | white to light blue or light grey (Interior Ministry); white or light (Embassy in Tokyo) | 2026-11-15 |
| Democratic Republic of the Congo | [DR Congo eVisa (evisa.gouv.cd) ID photo upload](https://winphoto.io/id/cd_evisa) | 100 x 200 px | plain and light (required from 1 December 2026; no background rule is stated before that date) | 2026-11-16 |
| Denmark | [Danish residence permit and residence card: facial image recorded with your fingerprints (biometric features)](https://winphoto.io/id/dk_residence_permit) | no photo to prepare, or no size published |  | 2026-11-15 |
| Djibouti | [Djibouti eVisa (evisa.gouv.dj) photograph upload](https://winphoto.io/id/dj_evisa) | no photo to prepare, or no size published |  | 2026-11-16 |
| Ethiopia | [Ethiopia e-Visa (evisa.gov.et) applicant photo](https://winphoto.io/id/et_evisa) | 2 x 2 inches | white (photo tips); a blurred or unclean background is not acceptable (upload notes) | 2026-11-05 |
| France | [French passport and carte nationale d'identité (CNI), identity photo](https://winphoto.io/id/fr_passport) | 35 mm wide x 45 mm high | plain, light colour (light blue or light grey for example); white is forbidden | 2026-11-04 |
| France | [French residence permit (titre de séjour, carte de séjour) photo: e-photo code online, or three printed photos](https://winphoto.io/id/fr_titre_sejour) | 35 mm wide x 45 mm high | plain, light colour (light blue or light grey for example); white is forbidden | 2026-11-15 |
| Georgia | [Georgia e-Visa (evisa.gov.ge) applicant photo upload](https://winphoto.io/id/ge_evisa) | no photo to prepare, or no size published | not stated in words; the portal's linked sheet of sample photos shows correct photos on plain, light backgrounds (light blue to white) | 2026-11-04 |
| Germany | [German national visa (type D: work, study, training, family reunion), printed biometric photo for the mission appointment](https://winphoto.io/id/de_national_visa) | 35 mm wide x 45 mm high | one plain bright colour, ideally neutral grey (medium grey behind light hair, light grey behind dark hair), contrasting with face and hair; no pattern, no shadows | 2026-11-15 |
| Germany | [German passport (Reisepass) and identity card (Personalausweis) photo, applied for in Germany](https://winphoto.io/id/de_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| Germany | [German passport (Reisepass) and identity card photo, applied for at a German embassy or consulate abroad (printed 35x45 mm)](https://winphoto.io/id/de_passport_abroad) | 35 mm wide x 45 mm high | plain single colour, shadow-free, in clear contrast with face and hair; preferably light grey (BMI template); Addis Ababa: white or light grey | 2026-11-04 |
| Germany | [German residence permit (elektronischer Aufenthaltstitel, eAT): digital photo taken at the foreigners authority or sent by a certified photo service](https://winphoto.io/id/de_residence_permit) | no photo to prepare, or no size published |  | 2026-11-15 |
| Ghana | [Ghana biometric passport, online application photo upload (passport.mfa.gov.gh, in Ghana or at a mission)](https://winphoto.io/id/gh_passport) | 140 x 170 px | white | 2026-11-04 |
| Greece | [Greek passport photo (digital via myPhoto in Greece; upload or print at consulates abroad)](https://winphoto.io/id/gr_passport) | 1280 x 1600 px | digital file: grey, about RGB 190,190,190 (+/- 10); printed photo abroad (2018 sheet): white, cream or 5% grey | 2026-11-04 |
| Hong Kong | [Hong Kong SAR passport photo (40 x 50 mm print, or a JPEG of at least 1200 x 1600 px for the online application)](https://winphoto.io/id/hk_passport) | 40 mm wide x 50 mm high; 1200 x 1600 px | plain white | 2026-11-15 |
| India | [All India Sainik Schools Entrance Examination (AISSEE) application photograph, signature and left-hand thumb impression](https://winphoto.io/id/in_aissee) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [CMAT application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_cmat) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [CTET application photograph and signature (Central Teacher Eligibility Test, CBSE)](https://winphoto.io/id/in_ctet) | no photo to prepare, or no size published | not stated in the bulletin | 2026-11-17 |
| India | [CUET (PG) application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_cuet_pg) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [CUET (UG) application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_cuet_ug) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [GATE application photograph and signature (Graduate Aptitude Test in Engineering)](https://winphoto.io/id/in_gate) | 200–530 x 260–690 px | white, with no other objects or persons | 2026-11-17 |
| India | [IBPS PO and Clerk application photograph, signature, left thumb impression and hand-written declaration](https://winphoto.io/id/in_ibps) | 200 x 230 px | light-coloured, preferably white | 2026-11-17 |
| India | [India e-Visa (e-Tourist, e-Business, e-Medical, etc.) applicant photograph](https://winphoto.io/id/in_evisa) | no photo to prepare, or no size published | plain light coloured or white | 2026-11-04 |
| India | [Indian PAN (Permanent Account Number) card application photo (Form 93 / Form 95 / PAN change request, photos pasted on the form or acknowledgement)](https://winphoto.io/id/in_pan_card) | 4.5 cm x 3.5 cm (35 mm wide x 45 mm high) | white | 2026-11-04 |
| India | [Indian passport (paper form at DPC/SPC/CSC in India; ICAO digital upload for applications through Indian missions abroad)](https://winphoto.io/id/in_passport) | 4.5 cm x 3.5 cm (35 mm wide x 45 mm high); 630 x 810 px | plain white | 2026-11-04 |
| India | [Indian passport for a child under 4 (printed photo carried to the PSK/POPSK/Passport Office; ICAO digital upload for applications through Indian missions abroad)](https://winphoto.io/id/in_passport_baby) | 4.5 cm x 3.5 cm (35 mm wide x 45 mm high); 630 x 810 px | plain white | 2026-11-04 |
| India | [Indian regular (paper) visa photo: digital upload on indianvisaonline.gov.in and the print pasted on the signed form](https://winphoto.io/id/in_visa_regular) | 2 x 2 inches; 350–1000 x 350–1000 px | plain light coloured or white (portal); plain white, no borders (High Commission in Ottawa) | 2026-11-04 |
| India | [JEE (Main) application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_jee_main) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [Joint CSIR-UGC NET application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_csir_net) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [NEET (UG) application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_neet_ug) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [NIFT entrance (NIFTEE) application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_niftee) | no photo to prepare, or no size published | white | 2026-11-17 |
| India | [Overseas Citizen of India (OCI) card application photo](https://winphoto.io/id/in_oci) | square, not less than 51 x 51 mm; 200–900 x 200–900 px | plain light colour, NOT white, no border | 2026-11-04 |
| India | [SBI PO and Junior Associate (Clerk) application photograph, signature, left-hand thumb impression and hand-written declaration](https://winphoto.io/id/in_sbi) | 200 x 230 px | light-coloured, preferably white | 2026-11-17 |
| India | [SSC application photograph and signature (Staff Selection Commission: CGL, CHSL, Constable GD)](https://winphoto.io/id/in_ssc) | no photo to prepare, or no size published | plain background, good light (live capture) | 2026-11-17 |
| India | [UGC NET application form photograph and signature (National Testing Agency)](https://winphoto.io/id/in_ugc_net) | no photo to prepare, or no size published | white | 2026-11-17 |
| Indonesia | [Indonesia e-Visa and e-VOA (evisa.imigrasi.go.id) profile photo](https://winphoto.io/id/id_evisa) | 4 x 6 cm (digital upload, at least 400 x 600 pixels); 400 x 600 px | not stated on the e-Visa portal; Indonesian missions ask for a white background (Caracas, embassy-issued visas) | 2026-11-04 |
| Indonesia | [Indonesian passport (applied on M-Paspor, photo taken at the immigration office)](https://winphoto.io/id/id_passport) | no photo to prepare, or no size published |  | 2026-11-12 |
| Iraq | [Iraq e-Visa (evisa.iq) digital photo](https://winphoto.io/id/iq_evisa) | no photo to prepare, or no size published | white | 2026-11-16 |
| Ireland | [Irish passport book or passport card, online application (digital photo)](https://winphoto.io/id/ie_passport_online) | 715 x 951 px | completely plain light grey, white or cream, with enough contrast | 2026-11-04 |
| Ireland | [Irish passport for a baby or young child, online application (digital photo)](https://winphoto.io/id/ie_passport_baby) | 715 x 951 px | completely plain light grey, white or cream with enough contrast; a baby who cannot support themselves lies on a plain, white surface | 2026-11-04 |
| Ireland | [Irish visa application photos: two identical printed photos, 35 to 38 mm wide and 45 to 50 mm high](https://winphoto.io/id/ie_visa) | 35 to 38 mm wide x 45 to 50 mm high (35 x 45 mm is the smallest allowed) | plain white or light grey, with good contrast between your face and the background; no shadows or glare | 2026-11-15 |
| Italy | [Italian electronic passport, printed photo (Questura, Commissariato or Italian consulate)](https://winphoto.io/id/it_passport) | 35 mm wide x 45 mm high | white, evenly lit; nothing and no one else in the background | 2026-11-04 |
| Jamaica | [Jamaican passport photo (35 x 45 mm prints; digital photo for the PICA online adult renewal)](https://winphoto.io/id/jm_passport) | 35 mm wide x 45 mm high | plain, no shadows: white for a dark complexion, pastel shaded for a light complexion, pale blue or pastel for grey/white hair (simplified renewal sheet: off-white, pale blue for grey/white or bleached hair) | 2026-11-04 |
| Japan | [JAPAN eVISA (evisa.mofa.go.jp) facial photo upload](https://winphoto.io/id/jp_evisa) | no photo to prepare, or no size published | plain and untextured (no colour named) | 2026-11-16 |
| Japan | [Japan residence card and Certificate of Eligibility application photo (Immigration Services Agency, 4 cm x 3 cm)](https://winphoto.io/id/jp_residence_card) | 4 cm high x 3 cm wide | no background, shadows included; a dark background that hides the outline is refused | 2026-11-15 |
| Japan | [Japan visa application photo (paper form at an embassy, consulate or accredited agency)](https://winphoto.io/id/jp_visa) | 35 mm wide x 45 mm high (MOFA form: 45mm x 35mm or 2in x 1.4in; some posts differ) | plain; most posts say white (Mumbai, Denver, Malaysia: white; Chicago: white or off-white; Houston: white or blue; Azerbaijan: plain colour-neutral, not necessarily white) | 2026-11-04 |
| Japan | [Japanese passport (旅券) application photo, printed 35 x 45 mm or uploaded in the online application (Mynaportal / ORRnet)](https://winphoto.io/id/jp_passport) | 35 mm wide x 45 mm high, no border | no background (plain, shadows included); white recommended, the traditional pale blue also accepted; no gradation, no pattern or textured wallcovering, no objects, not dark; clear contrast with face and hair | 2026-11-05 |
| Kenya | [Kenya Electronic Travel Authorisation (eTA) photo](https://winphoto.io/id/ke_eta) | no photo to prepare, or no size published |  | 2026-11-04 |
| Kenya | [Kenyan e-passport (applied on eCitizen, photo captured at biometrics)](https://winphoto.io/id/ke_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| Kuwait | [Kuwait e-visa face photo (Ministry of Interior Kuwait Visa platform: tourist and family visit visas)](https://winphoto.io/id/kw_evisa) | 30 mm wide x 40 mm high (digital upload); 720 x 720 px | white (FAQ); plain white or light grey, plain, even and uniform, no shadows or glare (upload instructions) | 2026-11-04 |
| Laos | [Laos eVisa (laoevisa.gov.la) applicant photo](https://winphoto.io/id/la_evisa) | 4 x 6 cm (digital upload); 300 x 300 px | plain white, no shadows | 2026-11-05 |
| Libya | [Libya e-visa (evisa.gov.ly) personal photo upload](https://winphoto.io/id/ly_evisa) | no photo to prepare, or no size published | white | 2026-11-16 |
| Malaysia | [Malaysia Employment Pass and expatriate pass photo (ESD Online, 35 x 50 mm, at most 25 KB)](https://winphoto.io/id/my_employment_pass) | 35 mm wide x 50 mm high | plain white, no border or frame (required for every pass type from 1 December 2026; until then plain blue is also accepted for VDR applications) | 2026-11-15 |
| Malaysia | [Malaysia eVISA photo (MyVISA portal; Visa Without Reference rules, Visa With Reference noted)](https://winphoto.io/id/my_evisa) | 35 mm wide x 50 mm high | plain white, no border or frame (VTR); plain white or plain blue (VDR) | 2026-11-04 |
| Mexico | [Mexican passport (pasaporte ordinario)](https://winphoto.io/id/mx_passport) | tamaño pasaporte (no millimetre size stated) | white | 2026-11-04 |
| Mexico | [Mexican visa applied for at an embassy or consulate (visitor, student, temporary or permanent resident)](https://winphoto.io/id/mx_visa) | no photo to prepare, or no size published |  | 2026-11-04 |
| Morocco | [Morocco eVisa (acces-maroc.ma) identity photo upload](https://winphoto.io/id/ma_evisa) | 35 x 45 mm | not stated for the eVisa beyond the ICAO standard; Moroccan consulates ask for a white background on visa photos, so white is used | 2026-11-04 |
| Myanmar | [Myanmar eVisa (evisa.moip.gov.mm) applicant photo: tourist and business eVisa](https://winphoto.io/id/mm_evisa) | 3.8 x 4.6 cm, or 1.5 x 1.8 inches (digital upload) | plain white or off-white | 2026-11-05 |
| Netherlands | [Dutch MVV long-stay visa (provisional residence permit), printed passport photo for the embassy appointment](https://winphoto.io/id/nl_mvv_visa) | 35 mm wide x 45 mm high | light grey, light blue or white; plain, one colour, no fade, enough contrast with the head | 2026-11-15 |
| Netherlands | [Dutch passport and identity card (ID-kaart), printed photo](https://winphoto.io/id/nl_passport) | 35 mm wide x 45 mm high | light grey, light blue or white; plain, one colour, no gradient, no shadow, enough contrast with the head | 2026-11-04 |
| Netherlands | [Dutch residence permit card (verblijfsdocument): photo taken by the IND at the biometrics appointment](https://winphoto.io/id/nl_residence_permit) | no photo to prepare, or no size published |  | 2026-11-15 |
| New Zealand | [New Zealand Electronic Travel Authority (NZeTA) photo, online form](https://winphoto.io/id/nz_nzeta) | 900–2250 x 1200–3000 px | plain and neutral, good contrast with the face; INZ photographer guide: plain, light-coloured (not white) | 2026-11-04 |
| New Zealand | [New Zealand passport (digital photo)](https://winphoto.io/id/nz_passport) | 900–4500 x 1200–6000 px | plain, light-coloured, strong contrast with the face, no shadows or objects | 2026-11-04 |
| New Zealand | [New Zealand passport for a baby or child (digital photo)](https://winphoto.io/id/nz_passport_baby) | 900–4500 x 1200–6000 px | a plain, light-coloured sheet under the baby, photographed from above; strong contrast with the face, no shadows or objects | 2026-11-04 |
| New Zealand | [New Zealand visa application photo (online upload; 35x45 mm prints for paper forms)](https://winphoto.io/id/nz_visa) | 35 mm wide x 45 mm high (paper applications); 900–2250 x 1200–3000 px | plain and neutral, good contrast with the face; INZ photographer guide: plain, light-coloured (not white) | 2026-11-04 |
| Nigeria | [Nigeria e-Visa (evisa.immigration.gov.ng) applicant photo upload](https://winphoto.io/id/ng_visa) | no photo to prepare, or no size published | white | 2026-11-05 |
| Nigeria | [Nigerian standard e-passport, online application photo upload (NIS portal, in Nigeria or abroad)](https://winphoto.io/id/ng_passport) | 600 x 800 px | white | 2026-11-04 |
| Norway | [Norwegian visa, residence permit and residence card (UDI): photo taken by the police or the foreign service mission](https://winphoto.io/id/no_residence_permit) | no photo to prepare, or no size published |  | 2026-11-15 |
| Oman | [Oman eVisa personal photo (Royal Oman Police eVisa portal)](https://winphoto.io/id/om_evisa) | no photo to prepare, or no size published | clear background (no colour named) | 2026-11-04 |
| Pakistan | [Pakistan online visa (Pakistan Online Visa System, visa.nadra.gov.pk) applicant photograph](https://winphoto.io/id/pk_evisa) | 35 mm wide x 45 mm high; 350 x 467 px | plain white (photograph guide and application guide); the guide's style section also says a plain light-coloured background | 2026-11-05 |
| Pakistan | [Pakistani passport, online application for Pakistanis abroad (DGI&P e-Services portal, photo upload)](https://winphoto.io/id/pk_passport) | 35 mm wide x 45 mm high (as a digital file of at most 20KB) | plain white | 2026-11-04 |
| Peru | [Peruvian visa (tourist and similar) application photo, as set by each Peruvian consulate](https://winphoto.io/id/pe_visa) | passport size; 3.5 x 4.5 cm, 35 x 43 mm or 2 x 2 in depending on the consulate | white (Santiago: plain white) | 2026-11-04 |
| Philippines | [Philippine passport (photo captured live by DFA)](https://winphoto.io/id/ph_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| Philippines | [Philippine visa (9(a) temporary visitor and other non-immigrant visas at embassies and consulates)](https://winphoto.io/id/ph_visa) | 3.5 cm x 4.5 cm (New York, Paris); some posts ask 2 x 2 in | white | 2026-11-04 |
| Poland | [Polish passport and ID card (dowód osobisty) photo: 35 x 45 mm print, or file for an online application](https://winphoto.io/id/pl_passport) | 35 mm wide x 45 mm high; 768 x 1004 px | white, evenly lit, no shadows or decorative elements (the passport act says a uniform light background) | 2026-11-04 |
| Qatar | [Qatar e-visa personal photo (Hayya platform: tourist and other Hayya entry visas)](https://winphoto.io/id/qa_visa) | 30 mm wide x 40 mm high (digital upload); 720 x 720 px | plain white or light grey, even and uniform, no shadows or glare | 2026-11-04 |
| Russia | [Russian unified e-visa (единая электронная виза) applicant face photo](https://winphoto.io/id/ru_evisa) | no photo to prepare, or no size published | plain light-coloured, no shadows | 2026-11-04 |
| Saudi Arabia | [Saudi Arabia tourist e-visa (Visit Saudi eVisa) personal photo](https://winphoto.io/id/sa_evisa) | 200 x 200 px | white, no pattern, no shadows (visa.visitsaudi.com); plain (ksavisa.sa) | 2026-11-17 |
| Schengen Area (France-Visas and German missions quoted) | [Schengen short-stay visa (type C) application photo, ICAO format](https://winphoto.io/id/schengen_visa) | 35 mm x 45 mm (France-Visas: 35–40 mm wide) | plain light-coloured (France-Visas); white (German mission in Dhaka) | 2026-11-04 |
| Singapore | [Singapore Long-Term Visit Pass (LTVP) application photo (ICA e-Service upload, 400 x 514 px)](https://winphoto.io/id/sg_ltvp) | 400 x 514 px | white | 2026-11-15 |
| Singapore | [Singapore citizenship application photo (ICA e-Service upload, 400 x 514 px)](https://winphoto.io/id/sg_citizenship) | 400 x 514 px | white | 2026-11-15 |
| Singapore | [Singapore entry visa application photo (ICA e-Service upload 400 x 514 px, or a 35 x 45 mm print with Form 14A)](https://winphoto.io/id/sg_visa) | 35 mm wide x 45 mm high; 400 x 514 px | plain white, no shadows | 2026-11-04 |
| Singapore | [Singapore identity card (NRIC) photo (ICA e-Service upload, 400 x 514 px)](https://winphoto.io/id/sg_nric) | 400 x 514 px | white | 2026-11-15 |
| Singapore | [Singapore passport photo (MyICA online application 400 x 514 px, or a 35 x 45 mm print with the overseas form)](https://winphoto.io/id/sg_passport) | 35 mm wide x 45 mm high; 400 x 514 px | plain white; light grey if your hair is white | 2026-11-12 |
| Singapore | [Singapore permanent residence (PR) application photo (ICA e-Service upload, 400 x 514 px)](https://winphoto.io/id/sg_pr) | 400 x 514 px | white | 2026-11-15 |
| South Africa | [South African passport (tourist, child, official), printed photos where not captured live](https://winphoto.io/id/za_passport) | 35 mm x 45 mm | light grey or plain cream-coloured (DHA leaflet); white at the Tokyo mission | 2026-11-04 |
| South Korea | [South Korea K-ETA (Korea Electronic Travel Authorization) face photo](https://winphoto.io/id/kr_keta) | no photo to prepare, or no size published |  | 2026-11-04 |
| South Korea | [South Korea visa application photo (visa form and Korea Visa Portal e-Form, 3.5 x 4.5 cm)](https://winphoto.io/id/kr_visa) | 3.5 cm x 4.5 cm (US posts: 2 x 2 in) | white (Korea Visa Portal); the visa form and some embassies also accept off-white | 2026-11-04 |
| South Korea | [South Korean passport photo (3.5 x 4.5 cm print, or the online reissue file of about 413 x 531 px)](https://winphoto.io/id/kr_passport) | 3.5 cm wide x 4.5 cm high; 395–431 x 507–550 px | uniform white, no ink marks, no border | 2026-11-12 |
| Spain | [Spanish passport and DNI (national identity card), printed photo 32 x 26 mm](https://winphoto.io/id/es_passport) | 26 mm wide x 32 mm high (written '32 x 26 mm') | plain, uniform white | 2026-11-04 |
| Sri Lanka | [Sri Lanka ETA (Electronic Travel Authorization, eta.gov.lk) - no photo required](https://winphoto.io/id/lk_eta) | no photo to prepare, or no size published |  | 2026-11-04 |
| Sweden | [Swedish passport and national ID card (photo taken at the police passport office)](https://winphoto.io/id/se_passport) | no photo to prepare, or no size published |  | 2026-11-12 |
| Sweden | [Swedish residence permit card (uppehållstillståndskort): photographed and fingerprinted by the Migration Agency or an embassy](https://winphoto.io/id/se_residence_permit) | no photo to prepare, or no size published |  | 2026-11-15 |
| Taiwan | [Taiwan (Republic of China) passport photo (35 x 45 mm print, and a JPG of at least 413 x 531 px for the online system)](https://winphoto.io/id/tw_passport) | 45 mm high x 35 mm wide (1.77 x 1.38 in); 413 x 531 px | plain white, no shadows or reflections | 2026-11-15 |
| Taiwan | [Taiwan (Republic of China) visa application photo (paper photos for a visitor or resident visa at a Taiwan overseas mission)](https://winphoto.io/id/tw_visa) | 35 mm wide x 45 mm high | plain white, uniform lighting, no shadows or reflections | 2026-11-04 |
| Taiwan | [Taiwan Alien Resident Certificate (ARC) photo (National Immigration Agency application form, 4.5 x 3.5 cm)](https://winphoto.io/id/tw_arc) | 4.5 cm high x 3.5 cm wide | white | 2026-11-16 |
| Tanzania | [Tanzania e-Visa (visa.immigration.go.tz) applicant photo](https://winphoto.io/id/tz_evisa) | 35 mm wide x 45 mm high (digital upload) | plain (no colour named); no distracting shadows or images on the background | 2026-11-05 |
| Thailand | [Thailand e-Visa (thaievisa.go.th) applicant photograph](https://winphoto.io/id/th_evisa) | passport size, 3.5 x 4.5 cm shape (Dhaka mission; US consulates ask 2 x 2 in) | white (Doha: white only; Singapore: plain white or off-white; Los Angeles: plain/blank/white) | 2026-11-04 |
| Togo | [Togo e-visa (Togo Voyage, voyage.gouv.tg) identity photo](https://winphoto.io/id/tg_evisa) | no photo to prepare, or no size published | light colour, even, plain, no gradient | 2026-11-16 |
| Trinidad and Tobago | [Trinidad and Tobago machine-readable passport photo](https://winphoto.io/id/tt_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| Turkey (Türkiye) | [Turkish passport and identity card (kimlik kartı) biometric photo, 50 x 60 mm print](https://winphoto.io/id/tr_passport) | 50 mm wide x 60 mm high (not 35 x 45 mm) | white, without pattern and without shadows | 2026-11-12 |
| Turkey (Türkiye) | [Türkiye e-Visa (evisa.gov.tr) - no photo required](https://winphoto.io/id/tr_evisa) | no photo to prepare, or no size published |  | 2026-11-04 |
| Turkey (Türkiye) | [Türkiye residence permit (ikamet izni) biometric photo: e-İkamet upload and prints for the appointment](https://winphoto.io/id/tr_residence_permit) | 5 x 6 cm (50 x 60 mm), as provincial offices state; no central size is published | white (e-İkamet document lists and goc.gov.tr); plain, no pattern and no shadow; the 2020 ICAO note prefers mid grey behind light hair | 2026-11-04 |
| Ukraine | [Ukrainian passport for travel abroad (biometric 'zakordonnyi pasport'), applied for in Ukraine or at a consulate](https://winphoto.io/id/ua_passport) | no photo to prepare, or no size published |  | 2026-11-04 |
| United Arab Emirates | [UAE Emirates ID card photo (ICP personal photo, 4.5 x 3.5 cm, white background)](https://winphoto.io/id/ae_emirates_id) | 4.5 cm x 3.5 cm | white | 2026-11-15 |
| United Kingdom | [UK Electronic Travel Authorisation (ETA), face photo](https://winphoto.io/id/uk_eta) | 600 x 750 px | plain light-coloured, in clear contrast to the person | 2026-11-04 |
| United Kingdom | [UK passport for a baby or child, paper application (printed photos)](https://winphoto.io/id/uk_passport_baby) | 35 mm wide x 45 mm high | plain cream or light grey, in clear contrast to the face | 2026-11-04 |
| United Kingdom | [UK passport, online application (digital photo)](https://winphoto.io/id/uk_passport_online) | 600 x 750 px | plain light-coloured, in clear contrast to the face | 2026-11-04 |
| United Kingdom | [UK passport, paper application (printed photos)](https://winphoto.io/id/uk_passport_print) | 35 mm wide x 45 mm high | plain cream or light grey, in clear contrast to the face | 2026-11-04 |
| United Kingdom | [UK visa application from outside the UK (entry clearance), facial photo](https://winphoto.io/id/uk_visa) | no photo to prepare, or no size published |  | 2026-11-04 |
| United Kingdom | [UK visa or permission application, digital photo of your face uploaded online (UKVI)](https://winphoto.io/id/uk_visa_digital_photo) | 600 x 750 px | plain light-coloured, in clear contrast to you | 2026-11-15 |
| United Kingdom (Northern Ireland) | [Northern Ireland photocard driving licence (DVA), printed photo for postal applications](https://winphoto.io/id/uk_ni_driving_licence) | 35 mm wide x 45 mm high | light grey or cream for printed photos (digital photos: plain light-coloured, no patterns or textures, no objects behind you); no shadows | 2026-11-05 |
| United States | [Asylum application photos, Form I-589 (Application for Asylum and for Withholding of Removal)](https://winphoto.io/id/us_i589) | no photo to prepare, or no size published |  | 2026-11-05 |
| United States | [DACA request photos (Form I-821D, Consideration of Deferred Action for Childhood Arrivals, filed with Form I-765)](https://winphoto.io/id/us_daca) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [Diversity Visa (DV, green card lottery) entry digital photo](https://winphoto.io/id/us_dv_lottery) | 2 x 2 inches (scanned prints and selectee interview prints); 600 x 600 px | plain white or off-white | 2026-11-04 |
| United States | [Diversity Visa (DV, green card lottery) entry digital photo for a child or baby listed on the entry](https://winphoto.io/id/us_dv_lottery_child) | 2 x 2 inches (scanned prints and selectee interview prints); 600 x 600 px | plain white or off-white; for a baby, a plain white or off-white sheet, or a car seat covered with one | 2026-11-04 |
| United States | [ESTA (Visa Waiver Program travel authorization), selfie](https://winphoto.io/id/us_esta) | no photo to prepare, or no size published |  | 2026-11-04 |
| United States | [Green Card (Permanent Resident Card) renewal or replacement, Form I-90](https://winphoto.io/id/us_green_card) | no photo to prepare, or no size published |  | 2026-11-04 |
| United States | [Green Card application (adjustment of status), Form I-485 photos](https://winphoto.io/id/us_i485) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [Petition for Alien Fiancé(e), Form I-129F (K-1 fiancé(e) or K-3 spouse) photos of the petitioner and the beneficiary](https://winphoto.io/id/us_i129f) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [Petition for Alien Relative, Form I-130 / I-130A, spouse petition photos (petitioner and spouse)](https://winphoto.io/id/us_i130) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [Petition to Remove Conditions on Residence, Form I-751 (10-year Green Card)](https://winphoto.io/id/us_i751) | no photo to prepare, or no size published |  | 2026-11-04 |
| United States | [U.S. Certificate of Citizenship photos, Form N-600, and replacement naturalization/citizenship document photos, Form N-565 (applicants living outside the U.S.)](https://winphoto.io/id/us_n600) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [U.S. naturalization photos, Form N-400 (Application for Naturalization), applicants residing outside the U.S.](https://winphoto.io/id/us_n400) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [U.S. passport (book or card)](https://winphoto.io/id/us_passport) | 2 x 2 inches | plain white or off-white, free of shadows, textures, objects or lines | 2026-11-04 |
| United States | [U.S. passport for a baby or young child (printed photo with Form DS-11)](https://winphoto.io/id/us_passport_baby) | 2 x 2 inches | plain white or off-white, free of shadows, textures or objects; for a baby, a plain white or off-white sheet, or a car seat covered with one | 2026-11-04 |
| United States | [U.S. travel document photos, Form I-131 (advance parole, TPS travel authorization, refugee travel document from abroad)](https://winphoto.io/id/us_travel_document) | 2 x 2 inches | white to off-white | 2026-11-16 |
| United States | [U.S. visa photo (DS-160 / DS-1648 nonimmigrant digital image; DS-260 immigrant visa prints)](https://winphoto.io/id/us_visa) | 2 x 2 inches; 600–1200 x 600–1200 px | plain white or off-white | 2026-11-04 |
| United States | [U.S. visa photo for a baby or child (DS-160 / DS-1648 digital image; DS-260 prints)](https://winphoto.io/id/us_visa_child) | 2 x 2 inches; 600–1200 x 600–1200 px | plain white or off-white; for a baby, a plain white or off-white sheet, or a car seat covered with one | 2026-11-11 |
| United States | [U.S. work permit (Employment Authorization Document, EAD), Form I-765 photos](https://winphoto.io/id/us_work_permit) | 2 x 2 inches | white to off-white | 2026-11-16 |
| Uzbekistan | [Uzbekistan e-visa (e-visa.gov.uz) face photo upload](https://winphoto.io/id/uz_evisa) | 35 x 45 mm at 300 dpi (digital upload) | not stated in words; the face image must follow ICAO Doc 9303, and the portal's own example of an accepted photo has a plain white background | 2026-11-04 |
| Vietnam | [Vietnam e-Visa (evisa.gov.vn) applicant portrait photo](https://winphoto.io/id/vn_evisa) | 4 x 6 cm (digital upload) | white | 2026-11-04 |
| Vietnam | [Vietnam ordinary passport photo (hộ chiếu phổ thông, 4 x 6 cm, white background)](https://winphoto.io/id/vn_passport) | 4 cm x 6 cm | white | 2026-11-15 |

## Method

Every value is taken from the issuing authority's own page (a ministry, an immigration service, a passport office), never from an agency or a visa-centre contractor. Each document's page on winphoto.io quotes the sentences the values come from and gives the date they were read. Rules change: check the official page, linked in `source_url`, before you apply. Only the issuing authority decides whether it accepts a photo.

Found a rule that has changed? Open an issue with the link to the official page.

## Licence and credit

The compilation is released under [CC BY 4.0](LICENSE): reuse it freely with a credit and a link, for example:

> WinPhoto, "Passport and visa photo sizes of the world: 164 documents, each from the official rule". Rules read up to 17 November 2026. https://winphoto.io/id/photo-sizes

The rules themselves belong to the authorities that publish them. WinPhoto is independent and not affiliated with any government.
