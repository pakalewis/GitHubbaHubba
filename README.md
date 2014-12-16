Week 3 project for the Code Fellows iOS Development Accelerator

This is a sample client app to access your GitHub account.
The user can log in and view their profile, search for repos, and search for other users.

__________________________________________________________________________________________
![](https://github.com/pakalewis/GitHubbaHubba/blob/master/screenshot1.png)
__________________________________________________________________________________________
![](https://github.com/pakalewis/GitHubbaHubba/blob/master/screenshot2.png)
__________________________________________________________________________________________


Features:
- UITableView
- NSURLSession
- UISearchBar
- NSUserDefaults
- WKWebView
- OAuth access to GitHub
- Split view controller
- Network calls to GitHub API
- JSON parsing
- Extension of the String class which has function that uses Regex (NSRegularExpression)



Monday
- Implement a split view controller in your app to control your interface
- Create a network controller and implement a method that fetches repositories based on a search term.
- Create a RepositoryViewController and parse through the JSON returned fromm the server into model objects and display the results in a table view.
- Devise a way to show the master view controller when the app is first launched on iPhone, not the detail view controller.

Tuesday
- Implement an OAuth workflow in your app that successfully lets the user authenticate with your app.
- Recreate a NSURLSession with a NSURLSessionConfiguration with the Authorization Header Field matched up with our oath token.
- Implement a UISearchBar on your repo search view controller and modify your repo search fetch method on your network controller to use the search bar’s text. Be sure to only be making authenticated network calls using your oath token!
- Display the repo’s they searched for a in the table view
- Implement user defaults to store the authorization token, so it only does the OAuth process once.

Wednesday
- Create a UserSearchViewController that searches for users, similar to how we are already searching for repositories. Instead of a table view, use a collection view to display the users avatar image and their name.
- Upon clicking on a cell, implement a custom transition, and transition the image clicked on to a UserDetailViewController page that has their picture, name, and whatever other info you want pulled from their API.

Thursday
- Implement Regex in your app. Use it to validate the characters the user types into the search bar. Extend String with this functionality.
- Implement WKWebView in your app. When a user clicks on a repo, show their repo's web page with WKWebView.


Challenges:
- Implement the 'My Profile' view controller in your app. This should display info about the currently logged in user (their bio, if they are hirable, their count of public and private repos, etc).