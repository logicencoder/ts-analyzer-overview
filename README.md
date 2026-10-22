# TS Analyzer

A television stream can look unstable for several different reasons: reception, tuning, transport errors or the content being carried. TS Analyzer brings those checks into a browser workspace, helping the operator investigate SAT>IP and DVB streams without jumping between several diagnostic utilities.

## Tech stack

| Layer | Technologies |
|---|---|
| Core stack | Rust; Python; FastAPI; JavaScript; HTML; CSS |

## Find a source and prepare a scan

Device discovery and manual source controls support selecting available equipment. Satellite and transponder lists help organise a scan around the intended target. Start and stop controls keep the investigation deliberate rather than leaving an unknown scan running.

## Inspect the scan results

A results workspace collects the available findings so they can be reviewed after scanning. Transponder and service information connect a result with the source being examined. JSON export supports retaining the findings for further analysis.

## Examine the transport stream

The analyser brings bitrate, active stream identifiers, continuity errors and timing information together. This helps distinguish a stream that is arriving from one whose transport has problems. Programme and service information give the diagnostic readings their content context.

## Keep reception and transport separate

When a supported receiver supplies radio-frequency measurements, the dashboard can show reception information alongside transport observations. These are different measurements: receiving packets does not by itself establish radio-signal quality. Unavailable receiver measurements should remain unavailable rather than being inferred from bitrate.

## Explore supporting diagnostics

Constellation and available signal-related views provide another route into the investigation when supported by the equipment and captured information. Settings and device controls keep the source selection close to the analysis. The result is a connected workflow from finding a source to retaining useful diagnostic evidence.

---

Private code: [ts-analyzer](https://github.com/logicencoder/ts-analyzer)

See [REPOS.md](REPOS.md) for related repositories.

**[Logic Encoder](https://logicencoder.com)** · [GitHub](https://github.com/logicencoder) · [Contact](https://logicencoder.com/contact/)
