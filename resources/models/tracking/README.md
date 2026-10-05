# Tracking models

CVKit owns the NanoTrack (`backbone.onnx`, `neckhead.onnx`) and ViT tracker
(`vitTracker.onnx`) model profiles. Download locations and backend selection
live in `src/services/tracking/tracking_service.cpp`.

Downloaded weights belong in `${F8_MODEL_ROOT}/tracking`, outside the extension
installation. Existing models are reused; automatic download is controlled by
the service's `autoDownloadModels` setting. Extension updates and uninstalls
preserve these files.
