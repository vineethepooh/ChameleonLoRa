# ChameleonLoRa
A dynamic Arduino LoRa wrapper that implements signal-aware frequency adaptation. By monitoring real-time RSSI (Received Signal Strength Indicator), this library allows LoRa nodes to automatically 'hop' to clearer frequencies when interference is detected or signal quality degrades, ensuring a stable communication link.

ChameleonLoRa is an intelligent extension of the Sandeep Mistry LoRa library. In congested RF environments (like the 915MHz or 868MHz ISM bands), interference can significantly degrade signal quality.

This library monitors the RSSI (Received Signal Strength Indicator) of every incoming packet. If the signal strength falls below a defined threshold, the library automatically triggers a frequency shift to a secondary "clear" channel, ensuring your communication link remains robust and resilient.
