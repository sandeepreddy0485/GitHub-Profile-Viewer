# 👨‍💻 GitHub Profile Viewer

A modern and responsive web application that allows users to search for any public GitHub profile and explore developer information, repositories, statistics, and activity using the **GitHub REST API**.

The application is built using **HTML, CSS, and JavaScript** and provides a clean dashboard-style interface for exploring GitHub profiles.

---

## 📌 Project Overview

GitHub contains millions of developer profiles and open-source repositories. While GitHub provides detailed information about each user, developers may want a simple and visually organized way to quickly explore public profile information.

The **GitHub Profile Viewer** provides an easy-to-use interface where users can enter a GitHub username and instantly retrieve publicly available profile and repository information.

The application communicates with the **GitHub REST API**, processes the returned data, and displays it through a responsive user interface.

---

## 🎯 Objectives

The main objectives of this project are:

- Search for GitHub users by username
- Fetch public profile information using the GitHub REST API
- Display developer profile statistics
- Fetch and display public repositories
- Calculate repository-related statistics
- Provide direct access to GitHub profiles and repositories
- Handle invalid usernames and API errors
- Maintain recent searches
- Build a responsive user interface
- Practice asynchronous JavaScript and REST API integration
- Deploy the application using Vercel

---

## ✨ Key Features

### 🔍 GitHub User Search

Users can enter a GitHub username to search for a public GitHub profile.

```text
Enter GitHub Username
        │
        ▼
     Search
        │
        ▼
   GitHub REST API
        │
        ▼
  Fetch User Profile
        │
        ▼
 Display Profile Data
```

---

### 👤 Profile Information

The application displays publicly available GitHub profile information such as:

- Profile picture
- Name
- GitHub username
- Bio
- Location
- Company
- Blog or website
- Account creation date

The exact information displayed depends on the data publicly available for the searched GitHub account.

---

### 📊 Profile Statistics

Users can quickly view important GitHub statistics, including:

- Public repositories
- Followers
- Following

Additional repository data can also be processed to provide useful developer insights.

---

### 📁 Repository Viewer

The application fetches and displays public repositories associated with the searched GitHub user.

Repository information may include:

- Repository name
- Description
- Programming language
- Star count
- Fork count
- Repository link

Users can directly visit repositories from the application.

---

### ⭐ Repository Statistics

The application can process repository information to provide statistics such as total stars received across public repositories.

```text
Public Repositories
        │
        ▼
 Fetch Repository Data
        │
        ▼
   Process Statistics
        │
        ├── Stars
        ├── Forks
        └── Languages
        │
        ▼
 Display Developer Insights
```

---

### 🕒 Recent Searches

The application keeps track of recently searched GitHub usernames, making it easier to revisit previously viewed profiles.

---

### 🔗 Quick Profile Access

Users can directly open the searched user's GitHub profile from the application.

The interface also provides convenient access to individual repositories.

---

### 📋 Copy Profile Link

The application provides functionality for easily copying or accessing the GitHub profile link of the searched user.

---

### ⏳ Loading State

A loading indicator improves the user experience while profile and repository information is being retrieved from the GitHub API.

```text
Search User
    │
    ▼
Loading...
    │
    ▼
API Response
    │
    ▼
Display Results
```

---

### ⚠️ Error Handling

The application handles common errors such as:

- Invalid GitHub usernames
- User not found
- Network errors
- API request failures

This ensures users receive useful feedback instead of encountering a broken interface.

---

### 📱 Responsive Design

The application is designed to work across different devices, including:

- Desktop
- Laptop
- Tablet
- Mobile

---

## 🏗️ System Architecture

```text
                     User
                       │
                       ▼
              GitHub Profile Viewer
                       │
                       ▼
                 Search Username
                       │
                       ▼
                JavaScript Fetch
                       │
                       ▼
                GitHub REST API
                       │
              ┌────────┴────────┐
              │                 │
              ▼                 ▼
         User Profile      Repositories
              │                 │
              ▼                 ▼
       Profile Details    Repository Data
              │                 │
              └────────┬────────┘
                       │
                       ▼
                 Data Processing
                       │
                       ▼
              Statistics & Results
                       │
                       ▼
              Responsive Dashboard
```

---

## 🔄 Application Workflow

### Step 1 – Enter Username

The user enters a valid GitHub username into the search field.

### Step 2 – Send API Request

JavaScript sends requests to the GitHub REST API.

Conceptually:

```text
GitHub Username
       │
       ▼
GitHub Users API
       │
       ├───────────────┐
       ▼               ▼
Profile Data     Repository Data
       │               │
       └───────┬───────┘
               │
               ▼
         Process Data
               │
               ▼
       Display Dashboard
```

### Step 3 – Fetch Profile

The application retrieves publicly available user information.

### Step 4 – Fetch Repositories

The application retrieves the user's public repositories.

### Step 5 – Process Statistics

Repository data is processed to calculate or display relevant statistics.

### Step 6 – Display Results

The profile, statistics, and repositories are presented through the user interface.

---

## 🛠️ Tech Stack

### Frontend

- HTML5
- CSS3
- JavaScript

### API

- GitHub REST API

### Icons

- Font Awesome

### Deployment

- Vercel

### Version Control

- Git
- GitHub

---

## 📁 Project Structure

```text
GitHub-Profile-Viewer/
│
├── index.html
├── vercel.json
└── README.md
```

The application uses a lightweight structure, with the primary frontend implementation contained in `index.html`.

---

## 🔌 GitHub API Integration

The application uses GitHub's public REST API to retrieve user and repository information.

The general data flow is:

```text
User Search
    │
    ▼
GitHub Username
    │
    ▼
API Request
    │
    ▼
GitHub REST API
    │
    ├── User Information
    │
    └── Repository Information
    │
    ▼
JSON Response
    │
    ▼
JavaScript Processing
    │
    ▼
Update User Interface
```

The application demonstrates practical experience with:

- REST APIs
- HTTP requests
- JavaScript Fetch API
- JSON data processing
- Asynchronous JavaScript
- DOM manipulation
- Error handling

---

## 🚀 Getting Started

### Prerequisites

You only need:

- A modern web browser
- Git

No backend server or database is required for the basic application.

---

## 📥 Clone the Repository

Clone the repository:

```bash
git clone https://github.com/sandeepreddy0485/GitHub-Profile-Viewer.git
```

Navigate to the project:

```bash
cd GitHub-Profile-Viewer
```

---

## ▶️ Run Locally

Since this is a frontend web application, you can open:

```text
index.html
```

directly in your browser.

For a better development experience, you can also use a local development server such as the **Live Server** extension in Visual Studio Code.

---

## ☁️ Deployment

The project includes a Vercel configuration file:

```text
vercel.json
```

### Deploy with Vercel

1. Push the project to GitHub.
2. Sign in to Vercel.
3. Import the `GitHub-Profile-Viewer` repository.
4. Configure the project if required.
5. Deploy.

Vercel can automatically redeploy the application whenever new changes are pushed to the connected branch.

---

## ⚠️ GitHub API Rate Limits

The GitHub API applies rate limits to requests.

Unauthenticated API requests have lower rate limits than authenticated requests.

If the application receives many requests within a short period, GitHub may temporarily limit additional API calls.

A future version of the project can use secure authenticated API requests through a backend service to support higher request limits.

> GitHub access tokens should never be exposed directly in frontend JavaScript or committed to a public repository.

---

## 💡 Use Cases

The GitHub Profile Viewer can be useful for:

### 👨‍💻 Developer Exploration

Quickly exploring public GitHub profiles.

### 📁 Repository Discovery

Viewing repositories created by a particular developer.

### 📊 Developer Insights

Getting a quick overview of public profile and repository statistics.

### 🎓 Learning REST APIs

Demonstrating practical integration with a third-party REST API.

### 💼 Portfolio Projects

Showing frontend development, API integration, asynchronous JavaScript, and responsive UI skills.

---

## 🔮 Future Improvements

Potential future enhancements include:

- 📊 Programming language distribution charts
- 📈 GitHub contribution visualization
- ⭐ Advanced repository analytics
- 🔥 Most popular repository detection
- 🗓️ Recent activity timeline
- 🔍 Repository search and filtering
- ↕️ Sort repositories by stars, forks, or update date
- 🌙 Dark and light themes
- 📊 Interactive developer statistics
- 👥 Compare two GitHub profiles
- 📄 Export profile summary as PDF
- 🔐 Secure authenticated GitHub API integration
- ⚡ Improved caching
- 📱 Progressive Web App support

---

## ⚠️ Disclaimer

This project uses publicly available information provided through the GitHub API.

The application is an independent educational project and is not affiliated with or endorsed by GitHub.

---

## 👨‍💻 Developer

**Sandeep Reddy Yaramala**

B.Tech Computer Science & Engineering Student

Interested in:

- Software Engineering
- Full-Stack Development
- Artificial Intelligence
- Machine Learning

### GitHub

@sandeepreddy0485

---

## 🤝 Contributing

Contributions and suggestions are welcome.

To contribute:

1. Fork the repository.
2. Create a feature branch:

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes.

4. Commit your changes:

```bash
git commit -m "Add new feature"
```

5. Push your branch:

```bash
git push origin feature/your-feature-name
```

6. Open a Pull Request.

---

## ⭐ Support

If you find this GitHub Profile Viewer useful or interesting, consider giving the repository a ⭐.

---

## 📄 License

This project is intended for educational and personal development purposes.

---

### 👨‍💻 GitHub Profile Viewer

**A responsive GitHub profile exploration application built with HTML, CSS, JavaScript, and the GitHub REST API.**
