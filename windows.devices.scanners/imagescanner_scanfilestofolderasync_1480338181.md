---
-api-type: winrt method
---
 It takes a few seconds before the scanner stops scanning.
 It stops only when it runs out of paper (for a Feeder acquisition).
 It completes running the scan head to the end of the bed and then fully returns the scan head to its parked location (for a Flatbed acquisition).
 The WIA’s HRESULT of S_FALSE will be translated to a canceled async call (AsyncStatus.Canceled).
 The WIA’s WIA_ERROR_PAPER_EMPTY will be translated by this API to a successful return (AsyncStatus.Completed) with an empty list of files (IVectorView.Size set to 0).