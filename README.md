Improvements:

1. ClientService/src/main/java/com/antra/report/client/service/ReportServiceImpl.java
   - "sendDirectRequests" method now uses threadpool to perform paralell process
   - "getFileBodyByReqId" method now enables both PDF and Excel files to get file from Amazon S3 rather than the local. 
2. ExcelService/src/main/java/com.antra.evaluation.reporting_system/service/ExcelServiceImpl.java
   - Added Amazon S3 Bucket so that excel could, following what PDFService has achieved, perform operations related to   S3 bucket as well.
   - "generateFile" method now could make the excel file store on Amazon S3 bucket after the file is generated and del   ete the local one
