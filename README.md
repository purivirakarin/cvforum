# CVForum - Web Forum Application

A modern web forum built with React and Go, featuring user authentication, post management, and real-time commenting.

## Technology

- [React.js](https://reactjs.org/) + [TailwindCSS](https://tailwindcss.com/)
- [Go](https://www.golangprograms.com) + [GORM](https://gorm.io)
- [MySQL](https://www.mysql.com) + [PlanetScale](https://planetscale.com)

## Installation

1. Clone the repository
```bash
git clone <repository-url>
cd cvforum
```

2. Install frontend dependencies
```bash
cd clientv2
yarn install
```

3. Install backend dependencies
```bash
cd server
go get
```

4. Set up MySQL database

5. Configure environment files

**Frontend** (`clientv2/.env`):
```
REACT_APP_BACKEND_URL=<YOUR_BACKEND_URL>
```

**Backend** (`server/.env`):
```
FRONTEND=<YOUR_FRONTEND_URL>
DSN=<DATABASE_CONNECTION_STRING>
PORT=<YOUR_DESIRED_BACKEND_PORT>
```

6. Start the development servers

**Frontend:**
```bash
cd clientv2
yarn start
```

**Backend:**
```bash
cd server
go run main.go
```

## Features

- **User Authentication**: Secure registration and login system with JWT tokens
- **Post Management**: Create, read, update, and delete forum posts
- **Comment System**: Interactive commenting on posts
- **Tag Filtering**: Organize and filter posts by categories
- **Responsive Design**: Mobile-friendly interface with TailwindCSS
- **Real-time Updates**: Dynamic content loading and updates

## Usage

### Navigation

The navigation bar adapts based on authentication status:
- **Authenticated users**: Home, My Posts, Create Post, and Logout options
- **Unauthenticated users**: Home and Login options

### Home Page

The main page displays all forum posts with filtering capabilities by category tags.

### User Authentication

#### Registration
1. Click the "Log In" button in the navigation bar
2. Select "Register here" link
3. Fill in username and password (minimum 6 characters)
4. Click "Register" to create your account

#### Login
1. Click "Log In" in the navigation bar
2. Enter your username and password
3. Click "Log In" to access your account

#### Logout
Click "Log Out" in the navigation bar to end your session.

### Posts

#### Viewing Posts
- **All Posts**: Access from the home page
- **Your Posts**: Click "My Posts" in the navigation bar
- **Full Post**: Click on any post card to view complete content and comments

#### Creating Posts
1. Click "Create new post" in the navigation bar
2. Fill in the title and description
3. Select a category tag
4. Click "Post" to publish

#### Editing Posts
1. Navigate to your post's individual page
2. Click "Edit Post" (only visible for post owners)
3. Modify title, description, or category
4. Click "Edit" to save changes

#### Deleting Posts
1. Go to the Edit Post page
2. Click "Delete" button
3. Confirm deletion

### Comments

#### Viewing Comments
Click on any post to view all its comments on the individual post page.

#### Adding Comments
1. Go to a post's individual page
2. Use the comment box below the post
3. Type your comment
4. Click "Post" to submit

#### Editing Comments
1. Find your comment on the post page
2. Click "Edit" (only visible for comment owners)
3. Modify the comment text
4. Click "Done" to save

#### Deleting Comments
1. Click "Edit" on your comment
2. Click "Delete" to remove the comment

### Filtering Posts

Use the category dropdown on both the Home page and My Posts page to filter posts by specific tags. Select "All" to view posts from all categories, or choose a specific category to narrow down the results.

## Acknowledgments

This project was built with knowledge gained from various online resources and educational content creators, including freeCodeCamp.org, Web Dev Simplified, and other programming tutorials that helped shape the development approach and implementation.
