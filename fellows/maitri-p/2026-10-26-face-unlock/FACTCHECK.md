# FACTCHECK — face-unlock

| # | Claim (beat) | Verdict | Source |
|---|---|---|---|
| 1 | Face ID projects more than 30,000 invisible infrared dots; IR camera reads them into a depth map; flood illuminator works in the dark (B01) | TRUE | Apple, "About Face ID advanced technology" |
| 2 | Depth sensing means a flat photo doesn't unlock it (B01) | TRUE — Apple states Face ID is designed to resist photo/mask spoofing | Apple, same page |
| 3 | A neural network converts the capture into a mathematical representation; similar faces → similar numbers; unlock if close enough to the enrolled one (B02) | TRUE — Apple: depth map and IR image are converted to a mathematical representation and compared to enrolled data; "embedding/distance" is the standard description | Apple; general ML |
| 4 | Threshold trade-off: stricter = fewer false accepts, more false rejects (B03) | TRUE — standard FAR/FRR trade-off | General |
| 5 | Attention-aware by default: eyes open, looking at the device (B03) | TRUE | Apple |
| 6 | Adapts to gradual changes (beard, glasses, ageing) (B03) | TRUE | Apple |
| 7 | Data encrypted, kept in the Secure Enclave, stays on device, not backed up to iCloud (B04) | TRUE | Apple |
| 8 | Random-person match < 1 in 1,000,000 (single enrolled appearance); higher for twins, look-alike siblings, under-13s (B04) | TRUE as Apple states it | Apple |
| 9 | Many Android phones use the 2D front camera; some can be fooled by a photo; banking apps often reject it (B05) | TRUE in general — Android classes many camera-only face unlocks below the "strong" biometric tier, which apps requiring strong biometrics won't accept. Not every Android phone; "many" / "some" kept | Android biometric classes (Class 3 "strong" vs lower) |
