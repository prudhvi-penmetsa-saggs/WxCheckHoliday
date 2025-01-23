WxCheckHoliday is  an IBM webMethods Integration Server version 11 package to check whether the given date is a Holiday or not. This package has two services
These sevvices uses Common Directory Services business calendars. Please refere to documentation https://docs.webmethods.io/on-premises/webmethods-integration-server/en/11.1.0/pdf/cds-ag-pdf.pdf
to configure holidays in  business calendars. 

Configure the business calendar and define the calendar Alias name in GlobaVariables
Service 1:  CheckHoliday:checkHoliday  service  checks whether given date is a company configure holiday in Common Directory Service Business Calendar
  Inputs:

         date: Enter the date  in yyyy-MM-dd format to check whether this date is a holiday in the business calendar.

  Outputs:
        isHoliday:   true - if the date is a company holiday 
                     false - if the date is a working day

.
Service 2:  CheckHoliday:isTodayHoliday ervice  checks whether the today is a hoiday or not.
   Inputs: None
   outputs:
        isHoliday:   true - if the date is a company holiday 
                     false - if the date is a working day
