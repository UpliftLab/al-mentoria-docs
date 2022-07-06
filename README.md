#  Final group capstone - Book an Appointment

### Estimated time: 60h

## Description

The project you are going to build for the Final Capstone Project is based on an app to book an appointment with a mentor. You should follow the given [design](https://www.behance.net/gallery/26425031/Vespa-Responsive-Redesign) of the website.

### Key features

 - All users can see lists and details of different mentors.
 - Logged in users can book an appointment with a mentor.
 - Logged in users can see list of their own appointments.
 - Admin user can add mentors.
 - Admin user can delete mentors.


### Project requirements

#### ERD

![image](https://user-images.githubusercontent.com/11241315/177653953-3439d932-23fb-4f20-872b-7d26f8c440cf.png)


#### Basics
- Follow the layout of [the provided design](https://www.behance.net/gallery/26425031/Vespa-Responsive-Redesign).

#### Features

- **User** (name, email, password, role)
  - Signup
  - logs in
  - Log out
  - User can apply to be a mentor (Phase II)
    - By applying, a new Mentor model is made for this user 1-1 relationship (user can have only one mentor profile)
    - User can delete mentorship profile

- **MentorProfile** (user_id, name, Photo, [mentorTopics], approved(phase II))
  - List (index)
  - Show detail

- **Topic** (label, icon)
  - Only admin can add topics

- **mentorTopics** (mentor, topic, rating)
  - User (owner of the mentor profile set their level of skills for the topic)

- **Reservation** (user, mentor, date, topic)
 - we get these items from the user:
   - Mentor (is filled automatically if we come from mentor detail page otherwise the user selects from dropdown)
   - Date
   - Topic

- In the navigation panel
  - Mentors: to a page with the list of all mentors)
  - Reserve: to Reservation page
  - My reservations: show all reservation of the logged in user (user can delete them as well)
    - Show name, date and topic
  - Add Mentor (only for admin)
    - When the admin clicks the "Add Mentor" link in the navigation panel they can see a form for adding a new mentor.
    - If admin, we see "add mentor", if user, we see "apply for mentorship". (phase II)
  - Delete Mentor (only for admin to get list of mentors to delete)
    - When the admin clicks the "Delete Mentor" link in the navigation panel they can see a list of all items with title and "Delete" button.
    - When the admin clicks the "Delete" button, the selected item is marked as removed and does not show on the main list anymore.
  - Sign in / Sign out

- On the main page, the user can see a list of Mentors
- When the user selects a specific mentor, they can see the details page with its full description.
    - In the details page, the user can click the "Reserve" button

- Make the app responsive.

- Add full documentation for your API.

### Workload distribution

To tackle this challenge, you need to create a Kanban board with a GitHub project that translates the requirements into a set of tasks that you will be able to use to organize your work. You will create your board in a separate activity.
