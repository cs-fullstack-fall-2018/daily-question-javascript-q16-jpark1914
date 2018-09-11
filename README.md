# Daily Question - JavaScript Try/Catch

### Try/Catch/Throw
MSJS practice question 19

The body of the HTML page contains the following script: 
```
    <script>
             const fileInfo = 'Could not process the file';
             const reportInfo = 'The daily report was not generated';
             const invoiceInfo = 'The invoices were not created';
             try {
                      logInfo(fileInfo, reportInfo, invoiceInfo);
             }
             catch (e) {
                      console.log('Could not call the function to log the info!');
             }
             finally {
                      console.log('Executed the finally block');
             }

             function logInfo(info) {
                      let date = new Date();
                      console.log(`INFO: ${info}; LOGGED ON ${date}`);
             }
    </script>
```
* What will be displayed in the console when this page is previewed in the browser?

1) 
INFO: Could not process the file; LOGGED ON Fri Nov 03 2018 20:19:53 GMT-0400 (Eastern Standard Time)

Could not call the function to log the info! 

Executed the finally block


2) 
Nothing will print as a 'too many arguments' exception will be thrown when it calls the ```logInfo()``` function


3) 
INFO: Could not process the file; LOGGED ON Fri Nov 03 2018 20:19:53 GMT-0400 (Eastern Standard Time) 

Executed the finally block 


4)
Could not call the function to log the info!


The answer is 3
