# Night Run 3D — vehicle model sourcing

This file tracks candidate assets for the eight requested real-world vehicles. **Do not treat a listing as approved just because it says “royalty-free”:** the downloaded file's exact license, redistribution rules, and any vehicle-brand/design rights must be checked before publication.

## Target asset files

Once licensed files are downloaded, convert/optimize them to self-contained GLB and place them here:

| Game car | Expected file | Sourcing status | Candidate |
|---|---|---|---|
| Nissan Note 2007 | `models/nissan-note-2007.glb` | Exact model family found; year/facelift needs visual check | [CGTrader — Nissan Note](https://www.cgtrader.com/3d-models/car/car/nissan-note), listed as Royalty Free; FBX/OBJ available. Listing describes a detailed, ~180k-polygon model. |
| VW Tiguan Allspace 2020 | `models/vw-tiguan-allspace-2020.glb` | Closest candidate is 2018, not exact 2020 | [CGTrader — Tiguan Allspace 2018](https://www.cgtrader.com/3d-models/car/suv/volkswagen-tiguan-allspace-2018), listed at $129 with Royalty Free License; FBX/OBJ available. Confirm the body matches the requested 2020 version before purchase. |
| VW Passat B6 2010 | `models/vw-passat-b6-2010.glb` | Exact generation found | [3DExport — Passat B6](https://3dexport.com/3d-model-volkswagen-passat-b6-36331). Listing describes Basic/Extended licenses and FBX/GLB formats; verify current price and license checkout details. |
| VW Tiguan 2013 | `models/vw-tiguan-2013.glb` | Exact year found, but candidate license is editorial-only | [Free3D — Tiguan 2013](https://free3d.com/3d-model/volkswagen-tiguan-2013-suv-8241.html) is listed at $99 and includes FBX/OBJ, but the listing says Editorial Only. **Do not use this in the game unless the seller supplies permission for game use.** |
| Volvo S40 2008 | `models/volvo-s40-2008.glb` | Exact year found | [CGTrader — Volvo S40 2008](https://www.cgtrader.com/3d-models/car/car/volvo-s40-2008), listed at $99 with Royalty Free License; FBX/OBJ available. Alternative [Volvo S40 Sedan](https://www.cgtrader.com/3d-models/car/luxury-car/volvo-s40-sedan) at $65, but verify year/body version. |
| Honda Pilot 2012 | `models/honda-pilot-2012.glb` | Exact year found, but candidate is editorial-only | [Free3D — Honda Pilot 2012](https://free3d.com/3d-model/honda-pilot-2012-1775.html), listed at $129 with FBX/OBJ, but Editorial Only. **Do not use in the game unless the seller supplies permission for game use.** Alternative [CGTrader — Honda Pilot-style SUV](https://www.cgtrader.com/3d-models/car/suv/suv-1-c6908406-6427-49a6-a71e-6f971c10e9e3) at $69 is not confirmed to be the exact 2012 Pilot. |
| Lada Granta | `models/lada-granta.glb` | Exact model family found, but visible candidates have editorial-only restrictions | [Free3D — Lada Granta FL](https://free3d.com/3d-model/lada-granta-fl-2581.html), listed at $22, FBX; Editorial Only. [CGTrader low-poly Granta](https://www.cgtrader.com/3d-models/car/car/lada-granta) is listed at $29 but has an Editorial License. **Need a seller-confirmed game-use license before use.** |
| Mitsubishi Colt 2007 | `models/mitsubishi-colt-2007.glb` | Exact model-year candidate not yet confirmed | [CGTrader — abandoned Mitsubishi Colt hatchback](https://www.cgtrader.com/3d-models/car/car/031-abandoned-car-mitsubishi-colt-hatchback) is listed at $14 with Royalty Free License and GLTF, but is weathered/abandoned and not confirmed as the 2007 generation. [3DExport — Mitsubishi Colt](https://3dexport.com/nl/3d-model-mitsubishi-colt-243148) is another candidate; confirm year, formats and license before buying. |

## Integration requirements

- Prefer self-contained `.glb` files with textures embedded. For FBX/OBJ purchases, convert in Blender and pack textures before export.
- Optimize high-poly assets for browser use (especially the 180k–550k polygon candidates); keep a high-quality garage preview and a lighter in-game version if needed.
- Preserve the seller's license receipt and original archive outside the public repository. Only publish the optimized model files if the applicable license permits embedding them in a publicly accessible web game.
- A royalty-free asset license does not automatically grant permission to use a vehicle manufacturer's trademarks or exact protected design in every commercial context. Confirm intended use before commercial release.
- Once the files are available, connect each car's loader entry to the matching GLB, normalize scale/orientation/ground height, and reuse the same model pipeline for traffic.

## Current state

No purchased model binaries have been added yet. Marketplace pages are references only; this avoids copying paid assets or assets with editorial-only restrictions into the repository without a license. The existing game remains unchanged until suitable files are supplied and verified.
