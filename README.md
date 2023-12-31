Prerequisite

1. Install JDK 11/8 version
2. Setup Environment variable for JAVA
3. Update build.gradle with below mentioned properties of testNG-
        For JAVA 11: testImplementation 'org.testng:testng:7.6.1';
        For JAVA 8: testImplementation group: 'org.testng', name: 'testng', version: '6.11';
4. Install IntelliJ IDEA 2022.22 (Community Edition)
5. Open this project as gradle project.
6. Connect your machine to internet for building/resolving the dependencies.
7. Now build the application.
8. Set up build path -> File->Settings->Build->Gradle->Run set with selecting Itillej Idea.
8. Execute any test case with connecting the internet( this is for the first time).
9. Update the config.properties with proper credentials according to the testing environment.

Step 1:
a. Execute the CorpNetApp/pom/Ops_TestSuiteExecution.01_TestSuite_CompanyAndAccountCreateWithAuthorize.xml

Step 2:
a. Configure index number with the created new company in "searchCompany" testcase of "TC_CreateMemberWithAllValidDataForBoth" Class
Path : CorpNetApp.pom.test.testOperation.TestCases_CompanyManagement.TestCase_MemberSetupAndSignatorySetup;
b. Execute the CorpNetApp/pom/Ops_TestSuiteExecution/02_TestSuite_CompanyMemberCreateAndApproveForBothCorpAndPayroll.xml

Step 3:
a. Configure index number with the created new company in "selectCompany" testcase of "TC__CreateSignatoryRulesForCorporateWithValidData" and "TC__CreateSimpleSignatoryRulesForPayrollWithValidData"Class
b. Execute the CorpNetApp/pom/Ops_TestSuiteExecution/03_TestSuite_CompanySignatorySetupAndApprove.xml

Step 4:
a. Configure index number with the created new company in "selectCompany" testcase of "TC_ReceiverSetupByComMaker" and "TC_ReceiverLimitSetupByComMaker" Classes
b. Execute the CorpNetApp/pom/Ops_TestSuiteExecution/04_TestSuite_CompanyTCSA_SetupByOps_MakerAndChecker.xml

Step 5:
a. Configure index number with the created new company in "selectCompany" all testcases of "CorpNetApp/pom/test/testOperation/TestCases_UserManagement" Package
b. Execute the CorpNetApp/pom/Ops_TestSuiteExecution/05_TestSuite_CompanyTranUsersSetup.xml

Step 6:
a. Provide company value with the created the new company in "selectCompany"  of All setting page like "CorpNetApp/pom/page/operation_Maker_MenuPages/ChargeSetupPage.java"
b. Execute the CorpNetApp/pom/Ops_TestSuiteExecution/06_TestSuite_CompanySetting.xml

Step 7:
 Prerequisite:
 1. Transaction User setup from config.properties
 2. DD bulk file prepare and provide valid SI Start Date and End Date for both own and Other transaction
 3. Check Beneficiary List for IFT,EFT,RTGS and Payroll Transactions for single transaction
 4. Self Account setup for Own Transfer for both DD & special Auth transaction.
 5. Execute CorpNetApp/pom/TransactionTestSuiteExecute/TransactionsTestSuite/AllTransactionTestSuiteExecute.xml
 or below individual Transaction Suite
    a. All_EFTTestSuiteExce.xml
    b. All_IFTTestSuiteExce.xml
    c. RTGS_TestSuiteExce.xml
    d. Payroll_TestSuiteExce.xml
    e. Sepcial_Auth_TestSuiteExce.xml
    f. DD_TestSuiteExce.xml

Step 8: Test

