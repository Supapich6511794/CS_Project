#Prerequisites
Dotnet (https://dotnet.microsoft.com/en-us/download)
Run application with : dotnet run
at Windows PowerShell in C:\Users\User\Desktop\AttendanceReports
            

#####   SYSTEM REQUIREMENTS  #####

# Requires dotnet (https://dotnet.microsoft.com/en-us/download)

#Visual Studio Code  


###### FILES INCLUDED ######
##### AttendanceReports #####

#Program.cs

### Infrastructure ###
#CsvMeetingRepository.cs

#### Domain ####

##Repositoriese##
#IMeetingRepository.cs

##Entities##
#InMeetingActivity.cs
#Participant.cs
#MeetingSummary.cs

#### Application ####

##Services##
#InMeetingActivity.cs
#PdfReportService.cs
#ParticipantStatusService

##Interfaces##
#Interfaces.cs
#IParticipantStatusService.cs
#IPdfReportService.cs

#attendance_dummy_data.zip: The ZIP file containing the attendance CSV files.

#README.txt: This file.


##### INSTUCTION FOR USE #####

1.Running the Script: To run the script, open a Windows PowerShell in the the project directory C:\Users\User\Desktop\AttendanceReports, and execute: dotnet run

2.Enter path of CSV file : C:\Users\User\Desktop\attendance_dummy_data
  Enter the late time : 10 (10 minute)
  

3.Attendance Processing: The script will:
  #Read and process the CSV files.
  #Generate a report summarizing the Number of attended sessions, Number of absent sessions, and Number of late sessions.

4.Generated Report: The report will be generated as Attendance_Summary_Report.pdf in the current directory. It contains the following columns:
#Student Name: The name of the student.
#ID/E-mail: The student’s email and ID.
#Number of attended sessions: Number of sessions attended.
#Number of absent sessions: Number of sessions missed.
#Number of late sessions: Number of sessions where the student was late.


##### ERROR HANDLING #####

#PermissionError: If the script encounters a permission error when generating the report, it will output the error message.

#General Errors: Any other exceptions that occur during report generation will be printed to the console.
