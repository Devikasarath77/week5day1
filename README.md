# week5day1

@test
user can run the testcase sequencely and parallely 
sequence - each test cases will be executing one by one 
parallel- if there are 2-3 testcase then it run parallely execute in browser at atime  - class,methods,test(tc1,TC2 - each case4 TC and threadcount is 2 , it execute the first 5 cases parallel and then it execute the next 5will be executed )
        
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                       -------------##parallel execution ---------------
-------===================================-------------------------  
  <?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">
<suite parallel="classes" name="Suite" thread-count="3">
  <test  parallel="classes" name="Test">
    <classes>
      <class name="testNGPra.Createleads"/>
      <class name="testNGPra.EditLead"/>
      <class name="testNGPra.LearnAlert"/>
      <class name="testNGPra.LearnFrame"/>
    </classes>
  </test> <!-- Test -->
  <test name="Test1">
    <classes>
      <class name="testNGPra.LearnAlert"/>
      <class name="testNGPra.LearnFrame"/>
    </classes>
  </test> <!-- Test -->
</suite> <!-- Suite -->
----------==================================-----------------------------------------------------------------------------------------------------------------------------



   failed tested cases are executed from test-output folder- failed.xml file 
- we can add the failed methods( in real time signle class  with mutliple methods are used and so that we can execute the failed methods alone via failed test .xml file 

## still more need to be updated 
