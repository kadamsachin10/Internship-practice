# Day 4 – Manual Testing vs Automation Testing

## 1. Task

**Topic:** Manual Testing vs Automation Testing

**Objective:** To understand Manual Testing and Automation Testing, their approaches, advantages, limitations, and suitable use cases.

### Topics Covered
1. Manual Testing Approach
2. Automation Testing Approach
3. Advantages of Manual Testing
4. Limitations of Manual Testing
5. Advantages of Automation Testing
6. Limitations of Automation Testing
7. Suitable Use Cases

---

## 2. Manual Testing Approach

### Definition
Manual Testing is a type of software testing in which a tester checks an application manually without using automation scripts.

### Example
Suppose we want to test a Login Page.

1. Open the Login Page.
2. Enter the username and password manually.
3. Click the Login button.
4. Check whether the login is successful.
5. Compare the actual result with the expected result.
6. If the actual result does not match the expected result, report a bug.

---

## 3. Advantages of Manual Testing

### 1. Easy to Learn
Manual Testing is easy to start learning because coding knowledge is not required initially.

### 2. Suitable for New Features
When a new feature is developed, we may not know whether it is stable or whether its requirements will change. Manual Testing is useful for initial testing and understanding the feature.

### 3. Suitable for Frequently Changing Features
If a feature changes frequently, automation scripts may need to be updated repeatedly. Manual Testing may be more convenient in such situations.

### 4. Suitable for Usability Testing
Manual Testing helps check whether an application is easy to use. Human observation and judgment are important for evaluating the user experience.

---

## 4. Limitations of Manual Testing

### 1. Time-Consuming
Manual Testing takes more time when many test cases need to be executed repeatedly.

**Example:** If 100 test cases need to be executed after every new build, the tester must execute them manually each time.

### 2. More Human Effort
The tester needs to execute each test case manually, which requires more time and effort.

### 3. Human Errors
A tester may accidentally skip a step, enter incorrect data, or record the wrong result.

### 4. Time-Consuming Compatibility Testing
Testing an application manually across multiple browsers and devices can take a lot of time.

**Example:** Executing the same 100 test cases on Chrome, Firefox, and Edge requires repeated manual execution.

---

## 5. Automation Testing Approach

### Definition
Automation Testing is a type of software testing in which test cases are executed automatically using automation tools and scripts.

### Example
Suppose we want to test a Login Page.

The tester creates an automation script using a tool such as Selenium.

The script:
1. Opens the Login Page.
2. Enters the username and password.
3. Clicks the Login button.
4. Checks whether the login is successful.
5. Compares the actual result with the expected result.

If the actual result matches the expected result, the test passes. Otherwise, the test fails and the issue can be investigated.

---

## 6. Advantages of Automation Testing

### 1. Easy Regression Testing
Regression Testing checks whether existing features are still working correctly after changes are made to the application.

Automation scripts can be executed again to check existing features.

**Example:** When a new Registration feature is added, we can run existing automation scripts for Login and Forgot Password to check whether they still work correctly.

### 2. Easy Compatibility Testing
Compatibility Testing checks whether an application works correctly across different browsers, operating systems, and devices.

With proper configuration, the same automation scripts can be executed across multiple supported browsers.

**Example:** We can use automation scripts to execute 100 test cases across Chrome, Firefox, and Edge.

### 3. Reduced Human Effort
Automation reduces the effort required to execute repetitive test cases manually.

**Example:** If 100 test cases need to be executed after every new build, the tester can run the automation scripts instead of executing every test case manually.

Creating and maintaining automation scripts also requires effort.

### 4. Reduced Human Errors
Automation scripts execute predefined steps consistently. This helps reduce some errors that may occur during manual execution.

However, incorrect scripts or incorrect expected results can also cause errors.

---

## 7. Limitations of Automation Testing

### 1. Difficult to Learn
Automation Testing may be more difficult to learn initially because it requires knowledge of automation tools and scripting.

### 2. Coding Knowledge Required
Many automation tools require coding or scripting knowledge to create and maintain test scripts. Some low-code and no-code tools are also available.

### 3. Difficult to Maintain Frequently Changing Features
If application features change frequently, automation scripts may need to be updated. This increases maintenance effort.

**Example:** If the Login Page layout or functionality changes, the existing automation script may need modification.

### 4. Not Suitable for Fully Evaluating Usability
Automation can check specific conditions, but it cannot fully replace human judgment when evaluating the overall user experience.

### 5. CAPTCHA Is Difficult to Automate
CAPTCHA is designed to distinguish human users from automated programs. Therefore, automating CAPTCHA interactions can be difficult.

### 6. OTP Testing May Require Special Setup
OTP testing can be automated, but it may require a suitable test environment, test OTPs, or access to email and SMS integrations.

### 7. Profile Picture Upload Testing
Profile picture upload can be automated by selecting an image, uploading it, and checking whether the upload is successful. However, checking visual appearance and quality may require manual verification.

**Note:** CAPTCHA, OTP, and profile picture upload are not completely impossible to automate. They may require special configuration or additional verification.

---

## 8. Suitable Use Cases

### A. Manual Testing

**1. Testing New Features**

When a new feature is developed, we may not know whether it is stable or whether its requirements will change.

If we automate it immediately and the requirements change later, we may need to update the automation scripts. Therefore, Manual Testing is useful for initial testing.

**2. Usability Testing**

Manual Testing is useful for checking whether an application is easy to use.

**3. Exploratory Testing**

Manual Testing allows testers to explore the application and identify unexpected issues.

**4. Frequently Changing Features**

Manual Testing may be more convenient when features change frequently and automation scripts require repeated updates.

### B. Automation Testing

**1. Regression Testing of Existing Features**

When a new feature is added, we need to check whether existing features are still working correctly.

**Example:** When a new Registration feature is added, we can execute existing automation scripts for Login and Forgot Password to check whether they still work correctly.

**2. Repetitive Testing**

Automation is useful when the same test cases need to be executed repeatedly.

**3. Compatibility Testing**

Automation can help execute test cases across multiple supported browsers with proper configuration.

**4. Large Test Suites**

Automation is useful when many test cases need to be executed repeatedly.

**5. Stable Features**

Features that are relatively stable and require frequent testing are often good candidates for automation.

**Important:** It is not a strict rule that every new feature must be tested manually or every old feature must be tested through automation. The choice depends on the feature, testing requirements, stability, and available automation scripts.

---

## 9. Manual Testing vs Automation Testing

| Point | Manual Testing | Automation Testing |
|---|---|---|
| Execution | Test cases are executed manually | Test cases are executed using scripts |
| Coding | Not required initially | Often required |
| Repetitive Testing | Can take more time | Can be faster |
| Regression Testing | Repeated execution takes time | Existing scripts can be reused |
| Human Effort | More effort for repetitive execution | Reduces repetitive manual effort |
| Human Errors | Can occur during manual execution | Can also occur due to script errors |
| Usability Testing | Useful for human judgment | Cannot fully replace human judgment |
| Changing Features | May be more convenient in some situations | Scripts may need frequent updates |
| Compatibility Testing | Repeated manual execution can take time | Scripts can run across supported browsers with proper configuration |

---

## 10. Conclusion

Manual Testing and Automation Testing are both important in software testing.

Manual Testing is useful for initial testing of new features, exploratory testing, and usability testing.

Automation Testing is useful for regression testing, repetitive test execution, and compatibility testing across supported browsers.

Both approaches have advantages and limitations. The choice depends on the application, testing requirements, feature stability, and available tools.