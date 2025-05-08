# Answers to Questions about the RecoNotas Bot

## Data Management

**How is data managed from creation to deletion?**  
Data is generated when YOU, as the user, create notes or reminders, and it is stored in a SQLite database (which has SQL syntax similar to Oracle). Data can be deleted manually with commands like `/deletenote` or automatically after reminders are sent and saved in a `.bd` file.

**What strategy do you follow to ensure data consistency and integrity?**  
I use SQL transactions to prevent data corruption and validations to avoid errors such as SQL injections (the AI recommended SQLite because it is lightweight and helps avoid errors).

**If you don't work with data, how could you include a data management feature?**  
I could allow users to save links, files, or tasks in a local or cloud-based database.

---

## Cloud Storage

**If your software uses cloud storage, how do you ensure security and availability?**  
Currently, I don't use the cloud. I thought about syncing it with Google Calendar, but ran into difficulties with the API.

**What alternatives did you consider, and why did you choose your current solution?**  
I considered Firebase, PostgreSQL, and OracleSQL (which I used last year), but I chose SQLite because the AI recommended it as less error-prone, more flexible, and simpler.

**If you don’t use the cloud, how could you integrate it in future versions?**  
I could integrate the cloud to sync data across devices using Google accounts... No promises though 😅

**EDIT:**  
I had already tried and it didn’t work as expected, so I temporarily discarded the idea.

---

## Security and Regulation

**What security measures have you implemented?**  
I use a local database (SQLite) and validate inputs to avoid SQL injections. I also restrict data access per user.

**What regulations might affect the use of your software?**  
If the project scales up, I would need to comply with GDPR by implementing privacy policies and data encryption—beyond just improving code, which sometimes gives me issues.

**If you haven't implemented security measures, what risks do you identify?**  
The main risk is unauthorized access to the database. I would address it with authentication and encryption.



NOTE: When enabling 2FA, copy the code it returns; without it, you won’t be able to access the program and its database.

---

## Involvement of Digital Enabling Technologies (THD) in Business and Industrial Settings

**What impact could your software have in a business or industrial environment?**  
It could be used to manage tasks, meetings, or maintenance, improving day-to-day organization. For example, if you forgot to schedule an appointment in your calendar, you can set it up in the bot with the date and time.

**How could it improve operational processes or decision-making?**  
By organizing tasks and reminders, it would reduce errors due to forgetfulness and improve productivity.

**If it doesn't directly apply, what other settings could benefit?**  
Educational institutions or software development teams could use it to manage tasks and deadlines.

---

## Improvements in IT and OT

**How can your software facilitate integration between IT and OT?**  
It could integrate with IT and OT systems to manage alerts and tasks like preventive maintenance.

**What processes could benefit from your solution?**  
Processes such as inventory management, preventive maintenance, or project planning.

**If it doesn't apply to IT or OT, how could you adapt it?**  
It could be adapted to manage software development tasks, such as reminders to review code.

---

## Digital Enabling Technologies (THD)

**What THD have you used or could integrate?**  
Currently, I haven’t used THD directly, but a large part of the project was driven by AI—it helped with the database, code, and more.

**How would these technologies improve your software?**  
They would make the software more proactive and personalized, improving user experience.

**If you haven’t used THD, how could you implement them?**  
I could use AI for recommendations or IoT to remind users of tasks related to smart devices.

**EDIT:**  
- In version 2.2, I implemented data encryption and started testing, but it didn’t work due to a coding error.

- In version 2.3, several bugs were fixed and encryption began working, but the option/command wasn’t in the guide nor was there a button for it.

- In version 2.5 (the current version), the help command and its button were added to enable 2FA—currently working without errors.

---

# THAAAT'S ALL FOLKS 🎉

[ Back ↩](../ReadMe.md)
