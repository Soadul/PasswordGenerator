# Password Generator System

একটি সুরক্ষিত পাসওয়ার্ড জেনারেটর সিস্টেম যা Java Swing ব্যবহার করে তৈরি করা হয়েছে।

## বৈশিষ্ট্যসমূহ

- সুরক্ষিত পাসওয়ার্ড জেনারেশন
- পাসওয়ার্ড স্ট্রেংথ অ্যানালাইসিস
- ডার্ক মোড UI
- ক্লিপবোর্ডে কপি করার সুবিধা
- SQLite ডাটাবেসে পাসওয়ার্ড সংরক্ষণ
- AES এনক্রিপশন

## প্রয়োজনীয়তা

- JDK 17 বা তার উপরে
- Maven
- SQLite

## ইনস্টলেশন

1. প্রজেক্টটি ক্লোন করুন
2. Maven ডিপেন্ডেন্সি ইনস্টল করুন:
   ```bash
   mvn clean install
   ```
3. প্রোগ্রাম চালু করুন:
   ```bash
   mvn exec:java -Dexec.mainClass="com.passwordgenerator.PasswordGeneratorApp"
   ```

## ব্যবহার

1. পাসওয়ার্ডের দৈর্ঘ্য স্লাইডার দিয়ে নির্বাচন করুন (৬-৩২ অক্ষর)
2. প্রয়োজনীয় অক্ষর টাইপ সিলেক্ট করুন:
   - বড় হাতের অক্ষর
   - ছোট হাতের অক্ষর
   - সংখ্যা
   - বিশেষ অক্ষর
3. "Generate Password" বাটনে ক্লিক করুন
4. পাসওয়ার্ড স্ট্রেংথ দেখুন
5. "Copy to Clipboard" বাটন দিয়ে পাসওয়ার্ড কপি করুন
6. ডার্ক মোড টগল করুন UI পরিবর্তনের জন্য

## সুরক্ষা বৈশিষ্ট্য

- SecureRandom ব্যবহার করে র্যান্ডম পাসওয়ার্ড জেনারেশন
- AES-256 এনক্রিপশন
- SQLite ডাটাবেসে সুরক্ষিত স্টোরেজ
- পাসওয়ার্ড স্ট্রেংথ অ্যানালাইসিস

## লাইসেন্স

MIT License #   P a s s w o r d G e n e r a t o r 


Software Development Note
1. Project Overview
I developed a password generator software that helps users create secure passwords, store them, and copy them when needed. The software operates through a user-friendly interface and includes a dark mode feature.
2. Technology Stack
Language: Java (JDK 17)
UI Library: Swing
Database: SQLite
Encryption: AES (Advanced Encryption Standard)
Package Manager: Maven
3. Libraries Used
SQLite JDBC: For connecting to the database and managing SQL queries.
Java Swing: For creating the GUI.
Java Preferences API: For storing user preferences.
4. Database Schema
A table named passwords was created in the database, which contains the following columns:
id: Primary key (INTEGER)
website: Name of the website (TEXT)
password: Encrypted password (TEXT)
created_at: Timestamp of when the password was created (TIMESTAMP)
5. SQL Queries
Saving Password:
Retrieving Passwords:
Deleting Password:
6. Software Features
Password Generation: Users can select specific length and character types (uppercase letters, lowercase letters, numbers, special characters).
Saving Passwords: Users can save passwords along with the corresponding website name.
Copying Passwords: Users can double-click on saved passwords to copy them to the clipboard.
Dark Mode: Users can switch the UI to dark mode.
7. Challenges and Solutions
Database Schema Update: Initially, the database did not have a website column, which caused issues. I updated the database schema to add the new column.
UI Design: The UI was modernized and made user-friendly to enhance the user experience.
8. Future Plans
Feature Expansion: In the future, I plan to add more features to the software, such as password strength analysis and storing password history for users.
This note will help you discuss your project in detail during an interview. If you need anything else, just let me know!




 
 
