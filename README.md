# RefactorMircoExcercise


**Telemetry System** 

voilating DIP principle. 
   Reason - TelemetryDiagnosticControls class directly depends on the TelemetryClient class, which is a low-level module.This direct dependency creates tight coupling between the two classes and makes it difficult to replace               or extend the TelemetryClient class without modifying the TelemetryDiagnosticControls class.

   
 **TicketDispenser**  

To make the code testabel , I have refactored the TicketDispenser class in order to mock the method - TurnNumberSequence.GetNextTurnNumber();
however there is no obious voilation of any SOLID principle


**TirePressureMonitoringSystem**

Alarm Class -
  voilating DIP principle 
  becase it is creating intance of Sensor class. and hence creating the dependecy on Sensor Class - low level module.
  and hence make the code tough for mocking and non-testable.


 **UnicodeFileToHtmlTextConverter**
 
   Voilation of SRP.
   class - UnicodeFileToHtmlTextConverter - is doing more than one job - read the file and then convert to HTML.
   job to read the file should be delegated to outer module - UnicodeFileReader 
   


  
  
  
