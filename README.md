# wh-automation-framework

Pre requisutes: 
- JAVA_HOME is preferabley JDK 1.7 or above
- Maven installation configured (M2_HOME or bundled version with IDE (intelliJ)
- project cloned and imported as a maven project 

Running the autmated tests on Desktop: 

Junit  - create a Junit run config pointing at RunCucumberTests.java 
  - the following cmd line argument can be set for running on mobile (ChromeDriver - Nexus 5 "-DdeviceType=mobile" if this is absent or anything else, the tests will be on Desktop (Chrome Driver).
  --NOTE-- Running the pack with Junit will not generate the pretty Cucumber report
  - An unstyled report will be generated in: target/cucumber
  
Maven - create a maven run config containing  "clean test" 
  - the following cmd line argument can be set for running on mobile (ChromeDriver - Nexus 5 "-DdeviceType=mobile" if this is absent or anything else, the tests will be on Desktop (Chrome Driver).
  - Running this way will generate the cucumber report
  
Cucumber report 
 - If running with mvn, after test completion find the report in: target/cucumber-reports-cucumber-html-reports
