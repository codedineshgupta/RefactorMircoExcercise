# RefactorMircoExcercise

**#Telemetry System -**
**TelemetryDiagnosticControls **
    voilating DIP principle. 
    Reason - TelemetryDiagnosticControls class directly depends on the TelemetryClient class, which is a low-level module.This direct dependency creates tight coupling between the two classes and makes it difficult to replace               or extend the TelemetryClient class without modifying the TelemetryDiagnosticControls class.

   
  
