# Planning for Front-End *User Testing*

*What we're testing (and what we're not)*

### Why plan testing now?

- **You get additional clarity on scope.**
  - Knowing which browsers and devices you'll test for helps you focus and saves time.
- **Less explaining (and argument) later with the client.**
  - Setting expectations now for what you'll test reduces misunderstanding later.
- **Less stress before, during, and after launch.**
  - If you've thoroughly tested everything, you can be confident everything displays an performs as expected.

<br />

### You can't test everything.
- Budgets are finite.
  - if you're working for a client, you're working with a budget.
- Schedules are finite.
  - If testing isn't on the schedule, it'll be rushed or left out.
- Not every scenario matters.
  - Your website may not need ot work on *EVERY* device.

<br />

---

<br />

## Creating a Test Plan

### **1. Who are we testing for?**

    - Focus on the scenarios most relevant to your audience:
      - What are the most popular devices they'll use?
      - What OS/browser combinations are most popular among your audience?
      - What connection speeds do they have?
      - How tech-savvy is your demographic?
    - **Use statistical information to identify demographics**
      - W3 Schools (http://www.w3schools.com/browsers/default.asp)
      - Net Market Share (http://www.netmarketshare.com)
      - StatCounter (http://gs.statcounter.com)

### **2. Prioritize Browser & Device Support**

    - Separate testing priorities into categories like below:

      ![04 - Notes - PrioritizeBrowserAndDeviceSupport](./images/04%20-%20Notes%20-%20PrioritizeBrowserAndDeviceSupport.png)

<br />

### **3. Decide What to Test**

<br />

**6 types of testing to perform:**
- Functionality
- Usability
- Errors and Exceptions
- Compatibility
- Performance
- Security

<br />

#### **Functionality:**

- Test all links 
  - internal, external, email/messaging links, and pages the don’t have a link (orphan pages)

- Test forms on all pages 
  - check validations, default values, test incorrect input to fields, test options to CRUD forms (like what an admit would)

- Test cookies 
  - test functionality and security by enabling/disabling cookies 
  - ensure cookies are encrypted before writing to users device 
  - check login sessions and user stats

- Test CSS/HTML Validation 
  - validated HTML 
    - http://validate.w3.org
  - check the site is crawlable 
    - Google.com/webmasters/tools)

- Test Database Connections and Consistency
  - Check data integrity and errors while you edit, delete, modify the forms or do any DB related functionality.
  - Ensure all database queries are executing correctly.
  - Ensure data is retrieved correctly
  - Ensure data is updated correctly

<br />

#### **Usability:**

- Usability Testing covers: navigation, ocntent, presentation, and task success.
  - User serveys such as **Survey Monkey**
  - Videotaped, moderated user sessions
  - Online services such as:
    - UserTesting (http://www.usertesting.com)
    - Loop 11 (http://www.loop11.com)
    - Optimizely (http://www.optimizely.com)
  
<br/>

- Test ease and effectiveness of navigation
  - Do users find what they need easily?
  - How long does it take them to find what they're looking for?
  - Does the structure and organization of the navigation match the user's expectations?
  - Are links labeled with terms that make sense to users?

- Test Usefullness of content:
  - Does content match what your users want/need?
  - Can users find and read the content they need?
  - DO they understand the content?
  - Can they act on the content?

- Test the effectiveness of visual presentation (UI):
  - Do UI elements clearly separate navigation from content?
  - Do UI elements distract or create a barrier between the suer and the content?
  - Do UI elements clearly signal what can be acted upon or interacted with (and how to do that)?
  - Do UI elements work together to guide the user through a particular process or task flow?

- Test Task Success:
  - Were users able to accomplish the key task they can to the site to perform?
  - If so, did they feel satisfied (or frustrated)?
  - If not, what prevented them from succeeding?
  - What's the consequence of each task failure?
    - ie: lost the customer, increased support costs, etc...

<br />

#### **Errors and Exceptions:**

- Error and exception testing covers what heppens when things go wrong - a user enters a bad information, stops a process, the system crashes, etc...
  - Test that interactions between servers are executed properly.
  - Test that errors are handled properly.
  - If the database or web server returns an error make sure error messages are displayed appropriately to users.
  - Make sureerror messages are understandable and instructive.
  - Test for **transaction interruption** or lost connection to a web server.

<br />

#### **Compatibility:**

- What happens when the site is used across different devices, browsers, etc... as well as specifics like mobile browsing and printing.
- Big two are:
  - Browser compatibility
  - OS & device compatibility

**Browser compatibility:**
  - Does the website display consistently in different broswers?
  - Does the website display consistently in the same browser across different OS platforms?
  - Does all functionality (links, forms, etc...) work properly across different browsers?

(*Online tools to simplify testing:
http://mashable.com/2014/02/26/browser-testing-tools/*)

**OS & device compatibility**
  - Does all functionality work properly across different OS platforms/devices?
  - Do web service calls (API) work across devices?
  - Do fonts/CSS styles display properly across devices?

<br />

#### **Performance:**

- Measures how well the website can accommodate heavy user activity. Performance testing should include:
  - Web Load Testing - Site sould be able to handle many simultaneous user requests, large data, multiple database connections, etc...
  - Web Stress testing - Show does the server/site react to stress and revover from crashes? (Input fields, login processes, etc...)

#### **Security:**

- Measures how well teh website (and user/product/transactional data) is protected against hackers
  - Pate an internal url (https) directly into a URL bar without loggin in (page should not open)
  - Try changin url options directly while logged in with specific (unauthorized) credentials 
  - Try some invalid entries in input fields
  - Web directories or files should not be directly accessible
  - Test whether SSL is used for security measures.
  - Check for logs of all transactions, error messages, and security breach attempts (usually on web server)

### Takeaways:
- You need to know three things up front:
  1. What's worth doing?
  2. What are we creating?
  3. What value does it provide?

- If you *ever* hear the words "We have no competition" - Exit the room and don't go back!
- The most important principle of good UI/UX is **Progressive Disclosure**
- 3 kinds of requirements: "Things people..."
  1. Say they need
  2. Actually need
  3. Don't know they need
- When you need to get requirements quickly, **Use Scenarios** are the best way to get them
- **Documentation** eliminates excuses and surprises
- When it comes to interacting with clients, partners or fellow team members **silence equals agreement**.
- If you're doing anything without documentation, you're guessing!
- **You can't test everything**.

