# CheckScheduledTask
This script checks the event logs for actions on an individual scheduled task and emails the events to chosen recipients.

Get-WinEvent uses the following filed sin the hashtable:
ProviderName - This is the Event provider, in this example it is "Microsoft-Windows-TaskScheduler" change this of you are looking for other events
Data - This is anything that is contained in the "Data Name" filecs of the XML ... look on the Additional Data tab of the event in event viewer
StartTime - this is the earliest event the script will find. I have it set to one day i.e. only go back to this time yesyerday

There are no parameters currently, you need to run this on the server that hold the logs you are checking
