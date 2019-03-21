# URL-Shortner: Like bit.ly

Build a simple ruby on rails application that enables URL shortening. A user of the app should be able to create a “short link” for an arbitrary destination URL that will redirect anyone who uses short link to the destination URL.

For example, if the user wants a shortlink for “google.com”, the service will provide them with a URL like “railsapp.com/xyz” (where “railsapp.com” is the domain of our service). Then when anyone navigates to the “railsapp.com/xyz” link, they will be redirected to “google.com”.

## Required Specs:
- Database table of User profiles
- Database table of shortlinks, each linked to the user profile that created it
- REST API for creating short links, only available to authenticated users
- Redirection behavior when navigating to a shortlink

## Extra Credit Specs
- Rate limit the create API to 10 new links per user per minute
- Allow admins to blacklist certain domains of where short links point
- Front end interface for users to create new shortlinks

## Notes:
- The database will be Postgres
- API authentication may be handled any way you like as long as it is secure
- You may use devise for the User table
- The shortlinks may have a static path like  “railsapp.com/s/xyz”
